# 🧠 FUTURE_CS_01 – Web Application Security Testing

### 👨‍💻 Author: Nagesh Patchipala  
### 📅 Date of Testing: November 3, 2025  
### 📄 Internship Domain: Cyber Security (Future Interns)

---

## 🧾 Overview
This project is part of my **Cyber Security Internship** with **Future Interns**.  
The goal of this task was to conduct a **Web Application Security Assessment** on the **OWASP Juice Shop**, an intentionally vulnerable application used for learning and practicing ethical hacking techniques.

The assessment aimed to identify and analyze vulnerabilities such as:
- SQL Injection (SQLi)
- Cross-Site Scripting (XSS)
- Security Misconfigurations
- Authentication & Header Weaknesses

---

## 🧰 Tools Used
- **OWASP ZAP** – Automated web vulnerability scanner  
- **Burp Suite** – Manual interception and testing  
- **Kali Linux** – Security testing platform  
- **OWASP Juice Shop** – Vulnerable web app target  

---

## ⚙️ Methodology
1. **Setup & Environment Preparation**
   - Deployed OWASP Juice Shop locally
   - Configured OWASP ZAP proxy and captured traffic
2. **Reconnaissance**
   - Identified endpoints, login forms, and hidden resources
3. **Vulnerability Scanning**
   - Performed active and passive scans in OWASP ZAP
4. **Manual Verification**
   - Tested SQLi and XSS vulnerabilities manually
5. **Reporting**
   - Documented findings, mapped to OWASP Top 10, and proposed mitigations

---

## 🧩 Key Findings
| Vulnerability | Risk Level | OWASP Mapping |
|----------------|-------------|----------------|
| Missing CSP Header | Medium | A05:2021 – Security Misconfiguration |
| Missing HSTS Header | Medium | A05:2021 – Security Misconfiguration |
| Hidden File Accessible (_darcs) | Medium | A05:2021 – Security Misconfiguration |
| SQL Injection (Login Page) | High | A03:2021 – Injection |
| Cache-Control Header Missing | Low | A05:2021 – Security Misconfiguration |

---

## 📷 Screenshots
- Screenshot 1: SQL Injection test result  
- Screenshot 2: XSS alert demonstration  
- Screenshot 3: ZAP vulnerability scan output  


## 🧱 Mitigation Recommendations
- Implement **parameterized queries**
- Enforce **Content Security Policy (CSP)** headers
- Enable **HTTPS (HSTS) enforcement**
- Regularly update web components and sanitize inputs



