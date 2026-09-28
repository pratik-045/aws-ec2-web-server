# AWS EC2 Web Server Deployment

##  Project Overview

This project demonstrates how I deployed a custom web server on an AWS EC2 instance using Amazon Linux and Nginx.

## AWS Services Used

- Amazon EC2
- Security Groups

## Technologies Used

- Amazon Linux
- Nginx
- Linux
- HTML

## Implementation Steps

1. Launched an Amazon EC2 instance.
2. Configured a Security Group.
3. Allowed SSH (Port 22) for remote access.
4. Allowed HTTP (Port 80) for web traffic.
5. Connected to EC2 using SSH.
6. Installed Nginx web server.
7. Started and enabled the Nginx service.
8. Created a custom HTML webpage.
9. Tested the website using the EC2 Public IPv4 address.

## Architecture

Internet  
↓  
AWS Security Group  
↓  
EC2 Instance  
↓  
Nginx Web Server  
↓  
Custom HTML Web Page

## Linux Commands Used

```bash
sudo dnf update -y
sudo dnf install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
sudo systemctl status nginx
cd /usr/share/nginx/html
sudo nano index.html
sudo systemctl restart nginx

## What I Learned

- Launching and configuring EC2 instances
- Working with AWS Security Groups
- Connecting to EC2 using SSH
- Installing and managing Nginx on Linux
- Hosting a custom webpage on an EC2 instance
- Understanding basic AWS web server deployment

## Project Screenshots

The following screenshots show the implementation and deployment of the AWS EC2 web server.

### 1. EC2 Instance
Shows the running EC2 instance used for the web server.

### 2. Security Group
Shows the inbound rules configured for SSH (Port 22) and HTTP (Port 80).

### 3. Nginx Web Server
Shows the Nginx service running successfully on the EC2 instance.

### 4. Custom Webpage
Shows the custom HTML webpage deployed on the EC2 instance and accessed through its public IP address.
