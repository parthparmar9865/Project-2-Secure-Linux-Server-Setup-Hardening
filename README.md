# Project-2-Secure-Linux-Server-Setup-Hardening
# Secure Kali Linux Server Setup & Hardening

## Project Overview
This project demonstrates how to deploy and secure a Kali Linux system using standard cybersecurity hardening techniques. The objective of this project is to protect the server from common threats such as unauthorized access, brute-force attacks, insecure configurations, and network vulnerabilities.

The project includes SSH hardening, firewall configuration, intrusion prevention using Fail2Ban, security auditing with Lynis, and vulnerability scanning using Nmap and Nikto.

---

## Objectives

- Deploy Kali Linux as a secure server environment
- Configure secure SSH access
- Implement firewall protection
- Prevent brute-force login attacks
- Perform vulnerability scanning
- Monitor system logs

---

## Tools & Technologies Used

| Tool | Purpose |
|-----|------|
| Kali Linux | Target system |
| OpenSSH | Secure remote access |
| UFW Firewall | Network security |
| Fail2Ban | Intrusion prevention |
| Lynis | Security auditing |
| Nmap | Network scanning |
| Nikto | Web vulnerability scanning |

---

## System Setup

### Step 1: Update Kali Linux

Update system packages to ensure all security patches are installed.

```bash
sudo apt update
sudo apt upgrade -y
VirtualBox / VMware

Minimum 2GB RAM

Internet connection





Step 2: Create a New User
sudo adduser secureuser
sudo usermod -aG sudo secureuser

This prevents direct use of the root account.

Step 3: Install SSH Server
sudo apt install openssh-server -y
