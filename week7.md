
# Week 7 – Security Audit and System Evaluation

## 1. Introduction
The objective of this week’s practical work is to conduct a comprehensive security audit and system evaluation of the Linux server configured during previous coursework weeks. The focus of this assessment is to evaluate the system’s security posture by analysing firewall configuration, SSH hardening, access control mechanisms, exposed network services, and residual security risks.
Both automated and manual security assessment techniques were considered. Any limitations encountered during testing were documented and addressed through alternative verification methods to ensure a complete and reliable security evaluation.

---

## 2. Security Audit Methodology
The security evaluation followed a structured and systematic methodology:

1. Attempt automated security auditing using Lynis  
2. Verify firewall configuration and network exposure  
3. Validate SSH authentication and access control policies  
4. Confirm mandatory access control enforcement  
5. Audit running services and justify necessity  
6. Analyse residual risks and security trade-offs  

This methodology aligns with real-world security auditing practices and ensures comprehensive coverage of key security areas.

---

## 3. Automated Security Audit Attempt (Lynis)

### 3.1 Lynis Installation Attempt
The Lynis security auditing tool was selected to perform an automated system-wide security assessment.

```bash
sudo apt install lynis -y
