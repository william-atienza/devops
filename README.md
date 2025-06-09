# DevOps
Page for DevOps

## Harbor Container Registry
- Make sure docker and OpenSSL is installed
- `$ wget https://github.com/goharbor/harbor/releases/download/v2.13.1/harbor-online-installer-v2`
- `$ tar xzvf harbor-online-installer-v2.13.1.tgz`
- `$ cd harbor`
- `$ cp harbor.yml.tmpl harbor.yml`
- `$ vim harbor.yml`
- `$ sudo ./install.sh`
- Access http://localhost/ using user: `admin`, password: `<the passyourd you configured in harbor.yml>`
- Reference: https://goharbor.io/docs/2.13.0/install-config/download-installer/
  
