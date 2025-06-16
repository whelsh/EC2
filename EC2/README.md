
Installation and Running of Apache Web server on the AWS EC2 instance

Steps followed:
1) Creation of an AWS EC2 instance running on Ubuntu.
2) Connecting to the EC2 instance through the MobaXterm SSH terminal by use of private key.
3) Installation of Apache Web Server in the Ubuntu based EC2 instance using following commands:
	sudo apt update && sudo apt upgrade
	sudo apt install apache2 -y
4) Start the Apache web server by following commands:
	sudo systemctl enable apache2
5) Modify the contents of index.html with file path /var/www/html/index.html using sudo commands.
6) Modify the rules of the Security group such that its ports 22, 80 and 443 are open for all traffic.
7) By use of the public IP of the instance, the created web page by index.html can be accessed.
