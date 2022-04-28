# Instalación de Odoo 15 CE

Israel Ubeda Bravo | Chile
- Email: israel.ubedabravo@gmail.com
- Github: https://github.com/israelubeda


## 1- Instalacion de PostgreSQL database

```linux
sudo apt update 
sudo apt install postgresql # Installs PostgreSQL 
sudo su -c "createuser -s $USER" postgres # Creates db superuser
```

## 2- Corriendo servidor PostgreSQL
```linux
sudo service postgresql start
```


## 3 - Instalamos dependencias de Odoo
```linux
sudo apt update 
sudo apt upgrade 
sudo apt install git  # Install Git 
sudo apt install python3-dev python3-pip python3-wheel \ 
python3-venv # Python 3 for dev 
sudo apt install build-essential libpq-dev libxslt-dev \ 
libzip-dev libldap2-dev libsasl2-dev libssl-dev
```

## 4 - Installing Odoo from source
```linux
mkdir ~/work15  # Create a directory to work in
cd ~/work15  # Go into our work directory
git clone https://github.com/odoo/odoo.git -b 15.0 \ 
--depth=1  # Get Odoo sources
```
