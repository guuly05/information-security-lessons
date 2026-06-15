# Fundamentals of Information Systems Security

## A Comprehensive Course in Information Assurance

Welcome to the **Fundamentals of Information Systems Security** course repository. This resource provides a complete, structured curriculum covering the essential principles, practices, and technologies required to protect modern information systems.

Whether you are a student pursuing a career in cybersecurity, an IT professional seeking to formalize your knowledge, or a self-directed learner, this course will equip you with the foundational understanding needed to identify risks, implement controls, and manage security operations within an organization.

---

## Course Description

This course provides a comprehensive introduction to the principles and practices of information systems security. It covers organization-wide policies, their documentation, and legal and business requirements. Students will explore security policy formats—including global, topic-specific, and application-specific policies—followed by asset classification, access control models, physical security components, and the foundations of risk analysis and management.

### Course Objectives

Upon completion, students will understand the key issues associated with:

- Protecting information assets
- Determining appropriate levels of protection
- Responding to security incidents
- Designing consistent, reasonable information security systems
- Implementing intrusion detection and reporting features

---

## Prerequisites

Before beginning this course, students should have:

- Basic computer science knowledge
- Understanding of operating systems and networks
- Familiarity with programming fundamentals
- Introductory knowledge of databases

---

## Required Textbook

| **Title**   | Fundamentals of Information Systems Security                                              |
| ----------- | ----------------------------------------------------------------------------------------- |
| **Edition** | Fourth Edition                                                                            |
| **Authors** | David Kim & Michael G. Solomon                                                            |
| **Focus**   | Information assurance, risk management, access control, cryptography, security operations |

### About the Authors

**David Kim** is a recognized information security expert, author, and educator with extensive experience in cybersecurity, IT auditing, and risk management. He has held senior security roles across government and private sectors and has been instrumental in developing security curricula for academic institutions.

**Michael G. Solomon** is a cybersecurity author, speaker, and professor with decades of experience in IT security, blockchain, and digital forensics. He has written numerous books on security, governance, and emerging technologies, and serves as a subject matter expert for multiple certification programs including CISSP and CEH.

Together, Kim and Solomon bring practical, real-world security expertise grounded in both technical depth and managerial perspective.

---

## Course Outline & Lesson Plan

The course is structured into **9 core chapters**, each designed to be completed in approximately **one week** of dedicated study (3–5 hours per chapter).

| Chapter | Title                                    | Key Topics                                                                    |
| :-----: | :--------------------------------------- | :---------------------------------------------------------------------------- |
|    1    | Introduction to Information Security     | CIA Triad, IT domains, security governance, human factors                     |
|    2    | Emerging Technologies & Their Impact     | IoT, AI, 3D printing, cloud, security/privacy challenges                      |
|    3    | Risks, Threats, and Vulnerabilities      | Risk management lifecycle, threat modeling, attack vectors                    |
|    4    | Business Drivers of Information Security | BIA, BCP, DRP, compliance laws, gap analysis, BYOD                            |
|    5    | Access Controls                          | Identification, authentication, authorization, accountability, RBAC, MAC, DAC |
|    6    | Cryptography                             | Symmetric/asymmetric encryption, hashing, PKI, digital signatures             |
|    7    | Malicious Software & Attack Vectors      | Viruses, worms, Trojans, ransomware, botnets, social engineering              |
|    8    | Security Operations & Administration     | Policies, standards, baselines, change management, SDLC security              |
|    9    | Auditing, Testing, and Monitoring        | Security audits, IDS/IPS, log management, penetration testing, hardening      |

### Total Estimated Time to Complete

| Activity                           | Hours           |
| :--------------------------------- | :-------------- |
| Reading & studying chapter content | 20–30 hours     |
| Hands-on labs & software exercises | 15–20 hours     |
| Class activities & final project   | 10–15 hours     |
| **Total (approximate)**            | **45–65 hours** |

> *This estimate varies based on prior experience and depth of engagement with hands-on exercises.*

---

## Assessment Structure

| Assessment Component | Weight |
| :--- | :--- |
| Mid-Exam | 30% |
| Class Activities & Final Project | 20% |
| Final Exam | 50% |

---

## Required Software & Tools

Students will need the following software to complete hands-on exercises and security testing labs:

| Tool | Purpose |
| :--- | :--- |
| **Kali Linux** (or other penetration testing distro) | Security testing, ethical hacking, vulnerability assessment |
| **Wireshark** | Network traffic analysis and packet inspection |
| **VirtualBox / VMware** | Virtual machine management for isolated lab environments |
| **OpenSSL** | Cryptography and certificate management exercises |
| **Python / Java** | Scripting custom security tools and automation |

### Optional / Recommended Tools

- **Nmap** – Network discovery and port scanning
- **Metasploit** – Penetration testing framework
- **Burp Suite** – Web application security testing
- **John the Ripper / Hashcat** – Password cracking exercises

---

## Key Terminology

This course introduces a comprehensive vocabulary of information security terms. Below are the foundational concepts every student must master:

### Foundation Concepts

| Term | Definition |
| :--- | :--- |
| **Information Security** | Protection of information and systems from unauthorized access, use, disclosure, disruption, modification, or destruction. |
| **CIA Triad** | Confidentiality, Integrity, Availability — the three core security principles. |
| **Asset** | Any data, device, or component that supports information-related activities and must be protected. |

### Risk Management

| Term | Definition |
| :--- | :--- |
| **Threat** | Any potential event or action that could cause harm (e.g., hackers, malware, natural disasters). |
| **Vulnerability** | A weakness that can be exploited by a threat. |
| **Risk** | Potential for loss: `Risk = Threat × Vulnerability × Asset Value` |
| **Residual Risk** | Risk remaining after security controls are applied. |
| **Risk Treatment** | Options to modify risk: Accept, Mitigate, Transfer, Avoid. |

### Access Management

| Term | Definition |
| :--- | :--- |
| **Identification** | Claiming an identity (e.g., username). |
| **Authentication** | Verifying that identity (e.g., password, biometric). |
| **Authorization** | Determining what an authenticated user can access. |
| **Least Privilege** | Granting only the minimum access necessary for job functions. |
| **RBAC** | Role-Based Access Control — permissions assigned to roles, users assigned to roles. |
| **MFA** | Multi-Factor Authentication — using two or more verification factors. |
| **Zero Trust** | "Never trust, always verify" — strict identity verification for every access attempt. |

### Cryptography

| Term | Definition |
| :--- | :--- |
| **Encryption** | Converting plaintext to unreadable ciphertext. |
| **Symmetric Encryption** | Same key for encryption and decryption (e.g., AES). |
| **Asymmetric Encryption** | Public/private key pairs (e.g., RSA). |
| **Hash Function** | One-way function producing a fixed-size digest for integrity verification (e.g., SHA-256). |
| **Digital Signature** | Cryptographic proof of authenticity and integrity. |
| **PKI** | Public Key Infrastructure — framework for managing digital certificates. |

### Malware & Attacks

| Term | Definition |
| :--- | :--- |
| **Virus** | Malware that replicates by modifying other programs. |
| **Worm** | Self-replicating malware spreading without user interaction. |
| **Trojan Horse** | Malware disguised as legitimate software. |
| **Ransomware** | Encrypts files and demands ransom for decryption. |
| **Phishing** | Fraudulent attempt to obtain sensitive information via deceptive communication. |
| **DDoS** | Distributed Denial-of-Service — overwhelming a target with traffic from many sources. |

### Security Operations

| Term | Definition |
| :--- | :--- |
| **IDS / IPS** | Intrusion Detection System (passive) / Intrusion Prevention System (active). |
| **SIEM** | Security Information and Event Management — aggregates and correlates log data. |
| **Incident Response (IR)** | Methodology for responding to and managing cyberattacks. |
| **BCP / DRP** | Business Continuity Plan / Disaster Recovery Plan. |
| **Defense in Depth** | Layered security controls — if one fails, another steps in. |

A complete glossary of over **150+ terms** is included in the course notes.

---

## Suggested Learning Path

For optimal results, follow this sequence:

1. **Read the chapter** thoroughly, taking notes on key terms and concepts.
2. **Review the learning objectives** at the start of each chapter to guide your focus.
3. **Complete hands-on labs** using the required software (Kali Linux, Wireshark, etc.).
4. **Test your understanding** using the chapter review questions (included in notes).
5. **Participate in discussions** or study groups to reinforce concepts.
6. **Complete the final project** — a comprehensive security assessment and policy design.
7. **Prepare for exams** using the glossary and chapter summaries.

---

## Additional Resources & Recommendations

### Free Online Resources

| Resource                                                        | Description                                                          |
| :-------------------------------------------------------------- | :------------------------------------------------------------------- |
| [NIST Computer Security Resource Center](https://csrc.nist.gov) | US government standards and guidelines (NIST SP 800 series)          |
| [OWASP](https://owasp.org)                                      | Open Web Application Security Project — web security resources       |
| [CVE Database](https://cve.mitre.org)                           | Common Vulnerabilities and Exposures — public vulnerability listings |
| [Kali Linux Docs](https://www.kali.org/docs/)                   | Official documentation for penetration testing tools                 |
| [Cybrary](https://www.cybrary.it)                               | Free cybersecurity courses and labs                                  |
| [TryHackMe](https://tryhackme.com)                              | Interactive hands-on security training (paid/free tiers)             |

### Certification Alignment

This course maps to foundational knowledge required for:

- **CompTIA Security+**
- **ISC² SSCP** (Systems Security Certified Practitioner)
- **GIAC GSEC** (Security Essentials)
- **CISSP** (domain foundations)

### Tips for Success

1. **Set up a lab environment early** — Install VirtualBox and Kali Linux during Week 1.
2. **Practice daily** — Even 15–20 minutes of hands-on tool use reinforces concepts.
3. **Document your work** — Keep a security notebook or digital journal of commands, findings, and lessons learned.
4. **Join a community** — Engage with security forums (Reddit r/netsec, StackExchange Security) to ask questions and share insights.
5. **Think like an adversary** — The best defenders understand how attackers think. Practice ethical hacking in your own lab.

---

## Final Project Overview

The final project requires students to:

1. **Conduct a risk assessment** for a mock organization across all seven IT domains.
2. **Develop a security policy framework** including AUP, access control policy, and incident response procedures.
3. **Perform basic vulnerability scanning** using tools from Kali Linux.
4. **Create a disaster recovery plan** with defined RPO and RTO.
5. **Present findings** in a professional report suitable for management review.

Detailed project specifications are provided during the course.

---

## License & Usage

This course material is provided for **educational purposes only**. All original content is free to use, adapt, and distribute for non-commercial teaching and learning. When using or adapting these materials, please attribute the source.

**Disclaimer:** This course includes discussions of security testing tools and techniques. Always obtain proper authorization before testing any system you do not own or have explicit permission to assess. Unauthorized access or attacks are illegal and unethical.

---

## Contributing

If you find errors or have suggestions for improvement, please open an issue or submit a pull request. Contributions that enhance the learning experience for all students are welcome.

---

*Built with dedication to accessible, high-quality cybersecurity education.*