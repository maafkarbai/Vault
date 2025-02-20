![[PT-Process.webp]]

# Areas and Domains of Testing
-  Network Infrastructure
- Web Applications
- Mobile Applications
- Cloud Infrastructure
- Physical Security
- Wireless Security
- Software Security
#### OpenVAS Vulnerability Scanner

![OpenVAS.gif](https://academy.hackthebox.com/storage/modules/295/OpenVAS.gif)

---
## PEN Testing Structure
A penetration test follows a structured process to identify and document security vulnerabilities, providing actionable insights for remediation.
#### **1. Pre-Engagement Phase**
Defines scope, objectives, and legal agreements (NDAs, RoE). Establishes timelines and permitted activities.
#### **2. Information Gathering Phase**
- **Passive Reconnaissance:** OSINT, social media, and public records.
- **Active Reconnaissance:** Direct scanning (Nmap), service enumeration, and banner grabbing.

#### **3. Vulnerability Assessment Phase**
Identifies security weaknesses using automated and manual techniques, eliminating false positives.

#### **4. Exploitation Phase**
Attempts to exploit vulnerabilities to demonstrate real-world risks, following RoE guidelines.

#### **5. Post-Exploitation Phase**
Assesses potential impact via privilege escalation, lateral movement, and data exfiltration testing.

#### **6. Lateral Movement Phase**
Expands access within the network using credential attacks and trust exploitation.

#### **7. Proof of Concept**
Documents exploitation steps with scripts, logs, and evidence for validation.

#### **8. Post-Engagement Phase**
Delivers a detailed report with risk ratings, findings, and remediation recommendations.

#### **9. Remediation Support & Retesting**
Guides fixes and verifies their effectiveness to ensure improved security.

---
## Methodologies Important
- http://www.pentest-standard.org/index.php/Main_Page
- https://www.nist.gov/privacy-framework/nist-sp-800-115
- https://owasp.org/www-project-web-security-testing-guide/stable/
---

## Web App Testing
Learn About:
- Injection Vulnerabilities
- Authentication & Session Management
- Cross-Site Scripting
### Tools
- https://portswigger.net/burp/pro
- https://www.zaproxy.org/

---

## Common Network Security Vulnerabilities
| **Vulnerability**               | **Description**                                                                                                                |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `Misconfigured Services`        | Improperly configured network services, default credentials, and unnecessary open ports that could provide unauthorized access |
| `Unpatched Systems`             | Systems and applications running outdated software versions with known security vulnerabilities                                |
| `Weak Authentication`           | Poor password policies, lack of multi-factor authentication, and insecure password storage mechanisms                          |
| `Insecure Protocols`            | Use of deprecated or unencrypted protocols like FTP, Telnet, or HTTP instead of their secure alternatives                      |
| `Network Segmentation Issues`   | Inadequate network segregation allowing lateral movement between different security zones                                      |
| `Exposed Management Interfaces` | Administrative interfaces accessible from unauthorized networks or the internet                                                |
| `Missing Security Controls`     | Absence of essential security measures like firewalls, IDS/IPS systems, or proper access controls                              |

## Essential Tools and Technologies
- `Network Mapping Tools`: Tools like Nmap for network discovery and security auditing

- `Vulnerability Scanners`: Nessus, OpenVAS, and similar tools for identifying known vulnerabilities
    
- `Exploitation Frameworks`: Metasploit Framework for developing and executing exploit code
    
- `Packet Analysis Tools`: Wireshark for analyzing network traffic and identifying potential security issues
    
- `Password Cracking Tools`: John the Ripper and Hashcat for testing password security

___
### Cloud Pen testing
Learn About:
- Infrastructure as a Service (IaaS)
- Platform as a Service (PaaS)
- Software as a Service (SaaS)
Steps:
- `reconnaissance` and enumeration of cloud resources
- `access control` testing:
	- I`dentity and Access Management` (`IAM`) policies
- Look for `security misconfigurations`
- Review `virtual network configurations`
- evaluating the implementation of encryption, data loss prevention (`DLP`), and key management practices
- `application security`
### Tools to use
- CloudSploit, 
- Scout Suite,
- and Prowler are also available for automated assessments 
- For container security testing, 
	- Clair,
	- Trivy, 
	- Anchore are essential
-  API testing tools such as 
- Postman  
- Burp Suite 

---
### Mobile Testing
-  Mobile device management tools like Android Debug Bridge (ADB) for Android
- Reverse engineering tools such as JADX and Ghidra
- Network analysis tools like Burp Suite Mobile Assistant
- Mobile framework testing tools like Frida and Objection