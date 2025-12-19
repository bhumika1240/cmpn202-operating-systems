
# Week 2 – Security Baseline and Performance Testing Methodology

## 1. Introduction
This week focuses on designing a security baseline and defining a performance testing methodology for the Ubuntu Server environment created in Week 1. The aim is to plan how the server will be monitored remotely, identify key security measures, and analyse potential security threats. This week focuses on planning only, with implementation scheduled for later weeks.

---

## 2. Performance Testing Plan and Remote Monitoring Methodology
Performance testing will be carried out remotely from the workstation to ensure that the server remains headless and securely administered. The workstation will connect to the server using SSH, and monitoring commands will be executed remotely.

The performance testing approach will include:
- Baseline testing when the server is idle
- Load testing when workloads are running
- Comparison of performance results to identify bottlenecks

The following performance metrics will be monitored:
- CPU usage
- Memory usage
- Disk input/output activity
- Network usage and latency

Standard Linux monitoring tools such as `top`, `htop`, `vmstat`, `iostat`, and `ping` will be used. The collected data will be used later to evaluate system performance and support optimisation decisions.

---

## 3. Security Configuration Checklist
The following security configuration checklist outlines the security measures planned for implementation in later weeks of the coursework.

### 3.1 SSH Hardening
- Disable direct root login via SSH
- Enable SSH key-based authentication
- Disable password-based authentication
- Restrict SSH access to the workstation IP address

### 3.2 Firewall Configuration
- Enable the system firewall
- Allow inbound traffic only on the SSH port
- Block all other incoming connections by default
- Restrict SSH access to trusted sources only

### 3.3 Mandatory Access Control
- Enable AppArmor on the server
- Ensure default AppArmor profiles are enforced
- Monitor AppArmor status and policy enforcement

### 3.4 Automatic Security Updates
- Enable automatic installation of security updates
- Ensure critical security patches are applied promptly
- Reduce the risk of vulnerabilities caused by outdated software

### 3.5 User Privilege Management
- Create a non-root administrative user
- Apply the principle of least privilege
- Avoid direct use of the root account
- Use privilege escalation only when required

### 3.6 Network Security
- Use an isolated VirtualBox host-only or internal network
- Prevent exposure to public or university networks
- Limit network access to the workstation only
- Reduce the server attack surface

---

## 4. Threat Model and Mitigation Strategies

### Threat 1: Unauthorised SSH Access
- **Risk:** Attackers may attempt to gain access to the server through brute-force or credential-based attacks.
- **Mitigation:** Use SSH key-based authentication, disable password login, restrict firewall access, and deploy fail2ban.

### Threat 2: Privilege Escalation
- **Risk:** A compromised user account could gain administrative privileges.
- **Mitigation:** Disable root login, enforce least-privilege access, and carefully manage user permissions.

### Threat 3: Network-Based Attacks
- **Risk:** The server could be targeted by network scanning or unauthorised connections.
- **Mitigation:** Isolate the server using VirtualBox networking and restrict open ports using firewall rules.

---

## 5. Reflection
This week established a clear plan for securing the server and testing its performance. By defining a performance testing methodology, creating a security configuration checklist, and identifying key threats with mitigation strategies, a strong foundation has been created for implementing security controls and performance evaluation in upcoming weeks.

