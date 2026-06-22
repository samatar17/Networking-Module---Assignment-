# Networking-Module---Assignment-
My networking assigment showing how I created an EC2 server, Installed NGINX and connected my domain.

Networking-Module-Assignment
My project 
In this project, I learned how to create a simple web server in AWS using NGINX and connecting it to my domain.
| <img width="940" height="251" alt="image" src="https://github.com/user-attachments/assets/757ee1c7-1518-410c-b9bf-430cf544bf68" />

I used:
. AWS EC2 
. Ubuntu 
. NGINX
. Cloudflare DNS 

Step 1: Create EC2 Instance 
First I created an EC2 instance in AWS 
I used:
. Ubuntu 20.04
. t3.micro 
. Region: eu-north-1
This gave me a cloud server with a public IP address.
| <img width="940" height="193" alt="image" src="https://github.com/user-attachments/assets/1d559288-00df-4dd1-85c7-15cca6375eb9" />
 

Step 2: Connect to EC2 
I connected to my EC2 server using SSH 
This allowed me to access the Linux terminal 

Step 3: Install NGINX 
After connecting I installed NGINX
Commands used in terminal 
sudo apt update 
sudo apt install nginx -y

Then I started NGINX 
sudo systemctL start nginx 
I checked if it was running:
sudo systemctL status nginx 


Step 4: Open Security Group Ports
At first my website did not work 
I fixed it by adding inbound rules in AWS
I opened: 
. Port 22 (SSH)
. Port 80 (HTTP)
This allowed browser traffic to reach my server.


Step 5: Test NGINX 
I copied my EC2 public IP and opened it in the browser 
http://16.170.250.109
I saw the NGINX welcome page.
| <img width="896" height="266" alt="image" src="https://github.com/user-attachments/assets/ecb78cc7-ea3f-4552-ba4d-31333897922a" />

