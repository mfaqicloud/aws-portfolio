# EC2 Web Server with Apache

## Overview
This project demonstrates how to launch a cloud-based virtual server using AWS EC2, connect securely using SSH, and configure it to run a web server using Apache. It proves the ability to manage infrastructure directly in the cloud.

## What I Did
- Created a t2.micro EC2 instance running Amazon Linux 2023
- Configured a security group to allow inbound traffic on ports 22 (SSH) and 80 (HTTP)
- Connected to the instance using SSH via my Mac terminal
- Installed Apache using the `yum` package manager
- Verified the server was active and running with `systemctl`

## Commands Used

Here are some key commands I used during setup:

```
ssh -i "mohamud-key.pem" ec2-user@your-ec2-ip
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
hostname
uname -a
systemctl status httpd
```

## Skills Demonstrated
- EC2 provisioning and security group configuration
- SSH access with key-based authentication
- Apache installation and Linux service management
- Hands-on use of AWS services and terminal commands

## Screenshot

The image below shows proof of Apache successfully running inside my EC2 instance:

![EC2 Setup](./ec2-proof.png)

## Portfolio Link

Explore my other projects:  
👉 http://mohamud-portfolio.s3-website.us-east-2.amazonaws.com

## Live Demo

This project was deployed to an Amazon EC2 instance with Apache installed and configured.  
To save on AWS costs, the instance may not currently be running.
