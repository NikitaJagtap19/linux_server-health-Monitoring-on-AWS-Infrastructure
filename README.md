# linux_server-health-Monitoring-on-AWS-Infrastructure
# AWS Linux Server Automation, Monitoring and Web Server Configuration

## Project Overview

This project demonstrates Linux server administration, automation, monitoring, and web server configuration on AWS Cloud using Amazon Linux EC2 instances. The project includes Apache web server setup, shell scripting automation, cronjob scheduling, IAM role configuration, CloudWatch monitoring, and SNS alert notifications.

The main objective of this project was to perform real-time Linux administration tasks and implement basic AWS infrastructure monitoring and automation.

---

# Technologies Used

- AWS EC2
- Amazon Linux
- Apache HTTP Server (httpd)
- Bash Shell Scripting
- Cronjob
- IAM Role
- Amazon CloudWatch
- Amazon SNS
- Linux System Administration
- SSH
- Security Groups

---

# Project Architecture

User → AWS EC2 Linux Server → Apache Web Server → CloudWatch Monitoring → SNS Email Alerts

---

# Project Implementation

1] Created and configured AWS EC2 Linux instance

2] Configured Security Group inbound rules for SSH, HTTP, and HTTPS access

3] Connected EC2 instance remotely using SSH and PEM key authentication

4] Updated DNF package manager and upgraded Linux system packages

5] Installed and configured Apache HTTP Server (httpd)

6] Started and enabled Apache service using systemctl commands

7] Hosted website on Apache web server

8] Created Bash shell scripts for Linux task automation

9] Configured Cronjobs for scheduled script execution

10] Attached IAM Role to EC2 instance for AWS service permissions

11] Configured CloudWatch CPU utilization alarm monitoring

12] Integrated Amazon SNS email notification service for alert management

13] Verified running services, ports, and server status using Linux administration commands

14] Performed troubleshooting for Apache services, cronjobs, and monitoring configurations

---

# Features

- Linux server administration on AWS cloud
- Apache web server configuration
- Shell scripting automation
- Scheduled task management using cronjobs
- CloudWatch infrastructure monitoring
- SNS email alert integration
- IAM role-based AWS permissions
- Linux service management and troubleshooting

---

# Linux Commands Used

```bash
sudo dnf update -y
sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
crontab -e
sudo systemctl status httpd
sudo ss -tulnp
