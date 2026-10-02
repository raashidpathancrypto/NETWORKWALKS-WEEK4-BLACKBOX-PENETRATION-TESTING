# NETWORKWALKS-WEEK4-BLACKBOX-PENETRATION-TESTING
# 🔐 Week 4 – Black-Box Penetration Testing Capstone

## 🏥 Mediroza General Hospital – Simulated Environment

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-red)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-v2026.2-blue)
![VAPT](https://img.shields.io/badge/VAPT-red)
![Penetration Testing](https://img.shields.io/badge/Penetration%20Testing-black)
![Ethical Hacking](https://img.shields.io/badge/Ethical%20Hacking-orange)
![SQL Injection](https://img.shields.io/badge/SQL%20Injection-critical)
![Hashcat](https://img.shields.io/badge/Hashcat-blue)
![John the Ripper](https://img.shields.io/badge/John%20the%20Ripper-red)

---

## 📌 Overview

This repository documents **Week 4 of my Cybersecurity Internship at NETWORKWALKS**.

The final week focused on a **Black-Box Penetration Testing Capstone Project** against a simulated hospital environment named **Mediroza General Hospital**.

The assessment combined the knowledge and techniques developed throughout the previous weeks, including:

* Reconnaissance
* Enumeration
* Attack Surface Mapping
* Web Application Security Testing
* Vulnerability Identification
* SQL Injection Testing
* Authentication Testing
* Password & Hash Security
* Risk Assessment
* Penetration Testing Reporting

> ⚠️ **Important:** Mediroza General Hospital is a simulated training environment. All testing was performed in an authorized cybersecurity lab for educational purposes.

---

# 🎯 Objectives

The main objectives of this assessment were to:

* Identify the target's attack surface
* Discover exposed resources and directories
* Identify security misconfigurations
* Test web application security
* Identify and validate SQL Injection
* Assess authentication controls
* Analyze password/hash security
* Determine potential security impact
* Document findings professionally
* Provide practical remediation recommendations

---

# 🔎 Penetration Testing Methodology

The assessment followed a structured penetration-testing workflow:

```text
Reconnaissance
      ↓
Attack Surface Mapping
      ↓
Enumeration
      ↓
Vulnerability Identification
      ↓
Vulnerability Validation
      ↓
Impact Analysis
      ↓
Risk Assessment
      ↓
Remediation
      ↓
Professional Reporting
```

---

# 1️⃣ Reconnaissance & Enumeration

The first phase focused on understanding the target environment and identifying accessible resources.

### Activities Performed

* Attack surface mapping
* Directory enumeration
* Resource discovery
* Information disclosure testing
* `robots.txt` analysis

### Finding

A `robots.txt` file was identified that disclosed paths which required further investigation.

### Security Lesson

`robots.txt` should not be treated as an access-control mechanism. Sensitive resources should be protected using proper authentication and authorization controls.

---

# 2️⃣ Exposed Directory & Backup

During enumeration, an **unprotected directory** was identified.

The directory exposed a simulated database backup containing sensitive-looking records as part of the training scenario.

### Potential Impact

An exposed database backup could potentially lead to:

* Sensitive information disclosure
* Privacy violations
* Credential exposure
* Data leakage
* Further attack opportunities

### Recommended Remediation

* Remove unnecessary backups from web-accessible directories
* Store backups outside the web root
* Implement authentication and authorization
* Encrypt sensitive backup files
* Apply appropriate file permissions
* Perform regular security reviews

---

# 3️⃣ SQL Injection

A **SQL Injection vulnerability** was identified in the simulated patient portal.

The vulnerability was validated within the authorized lab environment and demonstrated the potential for **authentication bypass**.

### Potential Impact

SQL Injection can potentially result in:

* Authentication bypass
* Unauthorized database access
* Sensitive information disclosure
* Database manipulation
* Further compromise depending on database privileges

### Recommended Remediation

* Use parameterized queries
* Implement prepared statements
* Perform server-side input validation
* Apply least-privilege database permissions
* Avoid dynamically constructed SQL queries
* Implement secure error handling
* Conduct regular application security testing

---

# 4️⃣ Password & Hash Security

The capstone scenario included simulated encrypted/password-protected patient reports.

Password/hash security testing was performed using:

![Hashcat](https://img.shields.io/badge/Hashcat-blue)
![RockYou](https://img.shields.io/badge/RockYou-Wordlist-purple)
![Password Security](https://img.shields.io/badge/Password%20Security-red)
![Hash Analysis](https://img.shields.io/badge/Hash%20Analysis-purple)

### Tools Used

* Hashcat
* RockYou wordlist
* NetworkWalks Password Cracker
* John the Ripper
* Johnny

### Key Learning

The exercise demonstrated the importance of:

* Strong password policies
* Long and unique passwords
* Secure password hashing
* Salted password storage
* Multi-factor authentication
* Protection against password guessing attacks

---

# 🛠️ Tools & Technologies

## Operating System

![Kali Linux](https://img.shields.io/badge/Kali%20Linux-v2026.2-blue)

## Penetration Testing

![VAPT](https://img.shields.io/badge/VAPT-red)
![Ethical Hacking](https://img.shields.io/badge/Ethical%20Hacking-orange)
![Penetration Testing](https://img.shields.io/badge/Penetration%20Testing-black)

## Password & Hash Analysis

![Hashcat](https://img.shields.io/badge/Hashcat-blue)
![John the Ripper](https://img.shields.io/badge/John%20the%20Ripper-red)
![Johnny](https://img.shields.io/badge/Johnny-orange)
![Hashing](https://img.shields.io/badge/Hashing-purple)
![Password Recovery](https://img.shields.io/badge/Password%20Recovery-darkred)

## Security Concepts

![SQL Injection](https://img.shields.io/badge/SQL%20Injection-critical)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-red)
![NetworkWalks](https://img.shields.io/badge/NetworkWalks-black)

---

# 📊 Key Findings

| # | Finding                                     | Category                 | Potential Impact                    |
| - | ------------------------------------------- | ------------------------ | ----------------------------------- |
| 1 | Information Disclosure through `robots.txt` | Reconnaissance           | Attack Surface Discovery            |
| 2 | Unprotected Backup Directory                | Information Disclosure   | Sensitive Data Exposure             |
| 3 | SQL Injection                               | Web Application Security | Authentication Bypass / Data Access |
| 4 | Weak Password Security                      | Authentication Security  | Unauthorized Access                 |

> **Note:** Risk ratings and evidence should be documented in the full penetration-testing report included with the project.

---

# 📄 Professional Penetration Testing Report

The final assessment was documented in a structured penetration-testing report containing:

* Executive Summary
* Scope
* Methodology
* Technical Findings
* Evidence
* Risk Ratings
* Potential Impact
* Remediation Recommendations
* Conclusion

### Report Structure

```text
Executive Summary
       ↓
Scope & Methodology
       ↓
Reconnaissance
       ↓
Technical Findings
       ↓
Evidence
       ↓
Risk Assessment
       ↓
Remediation
       ↓
Conclusion
```

---

# 💡 Key Takeaway

One of the biggest lessons from this capstone was that serious security impact can result from **multiple smaller weaknesses being chained together**.

```text
Information Disclosure
        +
Exposed Backup
        +
SQL Injection
        +
Weak Password
        ↓
Significant Security Impact
```

A penetration tester therefore needs to look beyond individual vulnerabilities and understand how weaknesses can interact within an attack path.

---

# 🎓 Skills Demonstrated

### Technical Skills

* Reconnaissance
* Enumeration
* Attack Surface Mapping
* Web Application Security
* SQL Injection Testing
* Authentication Testing
* Password Security
* Hash Analysis
* Vulnerability Assessment
* Penetration Testing
* Risk Analysis
* Security Reporting

### Professional Skills

* Technical Documentation
* Finding Analysis
* Risk Communication
* Remediation Planning
* Penetration Testing Reporting

---

# 📁 Repository Structure

```text
NETWORKWALKS-WEEK4-BLACKBOX-PENETRATION-TESTING/
│
├── README.md
│
├── Reconnaissance/
│   ├── reconnaissance-notes.md
│   └── screenshots/
│
├── Enumeration/
│   ├── enumeration-notes.md
│   └── screenshots/
│
├── Web-Application-Testing/
│   ├── sql-injection.md
│   ├── authentication-testing.md
│   └── screenshots/
│
├── Password-Security/
│   ├── hash-analysis.md
│   └── screenshots/
│
├── Reports/
│   └── penetration-testing-report.pdf
│
└── Evidence/
    └── redacted-screenshots/
```

---

# ⚠️ Responsible Disclosure & Lab Safety

All activities documented in this repository were performed in an **authorized simulated training environment**.

No unauthorized systems were targeted.

No real patient information, credentials, passwords, database backups, or sensitive organizational information is included in this repository.

Sensitive evidence should be **redacted before publication**.

---

# 🙏 Acknowledgement

I would like to thank **Waqas Karim (CCIE)** and the entire **NETWORKWALKS team** for providing a practical and hands-on cybersecurity learning experience throughout this internship.

---

## 🚀 Internship Journey

### Week 1

🔹 Cybersecurity Lab Environment Setup

### Week 2

🔹 Reconnaissance & Footprinting

### Week 3

🔹 Network Discovery & Security Analysis

### Week 4

🔹 Black-Box Penetration Testing Capstone

---

A big thank you to Waqas Karim (CCIE) and the entire NETWORKWALKS team for their guidance and support throughout this learning journey.

👩‍💻 Author Raashid Fazal Pathan

⭐ This repository documents my practical learning journey during my cybersecurity internship.

### ⭐ If you found this project useful

Feel free to explore the repository and follow my cybersecurity learning journey.

**#CyberSecurity #VAPT #PenetrationTesting #EthicalHacking #WebSecurity #KaliLinux #Hashcat #SQLInjection #CyberSecurityInternship #NetworkWalks**
