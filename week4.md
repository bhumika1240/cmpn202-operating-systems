## Week 4 – System Security and Hardening

In Week 4, the Ubuntu Server was hardened by applying essential security configurations. The focus of this week was to secure remote access, enable firewall protection, configure automatic updates, and enforce mandatory access control using AppArmor. These steps help reduce the attack surface and improve the overall security posture of the server.

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

SSH was enabled to allow secure remote administration of the server. The SSH service was verified to be running correctly.

![SSH Status](images/week1/week4-ssh-status.png)

**Security measures applied:**
- SSH service enabled and started
- Secure remote access configured using recommended settings

These measures help reduce the risk of unauthorised access and brute-force attacks.

---

### 3. Firewall (UFW) Status

The Uncomplicated Firewall (UFW) was configured to control incoming network traffic.

![UFW Status](images/week1/week4-ufw-status.png)

**Firewall rules applied:**
- Firewall enabled at startup
- SSH traffic (port 22) explicitly allowed
- All other unsolicited incoming connections blocked by default

This ensures only required services are accessible from the network.

---

### 4. Unattended Upgrades

Automatic updates were configured using the unattended-upgrades service to ensure critical security patches are applied without manual intervention.

![Unattended Upgrades](images/week1/week4-unattended-upgrades.png)

**Verification results:**
- Unattended upgrades service is enabled
- Service is actively running in the background

This helps maintain system security over time by automatically applying updates.

---

### 5. AppArmor Status

AppArmor was verified and confirmed to be active on the system. AppArmor enforces security policies that restrict what applications can access.

![AppArmor Status](images/week1/week4-apparmor-status.png)

**AppArmor status results:**
- AppArmor profiles are loaded
- At least one process is running in enforce mode
- No profiles are in complain or kill mode

This confirms that mandatory access control is functioning correctly and enforcing security rules.

---

## Conclusion

This week successfully implemented essential system hardening measures on the Ubuntu Server. SSH access was secured, firewall rules were applied, automatic updates were enabled, and AppArmor was confirmed to be enforcing security policies. These configurations significantly improve the security and stability of the server and provide a strong foundation for future performance monitoring and testing.
