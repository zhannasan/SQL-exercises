## SQL-exercises
### System
Ubuntu 20.04 LTS, mysql, phphMyAdmin
### Setting up
Update:
```sudo apr update```
### Install mysql:
```sudo apt install mysql-server```
Start 
```sudo systemctl start mysql.service```
Configure password for new installations:
```sudo mysql_secure_installation```
Create a user with a password
```sudo mysql```
```mysql -u root -p```
```CREATE USER 'username'@'host' IDENTIFIED WITH authentication_plugin BY 'password';```
### Install phpMyAdmin
```sudo apt install phpmyadmin```
Set user, password, and hostname (localhost or ip):
```sudo dpkg -reconfigure phpmyadmin```
Add phpmyadmin to apache2 config:
```sudo nano /etc/apache2/apache2.conf```
```Include /etc/phpmyadmin/apache.conf```
Restart Apache:
```/etc/init.d/apache2 restart```
Access at http://localhost/phpmyadmin/ and start SQLing!