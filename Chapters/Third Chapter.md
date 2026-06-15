# **CHAPTER 3: risks, threats and vulnerabilities**

## **Lesson Overview: Risk, Threats, and Vulnerabilities**

 "Nothing in life is certain," and for organizations, this uncertainty manifests as **risk**. The integration of technology exponentially increases this risk, making it imperative for organizations to formally understand and manage threats to their IT infrastructure and sensitive data.

**Goal:** To equip students with the knowledge to identify, distinguish, and understand the core components of organizational risk specifically risks, threats, and vulnerabilities and to introduce the fundamental principles of risk management as a defense strategy.

## **Lesson Objectives**
Upon completion of this chapter, you will be able to:

1. **Define** the core principles of risk management and its alignment with information security.
2. **Differentiate** between key risk terms: assets, threats, vulnerabilities, and risk.
3. **Identify** common perpetrators and various types of threats to an IT infrastructure.
4. **Explain** how attackers exploit vulnerabilities and list common attack vectors.
5. **Describe** the risk management lifecycle and the purpose of a risk management plan.
6. **Compare** qualitative and quantitative risk assessment approaches.
7. **Recognize** the critical role of countermeasures and list essential physical security controls.
## **Introduction: Why Risk Management is Central to Security**

Information security is not about eliminating all risk; that is impossible. Instead, it is about **managing risk** to ensure the survival and success of the business. Every action an organization takes involves a degree of risk. The goal is to find a balance between the utility (benefit) and the cost of various risk management options.

*   **Risk Tolerance Varies:** An established hospital has a very low risk tolerance, while a new startup might accept more risk for the chance of greater rewards.
*   **The Security Professional's Role:** You will work with others to identify risks and apply solutions so that critical business functions can continue, even when faced with obstacles. Your work directly supports the organization's most basic strategic goal: to stay in business.

## **Core Principles of Risk Management**

Two key principles must guide your decisions:

1.  **Do Not Spend More to Protect an Asset Than It Is Worth.**
    *   Determining an asset's true worth can be complex. The cost isn't just the price of replacement; it includes lost productivity, damage to customer confidence, lost sales, regulatory fines, and reputational harm. The true cost of a breach is often far higher than the immediate cleanup.

2.  **Every Countermeasure Must Align with a Specific Risk.**
    *   Countermeasures (safeguards and controls) require resources to implement. A control that doesn't mitigate a specific, identified risk is a "solution seeking a problem" and is difficult to justify.

### risk terminology 

1. **RISK:** Risk is the likelihood that something bad will happen. Most risks lead to possible damage or negative results that could impact an organization. Not all risks are inherently bad; some risks can lead to positive results. The extent of damage (or even positive effect) from a threat determines the level of risk. 
2. **THREAT** A threat is something bad that might happen to an organization. A threat could be a tornado hitting a data center or an attacker exfiltrating and leaking (perhaps for profit) sensitive data. 
3. **VULNERABILITY:** A vulnerability is any exposure that could allow a threat to be realized. Some vulnerabilities are weaknesses, such as a software bug, and some are just side effects of other actions, such as when employees use their personally owned smartphones to access corporate email or the corporate network. 
4. **IMPACT:** refers to the amount of risk or harm caused by a threat or vulnerability that is exploited by a perpetrator. For example, if malware or malicious software infects a system, the impact could affect all the data on the system, as in the case of a cryptolocker, which encrypts production data.
## **The Risk Management Process: A Continuous Cycle**

Risk management is not a one-time event. It is a continuous cycle with five key steps, as shown in Figure 3-1 of your text:

1.  **Identify Risks**
2.  **Assess and Prioritize Risks**
3.  **Plan Risk Response**
4.  **Implement Risk Response**
5.  **Monitor and Control Risk Response**

![[Pasted image 20251106184355.png]]

### **Step 1: Identify Risks**

The goal is to build a comprehensive list of anything that could go wrong and interrupt business operations (e.g., fire, flood, cyber-attack, human error).

**Methods for Identification:**
*   **Brainstorming:** Unstructured group input in a non-critical environment.
*   **Surveys & Delphi Method:** Anonymized questionnaires to foster open dialogue.
*   **Interviews & Working Groups:** Gathering detailed perspectives from specific areas.
*   **Checklists & Historical Information:** Using past incidents and industry-standard lists.

![[Pasted image 20251106184548.png]]

**Output: The Risk Register**
The result of this process is a **Risk Register** (Figure 3-2), a living document that contains for each risk:
*   A description of the risk
*   Expected impact
*   Probability of occurrence
*   Mitigation steps
*   Response steps if the risk occurs
*   A priority rank

![[Pasted image 20251106184627.png]]

### **Step 2: Assess and Prioritize Risks**

Once risks are identified, we must determine which are the most serious. We do this through assessment, which can be **Quantitative** (using numbers) or **Qualitative** (using ratings).

![[Pasted image 20251106184711.png]]

#### **Quantitative Risk Assessment**

This approach puts a financial value on risk, enabling clear cost-benefit analysis.

**The Quantitative Calculation Process:**

1.  **Asset Value (AV):** The total value of an asset (e.g., a server's hardware, software, data, and the business it supports). Example: $500,000.
2.  **Exposure Factor (EF):** The percentage of the asset's value lost in a single incident. Example: A disk failure corrupts 40% of the data, so EF = 40% (0.40).
3.  **Single Loss Expectancy (SLE):** The cost of a single occurrence of the risk.
    *   **Formula:** `SLE = AV × EF`
    *   **Example:** `$500,000 × 0.40 = $200,000`
4.  **Annual Rate of Occurrence (ARO):** How many times the threat is expected to occur per year. Example: A major disk failure happens once every 10 years, so ARO = 0.1.
5.  **Annualized Loss Expectancy (ALE):** The total expected financial loss per year. This is the most important figure.
    *   **Formula:** `ALE = SLE × ARO`
    *   **Example:** `$200,000 × 0.1 = $20,000 per year`

![[Pasted image 20251106184808.png]]

**The Business Decision:**
The ALE tells you the maximum you should spend on a countermeasure. If a backup system costs $8,000/year and reduces the ALE from $20,000 to a lower value, it is a sound investment.

*   **Pros:** Objective, data-driven, easy to justify financially.
*   **Cons:** Time-consuming, difficult to assign monetary value to intangibles like reputation.

#### **Qualitative Risk Assessment**

This approach uses relative scales (High, Medium, Low) to rate risks based on expert judgment.

**The Two Scales:**
*   **Probability/Likelihood:** The chance the threat will occur (Very High, High, Medium, Low, Very Low).
*   **Impact:** The negative effect on the organization if it does occur (Catastrophic, High, Medium, Low, Insignificant).

**The Risk Matrix:**
These two scales are plotted on a **Risk Matrix**. The intersection of likelihood and impact determines the overall risk level.
*   **Focus Area:** Risks in the **High Probability/High Impact** quadrant are the top priority for mitigation.

![[Pasted image 20251106185311.png]]

*   **Pros:** Faster, easier, good for intangibles, leverages organizational expertise.
*   **Cons:** Subjective, no direct financial justification.

**In Practice:** Most organizations use a **hybrid approach** a qualitative assessment to quickly find the most critical risks, followed by a quantitative analysis on those top risks to build a financial business case.

### **Step 3: Plan Risk Response**

For each prioritized risk, you must decide how to handle it. There are four common responses to **negative risks**:

1.  **Reduce/Mitigate:** Implement controls to lower the probability or impact of the risk. (e.g., installing antivirus software).
2.  **Transfer/Assign:** Shift the risk to a third party. (e.g., purchasing cyber insurance).
3.  **Accept:** Acknowledge the risk and choose to do nothing, typically because the cost of mitigation is greater than the potential loss. (e.g., self-insuring with a deductible).
4.  **Avoid:** Eliminate the risk entirely by discontinuing the risky activity. (e.g., deciding not to launch a product in a high-risk country).

There are also responses for **positive risks** (opportunities), such as **Exploit**, **Share**, **Enhance**, or **Accept**.

#### **Key Concepts: Total Risk vs. Residual Risk**

*   **Total Risk:** The risk to an asset before any controls are applied.
*   **Residual Risk:** The risk that remains after controls have been implemented.
    *   **Goal:** The objective of risk management is to reduce risk to an **acceptable level** (the "acceptable range" in Figure 3-5), not to zero. Residual risk is a fact of business life.

![[Pasted image 20251106185642.png]]

### **Step 4: Implement Risk Response**

This is the action phase where you deploy the chosen safeguards and countermeasures.

#### **Types of Security Controls:**

*   **Administrative Controls:** Policies, procedures, and training—things people are supposed to do or not do.
*   **Technical Controls:** Software and hardware solutions (firewalls, encryption).
*   **Physical Controls:** Locks, guards, mantraps, surveillance.

#### **Control Functions (by Activity Phase):**

*   **Preventive:** Stop an incident from occurring (e.g., IPS, door lock).
*   **Detective:** Identify that an incident is occurring or has occurred (e.g., IDS, alarm).
*   **Corrective:** Remedy the effects of an incident (e.g., restore from backup).
*   **Deterrent:** Discourage an action (e.g., warning signs).
*   **Compensating:** Provide an alternative way to meet a security requirement.

**Costing a Countermeasure:**
Remember, the cost is more than the purchase price. Consider:
*   Product, implementation, compatibility, environmental, testing, and productivity impact costs.

### **Step 5: Monitor and Control Risk Response**

The final, ongoing step is to ensure controls are working as intended.
*   **Continuous Monitoring:** Use logging and active testing to verify control performance.
*   **Certification & Accreditation:** Formally test and approve systems before they go live.
*   **Due Diligence:** Regularly evaluating controls shows auditors and management that the organization is taking a prudent approach to security.

#### **Connecting it All: Business Continuity and Disaster Recovery**

The entire risk management process feeds into higher-level plans that ensure the business can survive a major disruption:
*   **Business Impact Analysis (BIA):** Identifies the most critical business functions and the impact of their disruption. This is a key input for the...
*   **Business Continuity Plan (BCP):** A plan to ensure the *business* can continue operating after a disruption.
*   **Disaster Recovery Plan (DRP):** A plan focused on restoring the *IT infrastructure* and data after a disaster.

## **The Security Trinity - Risk, Threat, and Vulnerability**

To effectively defend an organization, you must first understand the relationship between three core concepts:

*   **Vulnerability:** A weakness in a system. This can be a software bug, a misconfiguration, or a flawed process.
    *   *Example:* An unpatched web server, an open network port, or a lack of employee security training.
*   **Threat:** Any action that can damage or compromise an asset by exploiting a vulnerability. A threat is the "actor" or "event."
    *   *Example:* A hacker, a malicious script, a natural disaster, or even a careless employee.
*   **Risk:** The probability that a threat will exploit a vulnerability and the resulting impact on the organization. It's the potential for loss.
    *   *Formula:* **Risk = Threat × Vulnerability × Impact**

![[Pasted image 20251106185940.png]]

**The Relationship:** You cannot eliminate all **threats**, but you can protect against **vulnerabilities**. By addressing vulnerabilities, you reduce the **risk** of a successful attack, even though the threat still exists.

### **Part 1: The Vulnerability Lifecycle**

Vulnerabilities, especially in software, are a constant reality.

**1. The Source of Vulnerabilities:**
*   All software has bugs. Some of these bugs create security vulnerabilities.
*   **Vendor Liability:** Software vendors often limit their financial liability for these vulnerabilities through an **End-User Licensing Agreement (EULA)**. For example, Microsoft's EULA may limit liability to $5.00, effectively transferring the risk to you, the end user.

**2. Finding Vulnerabilities:**
*   **Hackers & Security Professionals** use automated tools called **vulnerability scanners** (e.g., Qualys, Nessus, OpenVAS) to find known weaknesses.
*   These scanners use the **Common Vulnerabilities and Exposures (CVE)** database, a dictionary of publicly known security flaws.
*   **Key Resource:** The **National Vulnerability Database (NVD)** (`https://nvd.nist.gov`) is the U.S. government's repository that enhances CVE data with severity scores and impact metrics.

**3. The Race Against Time: Patching**
*   Once a vulnerability is announced, a "race" begins between attackers and defenders.
*   **Vulnerability Window:** The dangerous period between the announcement of a vulnerability and when a patch is applied.
*   **Zero-Day Vulnerability:** A particularly dangerous type of vulnerability where the threat is known, but no patch exists yet. The window is effectively "zero days" wide, leaving systems completely exposed until a fix is developed.

![[Pasted image 20251106190047.png]]

### **Part 2: Threat Targets in the IT Infrastructure**

To manage threats, we must know where they are most likely to strike. The "Seven Domains of a Typical IT Infrastructure" (Figure 3-7) provide a framework. Below is a summary of common threat targets (Table 3-3) and vulnerabilities (Table 3-2) in each domain.

| Domain | What is Targeted (Threat Target) | Common Weaknesses (Vulnerabilities) |
| :--- | :--- | :--- |
| **User Domain** | Human behavior and compliance with policy. | Lack of security awareness, accidental policy violations, falling for social engineering. |
| **Workstation Domain** | Laptops, desktops, and mobile devices. | Unauthorized access, malware, unpatched software. |
| **LAN Domain** | Internal network servers (Active Directory, file servers) and traffic. | Unauthorized network access, unencrypted data on the network, insecure file shares. |
| **LAN-to-WAN Domain** | Perimeter devices (firewalls, VPNs) and the DMZ. | Exposure of internal resources to the internet, introduction of malware from outside. |
| **WAN Domain** | Internet routers, service providers, and infrastructure. | Unencrypted data in transit, anonymous attacks (DoS), weak network device software. |
| **Remote Access Domain** | VPNs and the devices of remote workers. | Password attacks, unauthorized remote access, lost/stolen devices, delayed patching. |
| **System/Application Domain** | Servers, applications, and the sensitive data they hold. | Unauthorized access to servers, unpatched OS/application software, lack of digital certificates. |

![[Pasted image 20251006224609.png]]


### **Part 3: Categorizing Threats by Their Goal**

All threats ultimately aim to compromise one or more pillars of the **C-I-A Triad** (Confidentiality, Integrity, Availability).

| Threat Type | What it Attacks | Description | Examples |
| :--- | :--- | :--- | :--- |
| **Disclosure Threats** | **Confidentiality** | Unauthorized access to or disclosure of private information. | Packet sniffing, theft of a laptop with sensitive data, **espionage**. |
| **Alteration Threats** | **Integrity** | Unauthorized changes to data or systems. | Tampering with database records, altering configuration files. |
| **Denial/Destruction Threats** | **Availability** | Making systems or data unavailable or unusable. | **Sabotage**, Denial-of-Service (DoS) attacks, ransomware. |

![[Pasted image 20251106190209.png]]

### **Part 4: A Closer Look at Common Malicious Attacks**

Attacks can be **active** (altering systems/data) or **passive** (eavesdropping without change). Below are some of the most common techniques.

#### **A. Attacks on Access & Credentials**

*   **Brute-Force Attack:** Using software to try every possible password combination until the correct one is found.
*   **Dictionary Attack:** A faster version of a brute-force attack that only tries words from a dictionary list, exploiting poor password choices.
*   **Credential Stuffing:** Using stolen username/password pairs from one breach to try to log in to other, unrelated websites (many people reuse passwords).

#### **B. Attacks on Identity & Sessions**

*   **Spoofing:** Disguising a communication from an unknown source as being from a known, trusted source.
    *   **IP Spoofing:** Faking the source IP address to bypass network filters.
    *   **ARP Poisoning:** Spoofing MAC addresses on a local network to intercept traffic.
*   **Hijacking:** Taking control of a session.
    *   **Session Hijacking:** Stealing an active session between a user and a server to impersonate them.
    *   **Man-in-the-Middle (MitM):** Secretly intercepting and relaying messages between two parties who believe they are communicating directly with each other. The attacker can eavesdrop or alter the communication.
    *   **Browser Hijacking / Typosquatting:** Redirecting users to malicious websites through misspelled domain names.
*   **Replay Attack:** Intercepting and maliciously re-transmitting valid data to trick a system (e.g., replaying a captured authentication packet).
*   **Masquerading:** Pretending to be an authorized user or system, often using stolen credentials.

#### **C. Social Engineering Attacks (Attacks on People)**

These attacks manipulate human psychology rather than technical systems.

*   **Phishing:** Fraudulent emails/messages that trick victims into revealing sensitive data or clicking malicious links.
    *   **Spear Phishing:** Highly targeted phishing against a specific individual or organization.
    *   **Whaling:** Spear phishing targeting high-level executives ("the big fish").
    *   **Smishing:** Phishing via SMS (text messages).
    *   **Vishing:** Phishing via voice calls.
*   **Pharming:** Redirecting users from a legitimate website to a fake one by poisoning the DNS (Domain Name System). More dangerous than phishing as it doesn't require the user to click a link.
*   **Other Tactics:**
    *   **Impersonation:** Posing as an IT support technician, delivery person, or executive.
    *   **Tailgating:** Following an authorized person through a secure door.
    *   **Shoulder Surfing:** Observing someone typing their password.
    *   **Dumpster Diving:** Searching trash for sensitive documents.
    *   **Authority, Urgency, Scarcity:** Using psychological pressure to force a quick, unthinking action.

#### **D. Wireless Network Attacks**

*   **Evil Twin:** A rogue wireless access point that mimics a legitimate one to capture user traffic.
*   **Packet Sniffing:** Capturing and analyzing data packets traveling over a wireless network.
*   **War Driving/Chalking:** Locating and mapping wireless networks for potential exploitation.
*   **Jamming/Interference:** Disrupting wireless signals to cause a Denial-of-Service.

#### **E. Web Application Attacks**

These target the software that runs on web servers.

*   **SQL Injection (SQLi):** Injecting malicious SQL code into a web form to manipulate the back-end database. This can lead to data theft, deletion, or unauthorized access.
*   **Cross-Site Scripting (XSS):** Injecting malicious client-side scripts into web pages viewed by other users. This attacks the website's visitors, not the website itself.
*   **Cross-Site Request Forgery (CSRF):** Tricking a logged-in user's browser into sending an unauthorized request to a web application, performing an action without their consent.
*   **Buffer Overflow:** Sending more data to a program than it can handle, which can crash the program or allow the execution of malicious code.
*   **Zero-Day Exploit:** An attack that targets a previously unknown vulnerability for which no patch is available.

## conclusion 

Risks, threats, and vulnerabilities and how they impact the seven domains of an IT infrastructure and its assets are an everyday menace. It is essential that organizations and individual users identify their own risks, threats, and vulnerabilities and implement a plan to mitigate them. You learned about the reasons for and processes of risk management. You also learned about risk assessment, including the difference between a quantitative and a qualitative risk assessment as well as common responses to risk and how they can help to develop a risk reduction strategy. Many types of threats exist, including confidentiality threats, integrity threats, and availability threats. Another threat is the malicious attack. These attacks can originate from active threats that include brute-force, masquerading, IP address spoofing, session hijacking, replay, man-inthe-middle, and dictionary password attacks. Passive threats can include eavesdropping and monitoring. Vulnerabilities introduce weaknesses in the actual software used on production IT assets. Handling software vulnerabilities requires a vulnerability management plan that includes identifying and patching them in a timely manner. This race against time helps to reduce the vulnerability window and risk exposure caused by leaving exploitable vulnerabilities on production IT assets. With proper patching, this risk exposure can be reduced. Without it, hackers will likely find your software vulnerabilities and exploit them if they can. Threat targets are increasing as more users and devices connect to the Internet. Black-hat, white-hat, and gray-hat hackers; script kiddies; and crackers can launch attacks against common targets, including computer systems, network components, software, electrical systems, and databases.
