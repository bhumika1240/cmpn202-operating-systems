## Week 4 – System Security and Hardening

---
In Week 4, the Ubuntu Server was hardened by applying essential security configurations. The focus of this week was to secure remote access, enable firewall protection, configure automatic updates, and enforce mandatory access control using AppArmor. These steps help reduce attack surfaces and improve the overall security posture of the server.

---


### 1. System Update

The system was updated to ensure all installed packages and the kernel were up to date. Keeping the system patched is critical to protect against known vulnerabilities.

![System Update](images/week1/week4-system-update.png)

- Updated package lists
- Installed available security updates
- Verified system services after updates

This confirms the server is running with the latest security patches.

---

### 2. SSH Service Status

The SSH service was enabled and verified to be running correctly.

![SSH Status](images/week1/week4-ssh-status.png)

---

### 3. Firewall (UFW) Status

The Uncomplicated Firewall (UFW) was enabled and configured to allow SSH connections.

![UFW Status](images/week1/week4-ufw-status.png)

---

### 4. Unattended Upgrades

Automatic security updates were enabled using unattended-upgrades.

![Unattended Upgrades](images/week1/week4-unattended-upgrades.png)

---

### 5. AppArmor Status

AppArmor was verified to be active and enforcing security profiles.

![AppArmor Status](images/week1/week4-apparmor-status.png)

---

## Summary

In Week 4, basic system hardening was performed by updating the system, securing SSH access, enabling a firewall, configuring automatic updates, and verifying AppArmor enforcement.
