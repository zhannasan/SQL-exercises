## SQL-exercises
### System
Ubuntu 20.04 LTS, mysql, phphMyAdmin
### Setting up
Update:<br>
```sudo apr update```
### Install mysql:
```sudo apt install mysql-server```<br>
Start:<br>
```sudo systemctl start mysql.service```<br>
Configure password for new installations:<br>
```sudo mysql_secure_installation```<br>
Create a user with a password:<br>
```sudo mysql```<br>
```mysql -u root -p```<br>
```CREATE USER 'username'@'host' IDENTIFIED WITH authentication_plugin BY 'password';```<br>
### Install phpMyAdmin
```sudo apt install phpmyadmin```<br>
Set user, password, and hostname (localhost or ip):<br>
```sudo dpkg -reconfigure phpmyadmin```<br>
Add phpmyadmin to apache2 config:<br>
```sudo nano /etc/apache2/apache2.conf```<br>
```Include /etc/phpmyadmin/apache.conf```<br>
Restart Apache:<br>
```/etc/init.d/apache2 restart```<br>
Access at http://localhost/phpmyadmin/ and start SQLing!