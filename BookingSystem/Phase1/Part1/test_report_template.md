# 1️⃣ Introduction

**Tester(s):**  
- Name:  Vertti Ruotsalainen

**Purpose:**  
- We do fungtionality and security test for registration page

**Scope:**  
- Tested components:  Registeration page
- Exclusions:  
- Test approach: White-hat hacker, using a gray-box testing approach

**Test environment & dates:**  
- Start:  23.11
- End:  23.11
- Test environment details (OS, runtime, DB, browsers): Using Desktop Docker and PowerShell

**Assumptions & constraints:**  
- e.g., credentials provided, limited time, etc.

---

# 2️⃣ Executive Summary

**Short summary (1-2 sentences):**  

**Overall risk level:** (Low / Medium / High / Critical)

**Top 5 immediate actions:**  
1.  Path Travelsar)(Critical -- Assume all input is malicious. Use an "accept known good" input validation strategy, i.e., use an allow list of acceptable inputs that strictly conform to specifications.
2.  SQL injection(Critical) -- Do not trust client side input, even if there is client side validation in place.
In general, type check all data on the server side.
3.  
4.  
5.  

---

# 3️⃣ Severity scale & definitions

|  **Severity Level**  | **Description**                                                                                                              | **Recommended Action**           |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
|      🔴 **High**     | A serious vulnerability that can lead to full system compromise or data breach (e.g., SQL Injection, Remote Code Execution). | *Immediate fix required*         |
|     🟠 **Medium**    | A significant issue that may require specific conditions or user interaction (e.g., XSS, CSRF).                              | *Fix ASAP*                       |
|      🟡 **Low**      | A minor issue or configuration weakness (e.g., server version disclosure).                                                   | *Fix soon*                       |
| 🔵 **Info** | No direct risk, but useful for system hardening (e.g., missing security headers).                                            | *Monitor and fix in maintenance* |


---

# 4️⃣ Findings 

>

| ID | Severity | Finding | Description | Evidence / Proof |
|------|-----------|----------|--------------|------------------|
| F-01 | 🔴 High | Path Traversal | attack technique allows an attacker access to files, directories, and commands that potentially reside outside the web document root directory | <img width="1156" height="145" alt="kuva" src="https://github.com/user-attachments/assets/3eaf651f-36ad-4f00-bf66-ceac4e124960" /> |
| F-02 | 🔴 High | SQL injection | The page results were successfully manipulated using the boolean conditions | <img width="1216" height="137" alt="kuva" src="https://github.com/user-attachments/assets/95960b38-eaad-4571-af66-85a447ac6a9c" /> |
| F-03 | 🟠 Medium | Absence of Anti-CSRF Tokens | No Anti-CSRF tokens were found in a HTML submission form. | <img width="1150" height="177" alt="kuva" src="https://github.com/user-attachments/assets/21b0eb3d-0f68-47d0-abff-e24dab9a5b9f" /> |
| F-04 | 🟠 Medium | Missing Anti-clickjacking Header | The response does not protect against 'ClickJacking' attacks | <img width="342" height="142" alt="kuva" src="https://github.com/user-attachments/assets/59c18b6a-abcc-45e2-9cea-6021149881bd" /> |
| F-05 | 🟡 Low | Application error disclosure | error/warning message that may disclose sensitive information like the location of the file that produced the unhandled exception | <img width="490" height="142" alt="kuva" src="https://github.com/user-attachments/assets/3d7d43dc-0ed4-4700-a6ea-bd624a900bd9" /> |




---



---

# 5️⃣ OWASP ZAP Test Report (Attachment)


https://github.com/Vertti-Ruotsalainen/CybersecurityAndDataPrivacy2025/blob/main/BookingSystem/2025-11-23-ZAP-Report-part1.md

---


---
