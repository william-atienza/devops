# DevOps
Page for DevOps

## Harbor Container Registry
- Make sure docker and OpenSSL is installed
- Download Harbor installer: `$ wget https://github.com/goharbor/harbor/releases/download/v2.13.1/harbor-online-installer-v2`
![01_install harbor.png](instructions/harbor/01_install%20harbor.png)
- Extract: `$ tar xzvf harbor-online-installer-v2.13.1.tgz` ![02_extract.png](instructions/harbor/02_extract.png)
- Change directory to harbor folder: `$ cd harbor` ![03_cd to harbor.png](instructions/harbor/03_cd%20to%20harbor.png)
- Duplicate and rename to harbor.yml and edit the content: `$ cp harbor.yml.tmpl harbor.yml` followed by
`$ vim harbor.yml` 
![04_copy and update harbor yaml file.png](instructions/harbor/04_copy%20and%20update%20harbor%20yaml%20file.png) 
![change hostname and comment out https.png](instructions/harbor/change%20hostname%20and%20comment%20out%20https.png)
![change default UI password.png](instructions/harbor/change%20default%20UI%20password.png)

- Install: `$ sudo ./install.sh` ![05_execute install shell script.png](instructions/harbor/05_execute%20install%20shell%20script.png)
- Access http://localhost:8088/ using user: `admin`, password: `<the passyourd you configured in harbor.yml>`
![UI login.png](instructions/harbor/UI%20login.png)
- Reference: https://goharbor.io/docs/2.13.0/install-config/download-installer/
  
