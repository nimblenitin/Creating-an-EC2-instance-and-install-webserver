# Creating-an-EC2-instance-and-installing-webserver

Steps- 

```

1. Create an EC2 instance with below userdata-

#!/bin/bash 
# Use this for your user data (script without newlines) 
# install httpd (Linux 2 version) yum update -y yum install -y httpd.x86_64 systemctl start httpd.service systemctl enable httpd.service echo "Hello World from $(hostname -f)" > /var/www/html/index.html 


2. Open the public ip address to see the web server up and running.

```
