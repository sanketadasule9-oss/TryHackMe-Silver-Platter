# TryHackMe - Silver Platter

![TryHackMe](https://img.shields.io/badge/TryHackMe-Silver%20Platter-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Category](https://img.shields.io/badge/Category-Cybersecurity-blue?style=for-the-badge)

## Overview

This repository documents my hands-on experience completing the **Silver Platter** room on TryHackMe.

The challenge involved network enumeration, web application analysis, authentication bypass, API investigation, credential discovery, SSH access, and Linux privilege escalation.

| Detail | Information |
|---|---|
| Platform | TryHackMe |
| Room | Silver Platter |
| Difficulty | Easy |
| Status | Completed |

**Room Link:** https://tryhackme.com/room/silverplatter

---

## Objectives

- Perform network scanning and service enumeration.
- Identify exposed services and web applications.
- Investigate Silverpeas authentication behavior.
- Analyze API endpoints and notification functionality.
- Discover credentials through application analysis.
- Obtain initial access through SSH.
- Explore Linux privilege escalation techniques.

## Tools Used

| Tool | Purpose |
|---|---|
| Nmap | Network scanning |
| cURL | HTTP requests and API enumeration |
| Web Browser | Web application analysis |
| SSH | Remote system access |
| Linux Commands | System enumeration and privilege escalation |

---

## Walkthrough

### 1. Network Enumeration

Started with Nmap to identify open ports and running services.

```bash
nmap -Pn -p- --open -T4 <TARGET_IP> -oN fullscan.txt
```

The scan identified the following services:

| Port | Service |
|---|---|
| 22 | SSH |
| 80 | HTTP |
| 8080 | Silverpeas Web Application |

### 2. Web Application Enumeration

Investigated the available web services and identified the Silverpeas application running on port 8080.

Performed manual analysis of the application and examined its authentication behavior.

### 3. Authentication Bypass

Identified an authentication-related weakness in the Silverpeas application.

Further investigation involved examining application requests and authentication parameters.

### 4. API Enumeration

Investigated the notification functionality and discovered the following API endpoint:

```text
/silverpeas/services/usernotifications/inbox
```

Analyzed notification-related responses to identify useful application information.

### 5. Initial Access

Application analysis revealed credentials associated with a system user.

Used the discovered credentials to establish SSH access.

**Note:** Actual credentials have intentionally been excluded.

### 6. Linux Privilege Escalation

After obtaining initial access:

- Enumerated the Linux environment.
- Investigated system logs and relevant information.
- Identified a privilege escalation path involving another user account.
- Escalated privileges to obtain root access.

**Note:** User and root flags have intentionally been excluded.

---

## Key Learnings

This room helped me gain practical experience in:

- Network scanning using Nmap.
- Web application enumeration.
- Authentication weakness analysis.
- API endpoint investigation.
- Credential discovery.
- SSH-based initial access.
- Linux privilege escalation.
- Systematic penetration testing methodology.

## Conclusion

Completing Silver Platter was a valuable hands-on learning experience.

My biggest takeaway was that careful enumeration and attention to small details can reveal security weaknesses that might otherwise go unnoticed.

I look forward to solving more TryHackMe challenges and continuously improving my practical cybersecurity skills.

---

## Disclaimer

This repository is intended for educational purposes and documents my learning experience in an authorized TryHackMe lab environment.

No real-world systems were targeted.

Sensitive credentials, private information, and challenge flags have intentionally been excluded.

---

## Connect

- **TryHackMe:** https://tryhackme.com/room/silverplatter
- **GitHub:** My cybersecurity learning journey

## 🏆 TryHackMe Achievement

Successfully completed the **Silver Platter** room on TryHackMe!

This achievement represents my hands-on practice in network enumeration, web application security, authentication bypass, and Linux privilege escalation.

🔗 **Explore the Room:** [TryHackMe - Silver Platter](https://tryhackme.com/room/silverplatter?utm_campaign=social_share&utm_medium=social&utm_content=room&utm_source=whatsapp&sharerId=6ac348dfa089c90c825b47a5)

