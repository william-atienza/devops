# WSL2 on Windows

## Check running servers
`wsl -l -v`
![wslcommand.png](wslcommand.png)

## Export distro
- `wsl --terminate <DistributionName> <Filename>`
  - `wsl --terminate Ubuntu`
     ![terminatedistro.png](terminatedistro.png)
     ![terminateddistro.png](terminateddistro.png)
- `wsl --export <DistributionName> <Filename>`
  - `wsl --export Ubuntu C:\Users\william\dev\wls2\exports\UbuntuWsl.tar`
     ![exporttowindows.png](exporttowindows.png)
  - 
## Import distro
- `wsl –import <Image Name you choose> <Directory to store and run the image> 
    <Directory location of the exported .tar file>`
   - `wsl --import UbuntuCustomServer 'C:\Program Files\WSL\imported\UbuntuCustomServer' 'C:\Users\william\dev\wls2\exports\UbuntuWsl.tar'`
  ![importfromwindows.png](importfromwindows.png)

## Run distro
- `wsl -d <ImageName>`
  - `wsl -d UbuntuCustomServer`. Notice on the terminal that it will switch to WSL directory. It means that the image successfully run. 
  ![rundistro.png](rundistro.png)