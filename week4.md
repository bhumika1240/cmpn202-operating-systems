# Week 4 – Foundational Security Implementation
# Week 4 – System Hardening and Security Configuration

## Overview
This week focused on implementing essential security configurations on the Ubuntu Server. The aim was to establish a secure baseline by enabling secure remote access, applying firewall rules, configuring automatic updates, and verifying mandatory access control mechanisms.

---

## 1. System Update and Patch Management
The system was updated to ensure all installed packages and security patches were applied before further configuration.

![System Update](images/week4/system-update.png)

---

## 2. Secure Shell (SSH) Configuration
Secure Shell (SSH) was enabled and verified to be running correctly to allow secure remote administration of the server.

![SSH Status](images/week4/ssh-status.png)

---

## 3. Firewall Configuration (UFW)
The Uncomplicated Firewall (UFW) was enabled to restrict inbound network traffic. SSH access was explicitly allowed while all other unsolicited connections are blocked by default.

![UFW Status](images/week4/ufw-status.png)

---

## 4. Automatic Security Updates
Automatic security updates were verified using the unattended-upgrades service to ensure that critical patches are installed without manual intervention.

![Unattended Upgrades](images/week4/unattended-upgrades.png)

---

## 5. Mandatory Access Control – AppArmor
AppArmor was confirmed to be active and enforcing security profiles, providing mandatory access control for system services.

![AppArmor Status](images/week4/apparmor-status.png)

---

## Conclusion
Week 4 successfully established a secure baseline for the Ubuntu Server. Core security controls including system updates, secure remote access, firewall protection, automatic updates, and mandatory access control were implemented and verified. This configuration provides a strong foundation for monitoring and performance testing in later weeks.
