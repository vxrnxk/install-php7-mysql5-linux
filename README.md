# install-php7-mysql5-linux
Definitive guide made by Francisco V, to install PHP 7.x and MySQL 5.x on Linux distributions using APT package manager

## Install PHP
The official PHP website [php.net](https://www.php.net/)

```bash
sudo apt install -y software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt update
```

```bash
sudo apt install php7.4
```

```bash
sudo apt-get install php7.4-cli php7.4-fpm php7.4-bcmath php7.4-curl php7.4-gd php7.4-intl php7.4-json php7.4-mbstring php7.4-mysql php7.4-opcache php7.4-sqlite3 php7.4-xml php7.4-zip
```

```bash
php --version
```

## Install MySQL
The official MySQL website [mysql.com](https://www.mysql.com/)

```bash
sudo apt update
```

```bash
sudo apt install mysql-server
```

```bash
sudo mysql_secure_installation
```

```bash
sudo mysql -u root -p
```

```bash
select * from mysql.user;
```

```bash
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '<PASSWORD HERE>';
```

```bash
sudo service mysql restart
```

```bash
systemctl status mysql.service
```