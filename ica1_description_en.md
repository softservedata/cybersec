# ICA1 (English Translation)

This document provides a detailed explanation of the Capture the Flag (CTF) challenge published on the VulnHub platform by the author 'onurturali'.

Difficulty: EASY  
Goal: Gain root access and retrieve flags.

---

## Scenario
ICA is working on a secret project. The goal is to obtain access credentials, gain system access, and escalate privileges.

---

## Steps Overview
1. Setup virtual machines
2. Discover target IP
3. Scan ports
4. Analyze web service
5. Download config file
6. Access MySQL
7. Extract credentials
8. Prepare wordlist
9. Analyze hashes
10. Crack passwords
11. Login via SSH
12. Explore users
13. Privilege escalation
14. Gain root shell

---

## Key Findings
- Open ports: 22 (SSH), 80 (HTTP), 3306 (MySQL)
- Exposed config file with DB credentials
- Weak password hashing (MD5 + Base64)
- Successful brute-force attack
- PATH hijacking vulnerability
- SUID misconfiguration

---

## Final Result
Root access obtained.

---

## Security Recommendations
- Use strong password hashing (bcrypt/Argon2)
- Restrict access to config files
- Disable unnecessary services
- Apply least privilege principle
- Monitor logs and detect anomalies

---

## Conclusion
A chain of vulnerabilities led to complete system compromise.
