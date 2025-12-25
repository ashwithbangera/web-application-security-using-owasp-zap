# 🔐 Web Application Security - using OWASP ZAP & WebGoat

## 📌 Project Overview

This project demonstrates a **hands-on Web Application Security Assessment** performed on an intentionally vulnerable application using industry-recognized security tools. The objective of this project is to identify, analyze, and document common web application vulnerabilities such as **SQL Injection**, **Cross-Site Scripting (XSS)**, and **Cross-Site Request Forgery (CSRF)**.

The assessment was conducted in a controlled lab environment to simulate real-world web security testing practices.

---

## 🧰 Tools & Technologies Used

- **WebGoat** – An intentionally vulnerable web application developed by OWASP for security training.
- **OWASP ZAP (Zed Attack Proxy)** – An open-source web application security scanner.
- **Kali Linux** – Penetration testing operating system.
- **Docker** – Used to deploy WebGoat in a stable environment.
- **Firefox Browser**

---

## 🖥️ Environment Setup

- **Operating System:** Kali Linux
- **WebGoat Deployment:** Docker Container
- **WebGoat URL:** http://localhost:8080/WebGoat
- **OWASP ZAP Proxy Port:** 8081

---

## 🔍 Vulnerabilities Identified

### 1️⃣ SQL Injection (SQLi)

**Description:**  
SQL Injection occurs when user input is improperly handled and directly included in SQL queries.

**Observation:**  
- Abnormal input caused unexpected behavior.
- OWASP ZAP detected SQL Injection-related alerts.

**Impact:**  
- Authentication bypass  
- Unauthorized data access  
- Data manipulation  

---

### 2️⃣ Cross-Site Scripting (XSS)

**Description:**  
XSS allows attackers to inject malicious scripts into web pages that execute in a victim’s browser.

**Observation:**  
- OWASP ZAP detected a vulnerability labeled **“User-controllable HTML element attribute (XSS)”**.
- Indicates lack of proper input sanitization.

**Impact:**  
- Session hijacking  
- Cookie theft  
- Phishing attacks  

---

### 3️⃣ Cross-Site Request Forgery (CSRF)

**Description:**  
CSRF forces authenticated users to perform unintended actions without their consent.

**Observation:**  
- Forged requests were processed without anti-CSRF validation.
- Server responded with **405 Method Not Allowed**, indicating improper request handling.
- OWASP ZAP detected **Absence of Anti-CSRF Tokens**.

**Impact:**  
- Unauthorized account actions  
- Data modification  
- Privilege misuse  

---

## 📊 Reports & Evidence

- 📁 **Screenshots:** Stored in `/screenshots`
- 📄 **Detailed ZAP HTML Report:** Stored in `/zap-report`
- 📝 **Complete Task Report:** Stored in `/report`

---

## 🛡️ Mitigation Recommendations

- Use prepared statements and parameterized queries.
- Validate and encode all user inputs.
- Implement Anti-CSRF tokens and same-site cookies.
- Perform regular security assessments.
- Follow secure coding best practices.

---

## 🎯 Learning Outcomes

- Practical understanding of web application vulnerabilities.
- Hands-on experience with OWASP ZAP.
- Improved ability to identify and analyze security flaws.
- Exposure to real-world web security testing workflows.

---

## 📌 Conclusion

This project successfully demonstrates the identification and analysis of critical web application vulnerabilities using OWASP-recommended tools. It highlights the importance of secure coding practices and regular security testing in modern web applications.

---


