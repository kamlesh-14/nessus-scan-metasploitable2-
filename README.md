# Nessus Vulnerability Scan – Metasploitable 2

This repository documents a vulnerability assessment project where I used **Tenable Nessus Essentials** to scan a vulnerable machine (**Metasploitable 2**).

The goal was to simulate a real-world vulnerability assessment, identify and prioritize security issues, and document remediation strategies.

---

## Project Workflow

1. **Configured Nessus on Kali Linux**
2. **Scanned Metasploitable 2 in a lab environment**
3. **Exported the report in PDF format**
4. **Reviewed vulnerabilities and severity**
5. **Researched fixes/mitigations for major issues**
6. **Documented the most critical vulnerabilities**
7. **Took screenshots for future reference**

---

## 🧾 Scan Report

- [📄 Download Full PDF Report](scan-report/nessus_scan_report.pdf)

---

##  Top Critical Vulnerabilities Found

| # | Vulnerability | Severity | Notes |
|--|---------------|----------|-------|
| 1 | SMB Null Sessions | Critical | Allows unauthenticated enumeration |
| 2 | Anonymous FTP Login | High | Open FTP server with full read access |
| 3 | Outdated Services (Apache, Samba, MySQL) | High | Vulnerable versions with public exploits |
| 4 | MySQL Weak Auth | Medium | Weak username/password access |

Details for each are available in: [`doc/critical-vulnerabilities.md`](doc/critical-vulnerabilities.md)

---

## ✅ Fixes & Mitigations

Remediation guidance has been provided for critical issues:

- [`fixes/smb_null_sessions.md`](fixes/smb_null_sessions.md)
- [`fixes/ftp_anonymous_login.md`](fixes/ftp_anonymous_login.md)
- [`fixes/outdated_services.md`](fixes/outdated_services.md)
- [`fixes/mysql_weak_auth.md`](fixes/mysql_weak_auth.md)

---

## 📷 Screenshots

Visual reference of important parts of the scan:

- Summary view of vulnerabilities
- Specific vulnerability evidence
- Risk categorization by CVSS
- Individual plugin results

<img src="scan-report/screenshots/summary.png" width="600"/>

More in the `scan-report/screenshots/` folder.

---

##  Lab Setup

- **Scanner**: Kali Linux (with Nessus Essentials)
- **Target**: Metasploitable 2 (Host-only or NAT network)
- **Scan Policy**: Basic Network Scan
- **Report Format**: PDF + Screenshots

---

## 🎯 Goal of This Project

This repo serves as a reference for:
- Beginners learning network vulnerability assessments
- Building practical experience using **Nessus**
- Understanding the process of analyzing and mitigating vulnerabilities

---

## 💬 Feedback & Contributions

Suggestions and pull requests are welcome if you’d like to improve or expand this documentation!

---
