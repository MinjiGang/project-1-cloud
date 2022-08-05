# Using AWS EC2 and RDS to Launch a Simple Data Table
First what you need to do is either launch a default VPC or make one for example a VPC with a CIDR of 10.10.0.0/24 and be sure to make subnets at least 4 of them so that we can have 2 subnets with Public and 2 subnets with Private and be sure to connect the Public Subnets with IGW or Internet Gateway and NAT Gateway for Private Subnets.
Second We launch our Public EC2 Instance and be sure to install the following requirements:
- Php7.4
- Apache Web Server (HTTPD)
- AWS CLI V2
- MySQL
Third After Installing the following requirements we can download the following files from this repository the aws.zip and the inventory.zip.
be sure to unzip the aws.zip and inventory.zip in the Document Root of Apache (/var/www/html)
Check if the Website is running normally. If it's running normally we can move to our next step which is launching RDS
Launch a Normal RDS Database and after creating, add the RDS Endpoint link to the website.
Then we can just make a simple inventory Database Table.
