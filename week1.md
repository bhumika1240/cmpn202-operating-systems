# Week 1 – System Planning and Setup

## 1. Introduction
This week focuses on planning the system architecture, selecting a Linux server distribution, and setting up the initial virtual machine environment for the CMPN202 Operating Systems coursework. The aim is to deploy a secure, headless Linux server administered remotely.

---

## 2. System Architecture Overview
The coursework environment consists of two systems:

### Server
- Ubuntu Server 24.04 LTS running as a headless VirtualBox VM
- No graphical interface installed
- Used for security configuration and performance testing
- Managed remotely via SSH

### Workstation
- Host operating system
- Used to administer the server via terminal and SSH
- Used to collect evidence and manage GitHub Pages

---

## 3. Network Design
The server is connected using an isolated VirtualBox network to prevent external access.

- Network type: Host-Only / Internal Network
- Server IP address: `10.0.2.15`
- The server is not exposed to public or university networks

This design ensures a safe and ethical testing environment.

---

## 4. Linux Distribution Selection

### Chosen Distribution: Ubuntu Server 24.04 LTS
Ubuntu Server LTS was selected because:
- It provides long-term security updates
- It has strong community and documentation support
- It includes AppArmor for mandatory access control
- It is compatible with required tools such as Lynis and fail2ban

Alternative enterprise distributions were considered, but Ubuntu Server was chosen due to its ease of configuration and suitability for coursework.

---

## 5. Initial System Specification Checks
The following commands were executed on the server to verify system information:

```bash
uname -a
free -h
df -h
ip addr
lsb_release -a
