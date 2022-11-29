# Project_2
# WEB STACK IMPLEMENTATION LEMP (LINUX, NGINX, MYSQL, PHP) STACK USING AWS AS CLOUD SERVICE PROVIDER
___
Installing Ubuntu OS on AWS EC2 VM. Instance sucessfully spined up and running 
<img width="960" alt="Screenshot 2022-11-29 131144" src="https://user-images.githubusercontent.com/57721371/204527581-410c375a-ff9c-4766-b84f-cc10b44b2814.png">
```
Instance ID: i-0f731e62bd0f63eed
```
___
### Updating Nginx Package Manager and Installing the Nginx Webserver
![Screenshot (244)](https://user-images.githubusercontent.com/57721371/204528909-708d38b0-fc08-4337-9516-1fb63bc3e428.png)
<img width="477" alt="Screenshot 2022-11-29 150230" src="https://user-images.githubusercontent.com/57721371/204549447-f01bf537-654e-4f28-973c-497b84f6f91e.png">
```
sudo apt update
sudo apt install nginx
curl http://3.86.250.109:80
```
___
### Mysql Databae Management System sucessfully installed and integrated to work with the php environment
<img width="452" alt="Screenshot 2022-11-29 150609" src="https://user-images.githubusercontent.com/57721371/204550343-c1993f4e-c472-49bf-826c-0bc8c8631e8f.png">

```
sudo apt install mysql-server
sudo mysql
```
___
###  Installing PHP: php-fpm and php-mysql (a PHP module that allows PHP to communicate with MySQL-based databases) are both installed at once.
like Apache, Nginx can be configured to host more than one domain on a single server (these are known as server blocks).
![Screenshot (250)](https://user-images.githubusercontent.com/57721371/204553274-477dced9-6b51-4e25-aa56-f59aa3f49ad2.png)
```
sudo apt install php-fpm php-mysql
```
___
### Configuring Nginx to use Php Processor
Configuration file tested to uncover syntax error; no errors found after concluding test

<img width="386" alt="Screenshot 2022-11-29 045025" src="https://user-images.githubusercontent.com/57721371/204557589-222fcb16-bf41-4281-ab2e-0dabf58077cf.png">

```
sudo nginx -t
```
___
### Nginx site is up and working as expected; accessed via Public IP Adress
<img width="960" alt="Screenshot 2022-11-29 045606" src="https://user-images.githubusercontent.com/57721371/204559718-c97c9ab7-46ba-48a4-8e03-701edab1c59d.png">

```
Public IP: http://3.86.250.109:80
```
___
### Creating a PHP script to test and ensure that Nginx is able to handle .php files within the newly configured website.
<img width="730" alt="Screenshot 2022-11-29 155043" src="https://user-images.githubusercontent.com/57721371/204561523-b5d2b054-103a-46ba-a63f-edc3c19deedd.png">

```
sudo nano /var/www/projectLEMP/info.php
```








