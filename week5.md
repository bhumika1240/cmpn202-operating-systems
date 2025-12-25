
# Week 5 – Advanced Security and Monitoring Infrastructure

## Overview
Week 5 focuses on implementing advanced security controls and monitoring
capabilities on the Ubuntu Server. This phase extends the system hardening
performed in Week 4 by introducing mandatory access controls, automated
security updates, intrusion prevention, security verification, and server
monitoring.

All configurations were implemented and verified using command-line tools.

---

## 1. Mandatory Access Control – AppArmor

AppArmor was used to enforce Mandatory Access Control (MAC) on the server.
It limits application capabilities using predefined security profiles.

### Verification
The following command was used to verify AppArmor status:

week5/images/week5/
![Image description](relative/path/to/image.png)

```bash
sudo aa-status
