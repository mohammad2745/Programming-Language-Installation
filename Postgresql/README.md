## Install MySQL and phpMyAdmin process

### Install MySQL

```sh
sudo apt update
```

```sh
sudo apt install mysql-server
```

<p>Open mySQL on terminal</p>

```sh
sudo mysql
```

<p>Change Password</p>

```sh
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
```

<p>For more secure installation. (Need to exit from mysql by typing exit)</p>

```sh
mysql_secure_installation
```

<p>Open mySQL on terminal - After Secure Installation</p>

```sh
mysql -u root -p
```

<p>Create a new user</p>

```sh
CREATE USER 'username'@'host' IDENTIFIED WITH authentication_plugin BY 'password';
```

<p>Start mySQL</p>

```sh
sudo systemctl start mysql
```

<p> mySQL Status</p>

```sh
systemctl status mysql.service
```

<p>Stop mySQL</p>

```sh
sudo systemctl stop mysql.service
```

<p>Check mySQL version</p>

```sh
mysql --version
```

### Install phpMyAdmin

<p>Check mySQL version</p>

```sh
sudo apt install phpmyadmin php-mbstring php-zip php-gd php-json php-curl
```
