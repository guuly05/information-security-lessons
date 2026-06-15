# CHAPTER 8: Security Operations and Administration

---

## Learning Objectives

When you complete this chapter, you will be able to:

- Develop and maintain comprehensive security programs
- Understand and apply professional ethics in security roles
- Promote user awareness of security through training and education
- Create and support policies that govern the security infrastructure
- Classify data according to value, sensitivity, and criticality
- Control major and minor changes to systems through formal processes
- Understand how the System Life Cycle (SLC) and System Development Life Cycle (SDLC) promote security
- Evaluate and manage security outsourcing relationships
- Implement personnel security principles including least privilege and separation of duties
- Apply configuration management to maintain system integrity

## Introduction

SECURITY PROFESSIONALS MUST UNDERSTAND how security operations and administration create the foundation for a solid security program. Your role as a security professional is similar to that of a coach. You work with staff to identify the strengths and weaknesses of your "players," or assets, and your goal is to win the game, which, in the world of the security professional, is to secure your organization's resources. Your "opponents" are unauthorized users trying to crash your systems or steal your data and use it against you.

As a coach, you know the rules, and you have a playbook of strategies, which you need to keep out of the hands of your opponents. You also need to make sure your strategies abide by the rules and regulations of the industry. You have to play by the rules, but that does not mean your opponents will. To prepare your players for the challenge, you must educate and train them, so they have the skills they need to work together as a team to win the game.

If you are successful, your organization will run as smoothly as a championship team, and everybody will understand the mission and how to work together to complete it. If you are not prepared, your team will appear confused. Players will seem to be doing their own thing, regardless of the consequences. The next thing you know, your organization's information will fall into the hands of your opponents, and your systems will not work the way they are supposed to. Your trade secrets will no longer be secret, your organization will spend a lot of money fixing what's broken, and you and your employees might find yourselves "on the bench" or even looking for other jobs.

Everyone wants to be on a winning team. In this chapter, you will learn the skills needed to develop a strong security administration team.

## 8.1 Security Administration

**Security administration** within an organization refers to the group of individuals responsible for planning, designing, implementing, and monitoring an organization's security plan. The physical location where they work is often referred to as the **security operations center (SOC)** .

Even though it is not required that the SOC team work in a central location, it often does, where there are several large video screens that display real-time operational status of networks and information systems. With today's remote and distributed workforce, it is possible for a geographically diverse SOC team to work closely to maintain environmental security, but that's not all the SOC team members are responsible for. They work as a cohesive unit to share information, experience, and insight to collectively assess prevailing conditions, recommend actions as conditions change, and implement those changes.

As early SOC teams struggled to manage the growing volume of information about networks and systems, they began to accumulate and integrate useful tools, which grew into a tool set called security information and event management (SIEM) systems. SIEM provides a rich, integrated set of tools to help collect, assess, and visualize a networked environment's state. The latest extension to the SOC toolbox is a superset of tools that includes SIEM and others, used to organize and manage the response to security incidents. A security, orchestration, automation, and response (SOAR) system gives the SOC team an integrated set of tools with which to determine the security level of a networked environment, identify any anomalies, and respond to any issues in a structured manner.

Before you can form an administrative team, though, the organization must identify and document its information assets, after which, you should assign each responsibility to a person or position. This administrative team then determines the sensitivity of each asset so that it can plan how to secure each one accordingly.

### 8.1.1 Controlling Access

A primary task of an organization's security administration team is to control access to systems or resources. There are four aspects of access control:

- **Identification**—Assertions made by users about who they are
- **Authentication**—The proving of that assertion
- **Authorization**—The permissions a legitimate user or process has on the system
- **Accountability**—Tracking or logging what authenticated and unauthenticated users do while accessing the system

The security administration team leads these efforts by determining the best security controls to implement to secure an organization's resources.

### 8.1.2 Documentation, Procedures, and Guidelines

The security administration team handles the planning, design, implementation, and monitoring of an organization's security program. To make the best decisions to secure assets, several types of documentation are necessary to provide the input the security administration team needs. The most common documentation requirements include the following:

- **Sensitive assets list**—What assets must the organization take measures to secure? The list can include computers, devices, network components, databases, documents, and any other assets that could be vulnerable to attack.
- **The organization's security process**—How does it all work?
- **The authority of the persons responsible for security**—Which administrator is responsible or authorized for what assets and actions?
- **The policies, procedures, and guidelines adopted by the organization**—What information needs to be communicated, how is it communicated, and when is it communicated?

The security administration team puts together all the pieces of a puzzle to ensure the organization complies with stated policies. An organization must comply with rules on two levels:

- **Regulatory compliance**—The organization must comply with laws, government regulations, and contractual requirements.
- **Organizational compliance**—The organization must comply with its own policies, audits, culture, and standards.

As a result, the security administration team's documentation, procedures, and guidelines focus on compliance and compliance monitoring. The team members must ensure that the organization follows the various rules and regulations.

### 8.1.3 Disaster Assessment and Recovery

The security administration team's responsibilities include handling events (e.g., incidents, disasters, and other interruptions) that affect an organization's computers, devices, and networks. To handle these events, the security administration team forms an incident response team, which comprises individuals who are responsible for responding to incidents and investigating security breaches. Moreover, the security administration team also manages the emergency operations group, which is responsible for protecting sensitive data in the event of natural disasters and equipment failure, among other potential emergencies.

Despite the best efforts of the incident response team, the emergency operations group, and system administrators, all systems are still subject to failure or attack. Therefore, the best a security administration team can do is to ensure that an organization can respond rapidly and effectively to any event.

## 8.2 Security Outsourcing

Many organizations rely on outside firms to handle security monitoring and analysis, which means you might need to monitor the work of the outsourcing firm or work with it as an external entity when handling incidents. This approach has both advantages and disadvantages:

**Advantages**—An external security management firm has a high level of expertise because it focuses on security—and security only—every day. Simply put, it will have expertise and experience that an organization alone might not have.

**Disadvantages**—Outsourcing has two primary disadvantages. First, the outsourcing firm might not know the organization well nor possess enough internal knowledge necessary to protect its assets. Second, by outsourcing, the organization will not be developing its own in-house capability or talent and will therefore need to continue to pay for these services indefinitely.

### 8.2.1 Outsourcing Considerations

The security administration team and an outside firm must work together closely to make sure they agree to specific security requirements. Integrating data or processing with third parties introduces new threats, and relocating data or processes (or both) outside of an organization's own data centers raises trust questions. How can you trust another organization to protect your intellectual property? Though there are many concerns to address when outsourcing, the main concerns include the following:

- **Privacy**—Does the third party agree to uphold the organization's privacy policy? How does it plan to control how data is collected, stored, handled, and destroyed?
- **Risk**—What additional risks exist by transferring data over a trust boundary? How are any new risks addressed? Who is responsible for managing new outsourcing risks?
- **Data security**—What controls protect data confidentiality and integrity from unauthorized access? Are access controls consistent with internal controls? How is data availability protected? Are backups and redundancy measures in place to minimize downtime? How are backups and redundant data copies protected?
- **Ownership**—Who owns the data, the infrastructure, and the media? Who is responsible for each component?
- **Adherence to policy**—Does the third party commit to upholding the organization's security policies and procedures?

Several types of agreements that help to formalize answers to the preceding questions are common when outsourcing to external organizations. A list of the most common agreements that define how an outsourcing relationship works would include the following:

- **Service level agreement (SLA)** —This type of agreement is a legally binding formal contract between an organization and a third-party external organization that details the specific services the third party will provide. Following are examples of security-related services detailed in an SLA:
  - How and when potential security breaches are identified and communicated
  - How logs and events are reported
  - How confidential data is handled
  - What the security system uptime requirements are (e.g., an organization might require that all critical security systems have a 99.99 percent reliability)

The SLA should communicate the expectations and anticipate the needs of both the organization and the outside firm. Individual members of the security administration team must thoroughly analyze their department's risks because any risk unaccounted for is likely to cost an organization in terms of either data loss or expenses to fix it. You can compare this situation to maintaining an automobile: Regular oil changes are less expensive than blown head gaskets, so maintaining an engine is cheaper than fixing one.

- **Blanket purchase agreement (BPA)** —As a streamlined method of meeting recurring needs for supplies or services, a BPA creates preapproved accounts with qualified suppliers to fulfill recurring orders for products or services.

- **Memorandum of understanding (MOU)** —Also called a letter of intent, an MOU is an agreement between two or more parties that expresses areas of common interest that result in shared actions. MOUs are generally less enforceable than a formal agreement but still more formal than an oral agreement.

- **Interconnection security agreement (ISA)** —Often an extension of an MOU, an ISA documents the technical requirements of interconnected assets. This type of document is most often used to specify technical needs and security responsibilities of connected organizations.

The negotiation process and creation of agreements is one of the first steps in the business partner onboarding process. Any time an organization decides to outsource data or processing, it must carefully consider the security impact and responsibilities, and the onboarding process is just the time to plan for contingencies before a problem occurs. Moreover, it provides the opportunity to clearly communicate goals and expectations for all parties. Likewise, you should specify an offboarding process to follow when you terminate relationships with outsourced resources. This process defines how to transfer control of data and other assets, terminate communications, and complete any open transactions and is necessary to ensure that no remnants of data or processing remain once an outsourcing relationship ends.

## 8.3 Compliance

An organization's security policy sets the tone for the way you approach security activities and states the rules with which you must comply. Think of a security policy in terms of traffic laws, whose purpose is to maintain a certain degree of order and safety on the roads, but only if they are enforced; otherwise, the roads can become dangerous. Likewise, an information security policy must be enforced to be effective in protecting assets. When policies are enforced, the organization complies with them.

Three primary means are used to ensure compliance:

1. Event logs
2. Compliance liaison
3. Remediation

### 8.3.1 Event Logs

**Event logs** are records of actions that an organization's operating system or application software creates, showing which user or system accessed data or a resource and when. You can think of event logs as being similar to the system a public library uses to keep track of who checks out books: When a book is late or missing, the library checks its records to determine who last checked out the book. Likewise, when an information security breach occurs, an event log helps determine what happened to the system and when so that you can identify the culprit or fix the problem.

You can change the amount of information that event logs record. To record every event requires a tremendous amount of disk space and will probably slow down an organization's computers as well as making reading through the log files more difficult because there is so much data to examine. Contrarily, logging too few events may cause some important details to slip through the cracks. Therefore, it is important to record all the actions that you may need in the future to investigate security problems. Another concern is to ensure that access to the event logs is controlled because you do not want an attacker to be able to compromise the system and then erase any trace of the attack.

### 8.3.2 Compliance Liaison

As organizations and security policies become larger and more complex, staying compliant becomes more difficult. Therefore, organizations employ **compliance liaisons** whose responsibility is to make sure that all personnel are aware of—and comply with—the organization's policies. Because departments within an organization might have their own security ideas or needs different from other departments', a compliance liaison works with each department to ensure it understands, implements, and monitors compliance applicable to it. Moreover, a compliance liaison can also help departments understand how to include information security in their daily operations.

Another important role of a compliance liaison is to review agreements throughout any outsourcing engagement to ensure the rules that were established in the interoperability documents are being followed. This review helps validate whether a service provider is in compliance with current agreements. As compliance has become more and more important, many organizations have expanded executive leadership roles to include a chief security officer (CSO) or chief information security officer (CISO). A CSO/CISO provides guidance to executives in matters related to security. In organizations with a CSO/CISO, the compliance liaison works under that person's guidance.

### 8.3.3 Remediation

Mitigating vulnerabilities reduces the risk of attacks against an organization's computers and networks. In some cases, the best solution is to block an intruder and deny access to a resource, thus lessening the risk. In other cases, removing the vulnerability is possible through **remediation**. Remediation involves fixing something that is broken or defective, and, with computer systems, it refers to fixing security vulnerabilities.

Of course, some problems are more important than others; therefore, you should fix high-risk issues before lower-risk ones. When possible, the best option is to remove a vulnerability altogether, but, if you cannot do so effectively, the next best step is to remove the ability of an attacker to exploit it.

You should always design security policies to protect your assets from attack, but not all organizations invest enough in security on their own. Several government bodies and industry governance groups have developed requirements that compel organizations to remediate certain types of vulnerabilities. Compliance requirements exist because a governance body recognized weaknesses and decided to mandate protection against those weaknesses. Complying with mandated requirements goes a long way toward helping organizations to become more secure and to avoid sanctions or penalties, whereas noncompliance can result in fines or other penalties that can limit an organization's ability to carry out business functions. Furthermore, most compliance requirements come with auditing or other monitoring requirements that allow auditors to determine compliance.

Compliance is extremely important in securing information technology systems, but it is only the first step toward being secure. Think of checking all the compliance boxes and covering just the minimums. That is a great start, but you should strive to go beyond meeting compliance minimums.

## 8.4 Professional Ethics

Every respected profession has its own code of ethics and conduct, and adhering to such a code fosters the respect of any profession's practitioners. In this respect, the security profession is no different from other professions. Because people will not follow the rules if they do not trust the leaders, it is important that security professionals have a definite code of ethics that governs their behavior. Most security certification organizations publish their code of ethics, and, in fact, most certifications require candidates to commit to adhering to a specific code of ethics before qualifying for the certification. For example, both (ISC)² and CompTIA provide solid ethical guidelines. However, guidelines are not effective unless people adopt and practice them. Here are some tips for practicing strong ethics:

- **Set the example**—Security professionals must demonstrate strong ethical principles in their daily activities so that users will follow their lead. Being serious about ethics will help users to be serious also.
- **Encourage adopting ethical guidelines and standards**—Security professionals must know their ethical boundaries and set an example by adhering to them, which often means making difficult decisions and setting a good example. They must push the organization to define its code of ethics, which, in turn, helps the staff operate ethically and responsibly.
- **Inform users through security awareness training**—Security professionals must ensure that users are aware of and understand their ethical responsibilities.

### 8.4.1 Common Fallacies About Ethics

For security professionals, simply writing down a list of ethics-oriented rules is not enough; they must also apply ethics in their everyday lives. The first step in adhering to ethics rules is to understand the most common assumptions that many computer users hold that may lead them to unethical behavior. Here are some of these common assumptions:

- Users assume that computers should prevent abuse. If they can gain unauthorized access, it's the organization's fault—not theirs.
- Users believe that, in some legal systems, they have the right to explore security vulnerabilities as a form of free speech or expression.
- Users think their actions may cause only minor damage and that a little damage will not bother anyone.
- Users think that, if it's easy to break in, it must be all right to do so.
- Users think that hacking is okay if what they do is not damaging. They think that, if they are not making any money or otherwise advancing themselves by hacking into a system, they must not be committing a crime.
- Users think information should be free and that it's okay to look through somebody's system to obtain information.

### 8.4.2 Codes of Ethics

A code of ethics helps ensure professionalism, and there are several published codes that apply to information security. For example, published statements from the **Internet Architecture Board (IAB)** summarize the tone of most security-related codes of ethics and explain what the IAB considers ethical and appropriate behavior.

#### IAB Statement of Policy

The IAB has provided a list of unethical and unacceptable online practices, specifically related to activities involving the Internet. In 1989, the IAB issued RFC 1087, which is a statement of policy about Internet ethics. Although it was one of the first statements on the ethics of Internet use, it still applies today. RFC 1087 states that any activity is unethical and unacceptable that purposely does any of the following:

- "Seeks to gain unauthorized access to the resources of the Internet"
- "Disrupts the intended use of the Internet"
- "Wastes resources (people, capacity, computer) through such actions"
- "Destroys the integrity of computer-based information"
- "Compromises the privacy of users"
- "Involves negligence in the conduct of Internet-wide experiments"

The key point of the document is this: Access to the Internet is a privilege, not a right.

### 8.4.3 Professional Requirements

In any profession, rules and regulations enforce professional ethics, and sometimes, those rules come from certifying agencies, which means that, if you violate the rules, you risk losing your certification or license. In other contexts, laws and regulations require ethical behavior. For example, the Organisation for Economic Co-operation and Development (OECD) is an organization of more than 30 countries whose goal is economic cooperation and growth. In 1980, it created eight privacy principles, which have formed the basis for much of the world's privacy legislation. In summary, the principles state the following:

- An organization should collect only what it needs.
- An organization should not share its information.
- An organization should keep its information up to date.
- An organization should use its information only for the purposes for which it was collected.
- An organization should properly destroy its information when it is no longer needed.

> **NOTE:** For more information about the OECD, visit www.oecd.org. You can find the latest "OECD Privacy Framework," which includes guidelines and their application in today's environments, at www.oecd.org/sti/ieconomy/privacy-guidelines.htm.

> **TECHNICAL TIP:** As you have learned, many certification organizations require adherence to a code of ethics. You can find the (ISC)² Code of Ethics at www.isc2.org/Ethics. The CompTIA Candidate Code of Ethics is available at www.comptia.org/testing/testing-policies-procedures/test-policies/continuing-education-policies/candidate-code-of-ethics.

---

## 8.5 Personnel Security Principles

For all the technical solutions you can devise to secure an organization's systems, the human element remains your greatest challenge. You might be surprised how far a little education can go. If staff members are aware of how security risks can hurt both themselves and the organization, they will be more likely to help you run a tight ship.

It's important to know what a user should and should not do, and the best way to accomplish this goal is to create well-defined job descriptions, job roles, and responsibilities. When you know what people should be doing, it's easier to identify activities they are not supposed to do. If their roles or responsibilities are vague, it's more difficult to flag bad behavior, which means people are more likely to get away with things.

Minimizing access to information and assets is an important security control. Therefore, pay careful attention to any security concepts and controls that directly affect personnel. Because people are the most important assets in an organization, it is vital that they know how to contribute to maintaining the organization's security.

### 8.5.1 Limiting Access

When deciding how to grant access to users, one of the core principles is **least privilege**, which means limiting access to users based on the levels of permissions they need to perform their duties. Using this principle helps to keep unauthorized users from accessing information they should not be able to access. For example, weak access controls may allow a salesclerk to view employee salaries.

Another concept that relates to the principle of least privilege is the **need-to-know** requirement, which states that people should have access only to information they need to perform their jobs, regardless of their clearance level. The application of this principle means that, even though users might have a top-secret security clearance, they should not have access to all top-secret information, only the information they need to do their jobs.

### 8.5.2 Separation of Duties

Another security principle is **separation of duties**. This principle entails breaking a task into subtasks so that different users must carry them out; in other words, a user who plans to harm a system must get help from others, or form a conspiracy, which is hard to organize and to hide. For example, separation of duties in the context of vendor management helps prevent an employee from opening a bank account for Acme Consulting, going into the system at work to create a new vendor named Acme Consulting, and then cutting a check for $1,000 to Acme Consulting.

### 8.5.3 Job Rotation

Yet another way to protect against personnel-related security violations is to use **job rotation**, which minimizes risk by rotating employees among various systems or duties and thus prevents collusion (i.e., several employees conspire to commit fraud). It also gives managers a chance to track which users were authorized to take what actions and when. Therefore, if other security measures have failed, job rotation provides an opportunity to find the security breach before it inflicts more harm. Moreover, job rotation provides trained backup because several employees learn the skills of specific jobs.

### 8.5.4 Mandatory Vacations

Much like job rotation, **mandatory vacations** provide the chance to detect fraud. When users are on vacation, you should suspend their access to the organization's environment, thus preventing them from working from home, where they might attempt to cover their tracks. Moreover, under U.S. banking rules, for example, certain bank employees must take two consecutive weeks of vacation, and, until recently, the law forbade managers from contacting these vacationing employees with work-related matters. That rule has since been relaxed to allow for read-only access to systems so that employees can at least keep up with their email correspondence. However, they still cannot participate in work-related activities while on vacation.

### 8.5.5 Security Training

Because personnel are so important to solid security, one of the best security controls you can develop is a strong security training and awareness program. Security training helps gain the support of all employees, who then become security advocates who are motivated to comply with policies that relate to their jobs and to be careful to avoid security breaches. Following their initial security training, employees should undergo repeated training at specified intervals, which refreshes employees' knowledge and reminds them of the importance of security. Well-trained personnel can make the difference between a secure environment and a collection of attacks and mistakes.

Employees should be aware of security threats (e.g., installing rogue technologies, selecting weak passwords, and phishing attacks) to an organization, especially from human factors. These types of threats are common because so many organizations fail to train their personnel on the importance of recognizing them. Simply explaining how weak passwords can endanger personal and business information can often encourage users to create stronger passwords.

### 8.5.6 Security Awareness

A security awareness program should address the requirements and expectations of an organization's security policy, which requires actions and provides authority for security controls, and is one of the best forms of defense. Employees are more likely to comply with a security control if they realize that the policy mandates it. In addition to explaining why each part of the policy is necessary, the program should explain the penalties for policy violations.

An awareness program is different from a formal training program. Most users do not understand what security is and why it's necessary. You can use security awareness programs—including posters, emails, and employee newsletters, among other tools—to do the following:

- Teach users about security objectives
- Inform users about trends and threats in security
- Motivate users to comply with security policies

Employees generally want to do what is best for the company, but they will often bypass security measures to complete their work more quickly when security seems to get in the way of their productivity. For example, suppose Bob, an employee, is home for the weekend and receives a call from Sue, an employee at the office, asking him for his password to get to a file so she can finish a project. In this situation, even though employees have been reminded over and over of the risks of sharing passwords, most of them will still be quick to reveal their password to others. Therefore, the security professional must reinforce the importance of employees' following security policies as well as teach them how to solve productivity problems and still maintain a high level of security.

Awareness programs do just that, by reminding staff about security policies. They can also measure how well the staff follows the security policy, provide staff with practical advice on how to deal with security incidents, and convince staff members that security is their personal duty. Such programs can help employees change their behavior so that security becomes a part of their daily routine.

Make note of employees who are not following policies, and use this information in a training session to present employees with scenarios that are specific to their work. Ask employees, "What would you do when ______?" The information you gather will help identify gaps in the awareness program so that you can tailor the program to address them.

### 8.5.7 Social Engineering

One of the most popular types of attacks on computer systems, as well as one of the most critical areas of security, involves social engineering, which entails deceiving or using people to get around security controls. Because most people want to be helpful, it is not too hard for attackers to convince those with system access to do something they should not do. And, as the number of employees with access to systems and data increases, the risk of security breaches increases further. However, technical solutions will not stop an authorized user from calling an unauthorized person and reading sensitive data over the phone. Therefore, the best way to avoid social engineering is to train personnel to recognize social engineering attempts and how to handle them. The security training should cover the most common types of social engineering attacks, including:

- **Intimidation**—Using threats or harassment to bully another person for information
- **Name-dropping**—Using the names of managers or superiors to convince another person that a higher authority has allowed access to information
- **Appeals for help**—Tugging at a person's sense of compassion or understanding of a difficult, and perhaps unreasonable, situation. The goal of the emotional appeal is to bypass normal procedures or gain special consideration, and when combined with an incentive, such as a reward, this type of engineering is very effective. For example, consider the scam in which scammers promise to send you money if you will help them transfer money to a disadvantaged person. Unfortunately, this type of emotional appeal fools many people every year.
- **Phishing**—Technology works quite well in social engineering, as, for example, with phishing. In a phishing attack, scammers create an email or webpage that resembles the work of a reputable organization, hoping that you believe it's the real organization so you will share sensitive information with them. They then use this information to gain access to your financial information or to steal your identity. A phishing attack can also take the form of a survey that asks questions in an effort to capture sensitive information.

> **NOTE:** For more information about the latest phishing techniques and fraud alerts, see www.fraudwatchinternational.com/phishing.

---

## 8.6 The Infrastructure for an IT Security Policy

Every company operates within a complex combination of laws, regulations, requirements, competitor challenges, and partner expectations as well as being affected by morale, labor relations, productivity, costs, and cash flow. Within this environment, management must develop, publish, and maintain an overall security statement and directives. From the security team's perspective, a security program addresses these directives through policies and their supporting elements, such as standards, procedures, baselines, and guidelines. Figure 9-1 shows the elements of a security policy environment.

![[Pasted image 20260303105326.png]]
**Figure 8-1** The security policy environment.

Each element has a specific requirement for security professionals, who are involved with compliance monitoring, security awareness, training, access control, privacy, incident response, log analysis, and more. The security policy sets the tone and culture of an organization, which means that security professionals are often required to apply policy intent by putting what a policy says into action. Therefore, you must understand the details of the organization's security policy, which is the high-level statement of values and direction, supported and made possible by the organization's standards, baselines, procedures, and guidelines.

The role of the security professional is to provide support for these elements. This support includes informing personnel of policies, training, and enforcement when any policy element is violated as well as having a role in any updates or changes. Figure 9-2 shows a typical security policy hierarchy.

![[Pasted image 20260303105504.png]]
**Figure 8-2** The security policy hierarchy.

### 8.6.1 Policies

Written security policies document management's security goals and objectives and explain the company's security needs and its commitment to meeting those needs. A security policy should read like a short summary of key facts because management will have difficulty embracing and approving a policy that is too complex.

For example, a good organizational security policy might read simply as "Security is essential to the future of our organization" or "Security in our products is our most important task." This type of statement provides managers with guidance they need to make decisions. The security policy also helps an organization evaluate how well it is complying with laws, regulations, and standards of due care and due diligence, but the primary purpose of any security-related policy is to reduce risk by helping the organization focus its efforts in a particular area.

Policies that are not read, understood, available, enforced, and updated are not of much value. Post policies in a location available to every employee, for example, in break rooms. Policies must be current, especially in keeping with new laws, regulations, and any other requirements. You should meet with employees at least once a year to ensure they are up to date on the latest policies and be sure to maintain a record of this review with each employee.

A security policy helps all employees understand the assets and principles the organization values. Therefore, with a clear policy, an organization's staff is more likely to respect the organization's resources. Remember, personnel will take policies only as seriously as the organization does.

A **functional policy** sets out the direction for the management of an organization pertaining to security in such specific functional areas as email use, remote access, and Internet interaction (including social media). The departments responsible for these functional policies write them. For example, human resources, IT, operations, and facilities would each produce its own specific functional policy. Moreover, a functional policy should use strong language, such as *will* and *must*, to demand attention, and refrain from using a term such as *should*, which most people consider as merely a suggestion and not a mandate. For example, a clearly stated and strong access control functional policy might read as follows: "All authorized users must be allowed to do only their authorized tasks. Unauthorized users must not have access to the company systems or resources."

One example of a functional policy is a **privacy policy**, which specifies to consumers how an organization collects, uses, and disposes of their personal information. Another example of a functional policy is an acceptable use policy (AUP), which sets clear limits on how the organization will allow its assets to be used. The most common focus of an AUP dictates the way personnel must use the organization's computing resources, including guidance on the acceptable use of social media or even specific websites.

Policies allow organizations to state different goals at very high levels. These goals may be intended for their own employees, temporary personnel, business partners, customers, or perhaps all of these groups. They set the organization's tone and communicate commitment in different areas. All decisions that an organization's personnel make should flow from these high-level policies.

### 8.6.2 Standards

**Standards** are mandated requirements for hardware and software solutions used to address security risk throughout an organization. Standards might refer to a specific antivirus product or password-generation token. Simply put, when a standard is in place and enforced, it means the organization has selected a solution—and that solution only—to fulfill a policy goal.

Adopting standards carries many advantages. Often, standards save an organization money because it can negotiate bulk purchases with vendors. For example, a vendor might sell a single-user license for $29.95, but that same vendor might sell multiple licenses for only $24.95 per license. If that organization needs multiple licenses to comply with a standard, bulk purchasing can save the company several thousand dollars. In addition, many vendors offer free training with bulk purchases. Taking advantage of vendor-provided training without cost and using a single solution can save the organization the time and trouble of training its personnel and ensure that everyone follows the same procedures.

You do not have to develop your own standards for each situation because you can adopt standards created by government, industry, or other sectors and use them as the organization's own. Standards also establish a common basis throughout an organization, which helps to keep all departments on the same page and ensures that each department has the blueprints it needs to stay compliant.

The main disadvantage of standards is vulnerability. If the selected product is flawed, the entire organization will be at risk after installing the flawed product. A single standard cannot work if a vendor does not support the product or if it is too expensive to maintain or license. Examine alternatives when evaluating products for standards and be sure that each selection made comes with a guarantee of support if problems arise.

### 8.6.3 Procedures

One of the most powerful tools available to security professionals is **procedures**, which are step-by-step systematic actions taken to accomplish a security requirement, process, or objective. They can provide documentation of the way an organization does business and ensure that employees' critical knowledge does not remain only in their heads. Procedures cover things such as changing passwords, responding to incidents, and creating backups. Figure 8-3 shows a few examples of procedures.

![[Pasted image 20260303105557.png]]
**Figure 8-3** Systematic actions.

Procedures help enforce the intent of a policy. They require an employee to follow a series of organized steps to complete a task. All of the following statements are true of procedures:

- They reduce mistakes in a crisis.
- They ensure important steps are not missed.
- They provide for places within the process to conduct assurance checks.
- They are mandatory requirements, like policies and standards.

### 8.6.4 Baselines

In many cases, it is helpful to define and document basic configurations for specific types of computers or devices. For example, having a document that lists the components and configuration settings for a standard workstation makes it easy to ensure that all new workstations are the same. Security personnel often create such basic configuration documents, called **baselines**, to ensure that they enforce the security minimums. Baselines are one type of benchmark that helps ensure a minimum level of security exists across multiple applications of systems and across different products.

Baselines are helpful in configuring new computers or devices as well as for comparing with existing systems to see whether they still meet the minimums. Figure 8-4 shows a basic baseline corporate configuration.

![[Pasted image 20260303105631.png]]
**Figure 8-4** Baseline corporate configuration.

Baselines specify how to implement security devices to make sure that they create a constant level of security throughout the organization. Different systems or platforms have different ways of handling security issues, and baselines tell system administrators how to set up the security hardware devices and software for each platform, which helps achieve and maintain a constant level of security.

Baselines are the great leveler of options offered through different security products, operating systems, and applications, a factor that is becoming increasingly important as more hybrid products enter the security market. These products combine services into multifunctional devices. Organizations often create baseline standards for each operating system in use. There might be different baselines for Windows 8, Windows 10, Windows Server 2012 R2, Windows Server 2016, Windows Server 2019, macOS, Linux, Android, iOS, and so on.

### 8.6.5 Guidelines

Organizations often use **guidelines**, which are simply actions that the organization recommends (e.g., which products and systems are acceptable for use), to help provide structure to a security program. These guidelines usually exist in the form of white papers, best practices, or other formats defined by an organization's security program.

You must carefully select the language you use in guidelines. A few wrong words can transform a guideline into a company standard. For example, consider the following example of an overarching statement as dictated by the company CEO: "This company will follow the recommendations of the ISO 27001 standard." That statement makes ISO 27001 mandatory within that organization. Make sure that's the intent before you make such a bold statement.

---

## 8.7 Data Classification Standards

Mandatory access control (MAC) involves assigning each object a specific classification, which often relies on the regulations that apply to the specific type of data. Examples include the protection of personal information, financial information, and health information.

Classifying data is the duty of the data owner, which is the person who owns the data or someone the owner assigns. A similar term, system owner, refers to the person or group that manages the infrastructure. System owners are often in control of change or configuration management, but they are not in control of data classification.

It's important to understand the difference between clearance and classification. The authorization process grants clearance to users (subjects), and the data owner assigns a classification to data (objects). Systems enforce access control by determining that a subject has the right clearance to access a classified object and usually enforce access restrictions based on the principles of least privilege and need to know.

Organizations consider three criteria in classifying information:

- **Value**—You can define the value of information by several measures: the value to the organization, the value to competitors, the cost of replacement or loss, and the value to the organization's reputation.
- **Sensitivity**—Sensitivity is the measure of the effect that a breach of integrity or the disclosure of information would have on the organization. Organizations can measure sensitivity in many ways, including liability or fines, reputation, credibility, or loss of market share.
- **Criticality**—Criticality is the measure of the importance of the information to the mission of the organization. What would happen to the organization if the information were lost?

### 8.7.1 Information Classification Objectives

The objectives of classifying information are as follows:

- To identify information protection requirements, which are based on the risk the business faces if the information is disclosed or the data or system is corrupted
- To identify data value in accordance with organization policy
- To ensure that sensitive and/or critical information is provided appropriate protection/controls
- To lower costs by protecting only sensitive information
- To standardize classification labeling throughout the organization
- To alert employees and other authorized personnel to protection requirements
- To comply with privacy laws and regulations

Organizations can derive many benefits from classifying information:

- Data classified as sensitive or critical gets a level of protection that matches that data's classification.
- The organization gets more value for its security investment because it applies increased controls only where it needs them most. Compare, for example, costs of physical security at an expensive jewelry store, an inexpensive jewelry store, and a costume jewelry store. None of those stores would operate efficiently using the security system of any of the others. A costume jewelry store would waste lots of money if it invested the same amount as the store that secures expensive jewelry. Likewise, a store that invests in only minimal security to protect its expensive jewelry exposes itself to excessive risk of loss. All organizations have data that is of high, medium, and low value, and each classification value warrants a different security level.
- Appropriate markings enable staff to recognize the need to protect classified data.

### 8.7.2 Examples of Classification

The U.S. government uses a hierarchical series of classifications that include Unclassified, Restricted, Confidential, Secret, and Top Secret, all of which are well known and standardized. The private sector (i.e., companies) uses various categories, such as public (low), private (medium), and confidential (high), which are less well known and not standardized.

These types of categories create issues for the private sector. For example, when employees change jobs, their new employers might value "private" above "confidential," but in their old jobs, their employers valued "private" below "confidential," which makes these classifications confusing. Even more confusing is when this happens within different departments or divisions within the same company. Part of a security professional's job is to identify these inconsistencies and make recommendations to correct them.

> **NOTE:** Compartmentalized information is data that requires special authorization beyond the normal classification system. Therefore, it is important that the procedures include steps to properly handle this type of information.

### 8.7.3 Classification Procedures

Classification procedures are critical to effective data classification. Thus, before implementing these procedures, it's vital that you first determine their scope and process. Classification scope determines what data to classify, whereas classification process determines how to handle classified data. You must label and mark all resources properly. Moreover, adhering to strong procedures will ensure that the organization is ready for any upcoming audits.

To determine the scope of a classification plan, you should conduct a business impact analysis to evaluate all of the organization's data. This type of analysis identifies resources, including data, that are important to carrying out critical business functions. Data value is determined according to the following:

- Exclusive possession (trade secrets and intellectual property)
- Utility (usefulness)
- Cost to create or re-create the data
- Liability (protection regulations)
- Convertibility/negotiability (financial information)
- Operational impact (if data is unavailable)
- Threats to the information
- Risks

You initially use the results of the business impact analysis to identify the necessary number of classification levels, the titles of which you will standardize for use throughout the organization. Send this information to the information owners responsible for assigning the initial classifications. These classifiers must understand the related regulations, customer expectations, and business concerns. The goal is to achieve a consistent approach to handling classified information. Therefore, it may be useful to create a training program to instruct the classifiers how to handle all data in a consistent manner.

The owners are also responsible for conducting a periodic review of classifications to ensure they are still current, particularly any time legislators or regulators introduce new government regulations. Finally, the owners are responsible for declassifying information that no longer requires special handling. Government organizations often handle declassification by declaring information automatically declassified after a certain number of years.

You must mark all media containing sensitive information according to the organization's classification policy and procedures, which is the only way personnel will know what special handling measures to use. You should label removable media both electronically and with simple physical labels; documents in hard-copy form require labels externally on the cover and internally on the pages.

### 8.7.4 Assurance

Internal and external auditors should review the organization's information-classification status as a component of their regular audit process, as well as evaluating the level of compliance with the classification policy and procedures, to ensure that all parts of the organization adhere to the process. This review might reveal situations in which information is overclassified.

Information security personnel should regularly visit workstations and other areas where users might leave unprotected classified materials. They also should make sure that, when violations occur, they submit appropriate reports to supervisors and managers. Ideally, to help staff understand the importance of handling classified materials, employee performance evaluations should include any instances when employees mishandled information. The organization should consider implementing a clean desk/clear screen policy, which states that users must never leave sensitive information in plain view on an unattended desk or workstation.

## 8.8 Configuration Management

One constant you can always depend on in information system environments is change, because it is unusual for any component in a networked computer environment to remain unchanged for a long period. Organizations commonly modify the hardware, software, firmware, documentation, test plans, and test documentation of automated systems throughout the SLC. Because uncontrolled configuration changes often result in conflicts and even new security vulnerabilities, it's important that all configuration changes occur only within a controlled process, which is called **configuration management**.

From the perspective of a security professional, configuration management evaluates the impact a modification might have on security. Will it affect the confidentiality, integrity, or availability of the system, application, or documentation? In this context, the job of the security professional is twofold:

- Be sure to adequately review all system changes before approval or implementation.
- Ensure that the change to the configuration will not cause unintended consequences for security; that is, the changes will affect the environment as expected and the environment will operate as authorized.

### 8.8.1 Hardware Inventory and Configuration Chart

A serious gap in a security program exists when organizations lack a hardware inventory that tells them what they currently have, who has ownership or possession of it, and which departments or systems are using it. In the event of a fire, equipment failure, or theft, this lack of documentation can slow the response and extend operational loss as well as making proper configuration management extremely difficult, if not impossible. A decision to roll out a new patch, service pack, or release will be complicated if you cannot find, update, and test every affected device.

> **NOTE:** One part of an effective configuration management plan is to use standard naming conventions for devices and components. A standard naming convention consists of well-defined labels that indicate a component's function and perhaps even location. Infrastructures that comprise components with standardized names are easier to manage without anyone's having to look up what each component does, and inventory lists are easier to decipher.

#### Hardware Configuration Chart

Having an up-to-date layout of the configuration of all hardware components is a necessity to help ensure that you configure all systems according to the baseline. It also ensures that you properly review the work completed on a system or network so that you can make the correct changes without bypassing any security features. A hardware configuration chart should include the following:

- An as-built diagram of the network, to help you plan the sequence of a change and see the ripple effects it might generate
- Copies of all software configurations so that you can examine changes and updates planned for one device in terms of their impact on other devices. These configurations should include those for items such as routers, switches, and firewalls. Stored copies of system and device configurations also make it easier to detect unauthorized configuration changes.

### 8.8.2 Patch and Service Pack Management

It is important to regularly check for any available vendor upgrades and service packs for all hardware and software in the environment, a process that may be quite involved when there are many types of software and hardware from different vendors. Such a process will be impossible, though, if the inventory list is incomplete. To address all known vulnerabilities, the organization must have a patch-management process to ensure that it rolls out patches to all computers and devices without causing system outages. Therefore, be sure to test every patch before rollout so that it will not disable other systems or functions.

## 8.9 The Change Management Process

It is common to discuss change and configuration control as a pair of activities, but they are really two ends of a spectrum. The confusion lies in where a particular activity crosses from one to another. Drawing a sharp line between the two is difficult because organizations of different complexities will draw the line in different places:

- **Configuration control** is the management of the baseline settings for a system device so that it meets security requirements. The settings must be implemented carefully and only with prior approval.
- **Change control** is the management of changes to the configuration. Unmanaged changes introduce risk because they might affect security operations or controls, and an improper change could even disable the system or equipment. Change control ensures that any changes to a production system are tested, documented, and approved. The change itself must follow a change control process that ensures that you make the change correctly and report it to management.

### 8.9.1 Change Control Management

Change control management is a planned approach to controlling change by involving all affected departments. Its objective is to maximize the benefits and minimize the risk of failure for all people involved in the change.

To be effective, change management should be multidisciplinary, touching all aspects of the organization. Nevertheless, an organization should not be so constrained by change management that it loses all flexibility in being able to adopt new technologies, improvements, and modifications.

A written policy approved by the chief information officer or the IT director and the business information security manager is necessary to define all roles, responsibilities, and procedures related to change management. Here are some important things to remember:

- You should communicate change management procedures and standards effectively. They should define the techniques and technologies you will use throughout the enterprise in support of the policy.
- Change management can be either reactive or proactive. Management's responding to external changes in the business environment is reactive change management, examples of which are changes in regulations, customer expectations, and the supply chain. With proactive change management, management initiates the change to achieve a desired goal. In this case, the source of the change is internal, such as the adoption of new technology.
- An organization can conduct change management in several ways: on a continuous basis, a regularly scheduled basis, or a release basis or when deemed necessary on a program-by-program basis.

### 8.9.2 Reviewing Changes for Potential Security Impact

Change creates risk for a business. It might circumvent established security features, result in outage or system failure, or require extensive retraining for employees to learn how to use the new systems. Because of the risk involved, you must include security personnel in the change control process.

The formal change control process should protect the integrity of the IT systems and ensure that all changes in the production environment are properly tested, scheduled, and communicated. Members of the change control committee attend meetings and forums to estimate, plan, review, and prepare for the organization's production environment.

### 8.9.3 Change Control Committees

A senior manager or business-process owner should lead a **change control committee**, whose responsibility is to oversee all proposed changes to systems and networks. The committee approves changes and the schedule for implementing the changes. In this manner, you cannot make changes to a system, application, or network without the proper review, funding, and documentation.

In cooperation with IT, the change control committee—in some cases called a change control board—provides the oversight to protect the computing resources and the data contained within those applications and databases. As part of the change process, key members meet with counterparts from the IT organizations to review upcoming plans and ensure that you properly evaluated all changes and the necessary security controls have been applied and evaluated. They then communicate their findings to all parts of the organization.

In brief, the primary objectives of the change control committee are to ensure all changes are as follows:

- Properly tested
- Authorized
- Scheduled
- Communicated
- Documented

Using rigorous change control makes it easy to identify recent changes that might have caused a production problem, which simplifies the problem's root cause and resolution processes and helps make the environment more secure.

### 8.9.4 Change Control Procedures

Change control procedures ensure that a change does not happen without following the right steps. Following procedures helps you avoid problems such as scope creep, which allows unauthorized changes to sneak into a system, and those caused by lack of oversight, lack of testing, or making changes without proper authorization. Figure 8-5 shows a sequence of change control procedures.

![[Pasted image 20260303105917.png]]
**Figure 8-5** Change control procedures.

1. **Request**—In the request stage, you should describe all proposed changes in writing and submit the change request to the change control committee for review. You should never make a change to a system without approval.
2. **Impact assessment**—The impact assessment stage evaluates the effect of the change on the budget, resources, and security of the system or project.
3. **Approval**—The approval (or, in some cases, disapproval) stage is the formal review and acceptance (or rejection) of the change by the change control committee.
4. **Build/test**—The build/test stage is the actual development or building of the change according to the approved change document. To ensure that the change does not cause unexpected problems for other systems or components, you must test it, which might include regression testing and an in-depth review of the security of the modified product.
5. **Implement**—Once you test the change and approve it for release, you can schedule the installation process. This is the stage in which adequate separation of duties ensures that no one person can make the change without proper review and oversight. The final hurdle is notifying management that you have made the change successfully.
6. **Monitor**—In this stage, you must monitor all systems to ensure that the system, program, network, and other resources are working correctly. You should address any user issues or requests using the organization's problem resolution procedures. Monitoring might identify the need for future changes, which then restarts the change control process.

### 8.9.5 Change Control Issues

Solid change control procedures include the components that tend to identify issues and provide recovery avenues if needed. A successful change control program should include the following elements to ensure the quality of the change control process:

- **Peer review**—This review ensures that a peer or another expert double-checks all changes before you put them into production. Peers can often catch problems before they make it to the testing phase.
- **Back-out plans**—These plans ensure that if the change does not work properly, a process exists to restore the system to a known good condition. Despite the best control procedures, you may accidentally release changes that have unintended effects. Therefore, it is important to know how to undo, or back out of, a destructive change.
- **Documentation**—You must keep documentation current to reflect the system's true design, and you should keep backup copies offsite. Documentation is necessary to understand how the system is supposed to operate.

## 8.10 Application Software Security

One critical area of security concern is application software because secure software can be difficult to design and write and even more difficult to deploy securely. Attackers know that the software development process is complex and that the result of the process is often an application that contains weaknesses, which they can exploit. Therefore, developing and deploying software require attention to security at every stage of the process as well as a structured process to ensure that the software does just what it is supposed to do. To describe and control systems and software development processes, there are several popular methods, two of which are the **system life cycle (SLC)** and the **system development life cycle (SDLC)** . The steps in these processes are very similar except that the SLC includes operations and disposal and the SDLC ends with the transition to production.

For some organizations, maintenance and new development are done by developers, making them part of SDLC. For others, specialized maintenance teams handle maintenance and development, making them part of SLC. More and more organizations use the term SDLC to describe the entire change and maintenance process for application and system software.

### 8.10.1 The System Life Cycle

This section covers the common steps used in the SLC. The more the security professional can be involved in each step, the more likely the system will include the needed security from the start. The main justification for SLC—and for building in security at the start—is to reduce or avoid cost:

- Consumers of commercial software products will see lower costs because you will need to deliver fewer patches and fixes. In addition, there will be fewer losses due to weaknesses in the software that attackers can find and exploit.
- Vendors of commercial software will see lower costs because they require smaller support staffs and have lower warranty and product maintenance costs.

The common steps used in the SLC are as follows:

1. **Project initiation and planning**—One of the first requirements of a successful project is to have all the necessary resources available. The resources required should represent the areas that you need to consider and integrate into the project. Your role is to provide advice on building security into the project from the very beginning, which includes project budgets, system design, maintenance, and the project timeline. You should address threats, vulnerabilities, risks, and controls here first.

2. **Functional requirements and definition**—This is the "what-if?" phase. Always state requirements using positive terms: The program must handle this data or perform that function. You must consider what the program should or will do when the data does not meet the specifications. What happens when the software receives unexpected input? Are there too many characters? Are fields missing? Are users seeing delayed transmissions? Failure to consider these factors creates a great number of security mishaps.

3. **System design specification**—In this phase, a project is broken into functions and modules, which requires that you consider the type of hardware on which the system is going to run. Security issues here include physical security of the hardware and network, as well as accounting for all the possible platforms. It is not enough to say the project is limited to Linux or Windows, for example. Each platform features a wide variety of versions and runs on an almost infinite combination of peripherals, chipsets, and drivers.

4. **Build (develop) and document**—Coding standards should include standard libraries of function calls as well as industry-standard solutions for items such as cryptography, hashing, and access control. You need to secure code in development so that only developers have access and only on a need-to-know basis. You should securely store copies in either printed or machine-readable form, such as on CDs or USB memory sticks, so they are not left lying around.

5. **Acceptance testing**—During the functional design stage, you should create a test plan that must include testing to make sure the new programs provide the necessary security and, where applicable, privacy. Moreover, the people responsible for the tests should not be the developers, and past-due delivery dates for developers should not affect the time allotted for testing.

6. **Implementation (transition to production)** —During this transition, developers will be working on delivery of training and assistance to users and help-desk personnel. Security features need to be carefully explained to both groups. In some organizations, developers also will help manage the turnover of code to maintenance staff.

7. **Operations and maintenance**—When there are problems with the system, it's likely that maintenance, operations, and help-desk personnel will be the first to know. They need to track the issues that come in and be ready to report their results to management. This procedure fuels the change management process. These personnel require training to understand the differences between a request for change, a software malfunction, and a security weakness or breach as well as how to handle each of those events.

8. **Disposal**—Over time, component parts will reach the end of their life span or you will need to upgrade a backup system or procure a larger disk to replace a smaller one. You should ensure that you have procedures to sanitize the media and then dispose of it in a cost-effective way. In years past, organizations would wipe a disk and resell it. Today, the value of a small used disk is often less than the cost to securely wipe it with a tool such as DBAN and then simply dispose of the disk.

### 8.10.2 Testing Application Software

Security professionals often help test new systems or upgrades to existing systems. These tests should be thorough enough to ensure that you test for all expected and unexpected actions and that you handle errors correctly. You should also perform tests to verify the maximum load on the system, including transaction volume, memory allocation, network bandwidth, and response times. If you use production or sensitive data in testing, make sure you take steps to keep those data secure.

Because input validation attacks are so common, security personnel should work with software testing personnel to make sure tests catch any input vulnerabilities. One type of testing for input vulnerabilities is called fuzzing, which is the practice of providing random input to software to see how it handles unexpected data. Fuzzing can help identify input vulnerabilities better than testers trying to think of bad input.

### 8.10.3 Systems Procurement

One common way new vulnerabilities make their way into an environment is through a change that causes unintended side effects. Therefore, you should thoroughly evaluate any change to an environment to ensure that it does not introduce new vulnerabilities, and this includes new hardware and software as well. Procuring new equipment is a critical role of the security professional, but doing so can decrease overall security if the process is not handled well. Any time you need to procure new equipment, you should carefully evaluate which products will meet the organization's requirements. To ensure that new equipment does not expose an environment to any new vulnerabilities, you must do the following:

- Evaluate the various solutions that are available
- Evaluate the vendors in terms of maintenance, support, and training
- Use the Common Criteria to ensure that you simplify the evaluation process
- Monitor vendor contracts and SLAs
- Correctly install equipment and formally accept it at the end of the project
- Follow the organization's procurement procedures to ensure a fair purchasing process
- Monitor systems and equipment to identify those that are reaching the end of their life span so that you can schedule them for replacement

### 8.10.4 The Common Criteria

Because procuring new equipment can lead to security vulnerabilities, formalizing the process makes sense. The need for a formal approach to evaluate systems and equipment gave rise to several sets of standards. The U.S. government created a series of computer security standards documents known as the Rainbow Series, so named because of the bold colors on the covers of the documents. The Red Book describes components of a trusted network infrastructure (TNI), and The Orange Book talks about maintaining access control and confidentiality in a classified system. Both books used a series of evaluative levels (C2, B3, and so on), and vendors had their products evaluated against these levels. The developers of the Rainbow Series formally called this classification system TCSEC.

Other governments created their own equivalents by starting with TCSEC and making modifications. Eventually, these systems merged into what became ITSEC. The governments of the United States, the United Kingdom, Canada, Germany, France, and the Netherlands used ITSEC as a starting point, and then they developed a new procurement standard called the Common Criteria.

The Common Criteria include a series of increasingly more difficult evaluation assurance levels (EALs) numbered from 1 (lowest) to 7 (highest). Evaluation labs are scattered worldwide. Leading vendors within an industry (e.g., vendors of firewalls) collectively create a standard, ideal, and perfect solution, and any vendor can have its product evaluated against that standard. An EAL rating assures that the vendor's claims match the collective standard to a defined level of testing and all the product's documentation, development, and performance match the evaluation claims.

> **TECHNICAL TIP:** The formal name for the Common Criteria is ISO/IEC 15408.

### 8.10.5 Data Policies

All data reaches its end of usefulness at some point, so what do you do when you no longer need or can use data? The answer is to simply follow the guidance in the organization's data policies, which of course means they must already be in place. Policies that cover data management should cover transitions throughout the data's life cycle and contain sections or even full documents that cover retention and storage as well as disposal.

Because data items vary in their lifetimes of usefulness, retention and storage sections of an organization's data policies should state how long to keep different types of data. If you need to keep historical data for research purposes, your policy should address how to store it. Your security policy should extend to cover stored data as well.

But what do you do when you no longer need data? One of two choices exist, either overwrite the data on the media to ready the media for reuse, which is a process called wiping, or destroy the media. Your choice depends on the usefulness of the media and the sensitivity of the data. For extremely sensitive data, the safer choice is to erase the data and destroy the media to keep it out of the hands of someone who may be able to recover all or part of the erased data.

Whenever you need to dispose of equipment, you should ensure that you dispose of it in a secure way so that you do not expose any confidential data. Several options are available to you, including the following:

- **Degaussing**—Applying a strong magnetic force to magnetic media usually makes all electronics unusable.
- **Physical destruction**—Physically destroying the media on which data is stored guarantees that you eliminate any confidential material.
- **Overwriting data**—Even though this option does not destroy the media, it is included here as a viable alternative to actual media destruction. Repeatedly overwriting data on media reduces the chance that any data can be recovered. However, the possibility remains that a determined person may be able to recover some of the overwritten data.

## 8.11 Certification and Accreditation

Between procurement and disposal, you will need to ensure that the components in the organization's computing environment are sufficient for your requirements. To do so, both certification and accreditation can be employed. **Certification** is the process of reviewing a system throughout its life cycle to ensure that it meets its specified security requirements, whereas **accreditation** is the formal agreement by the authorizing official to accept the risk of implementing the system. The accreditation process includes the following players:

- **Authorizing official (AO)** —The senior manager who must review the certification report and decide whether to approve the system for implementation. The AO officially acknowledges and accepts the risk that the system may pose to an agency's mission, assets, or individuals.
- **Certifier** —The individual or team that is responsible for performing the security test and evaluation (ST+E) for the system. The certifier also prepares the report for the AO on the system's operating risk.
- **System owner** —The person responsible for the daily operations of the system and ensuring that the system continues to operate in compliance with the conditions set out by the AO.

### 8.11.1 Certification

Certification is the process carried out by a certifier or team of certifiers of technically evaluating a system to provide assurance that the organization implemented the system correctly. The system should meet the initial design requirements to ensure that the security controls are working effectively. The certifier should have the skill to perform the verification process and the tests necessary to prove compliance. Certification of a system means the following:

- The system meets the technical requirements.
- The system meets the functional requirements.
- The system provides assurance of proper operation.

To certify a system, the person (or people) involved in the process must know the technical and functional requirements as well as the capabilities of the system they are recommending for purchase or for approval to move into production. These requirements might be related to either software or hardware. The certifiers might evaluate the systems in terms of quantity or quality, such as the ability to authenticate 100 users a minute or to ensure 99.99 percent uptime, or review non-IT factors, such as weight or energy consumption. The accreditors must examine all the requirements. Whether conducting or managing these tasks, many of them will fall to the security professional.

Finally, the certifiers must assess each requirement to make sure the new system meets or exceeds each specification. When they are sure that it does, they recommend management approval. However, certification of equipment or software does not mean it is right for the organization or the best solution available. It means only that the product meets its technical and functional specifications and operates as promised.

### 8.11.2 Accreditation

Accreditation is the process of management's officially accepting the system after the completion of the certification process. The accreditor or designated approving authority reviews the certification reports and, based on the operational environment, accepts the system for operation. You can define this process in two ways:

- Accreditation is management's formal acceptance of risk.
- Accreditation is management's permission to implement.

### 8.11.3 Triggers for New Certification

The certification and accreditation processes ensure that a system not only meets the security requirements today but that it continues to meet them through the operations and maintenance phases of its life cycle. The post-accreditation phase lists the activities required to continue to operate and manage the system so that it maintains an acceptable level of risk. You must continually assess risk to meet this requirement for the following reasons:

- The business must change due to new products, new processes, mergers, or divestitures.
- Products (solutions) that were once accredited might no longer meet the needs of the business.
- Vendors often upgrade or replace products, and these replacements need to be recertified and reaccredited.

## 8.12 Software Development and Security

You learned earlier in this chapter about the importance of developing secure software and that software development requires special attention from a security perspective. Applications represent the most common avenue for users, customers, and attackers to access data, which means you must build the software to enforce the security policy and to ensure compliance with regulations, including the privacy and integrity of both data and system processes. Regardless of the development model an organization adopts, the application must properly perform the following tasks:

- Checks user authentication to the application
- Checks user authorization (privilege level)
- Has procedures for recovering database integrity in the event of system failure
- Handles errors and exceptions consistently with standard responses and does not allow any error or exception to go unhandled because unhandled exceptions can reduce an application's security. Gives consistent error responses and provides clear explanations and instructions to empower users to make the right choices.
- Validates all input (i.e., never accepts any input from a source without validating it first). If the data fails validation, throw it away; do not try to sanitize it. Because attackers can often change data as it travels from a client to a server, validating it on both the client and the server is the only way to be sure that the data is valid. Some attacks that depend on weak validation include the following:

  - **Cross-site scripting (XSS)** —This is an attack in which an attacker inputs client-side script code to a web application. The code would then be viewed by other users, and their client software would execute the script instructions. The XSS attack exploits the trust users have for a server.
  
  - **Cross-site request forgery (XSRF)** —Similar to the XSS attack, an attacker provides script code that causes a trusted user who views the input script to send malicious commands to a web server. The XSRF attack exploits the trust a server has in a user.
  
  - **Structured Query Language (SQL) injection** —This is an attack technique in which an attacker provides malicious SQL statements to access unauthorized data or carry out unauthorized commands.

> **TECHNICAL TIP:** You may recognize SQL injection as a common attack. According to the Open Web Application Security Project (www.owasp.org), SQL injection vulnerability is one of the most common recurring vulnerabilities in web applications. Growing databases and a need for faster data have led to a growth in nonrelational databases, called NoSQL databases. Although NoSQL databases are not specifically vulnerable to SQL injection attacks, that does not mean you should consider them any more secure than SQL-based databases. Even NoSQL databases are vulnerable to injection attacks.

- Defines secure configuration baselines. When released to end users, the application provides a documented set of configuration settings that define a secure baseline, or starting point.
- Provides guidance on hardening the application. In addition to providing a secure baseline, the application should offer guidance on changing configuration settings that will keep the application secure as well as guidance on further configuration settings or the addition of external controls that will increase the application's security.
- Provides and applies frequent patches. Ensure that you apply the latest security patches for the particular environment. The application should also provide frequent security patches to the users of the application, along with a convenient method of applying patches and managing the patching process.

Software developed in-house will have source code, object code, and runtime executables, all of which you need to manage and protect with policies, standards, and procedures. For example:

- You should protect source code from access by unauthorized users.
- You should track changes to source code by version control systems so that rollback to a previous version is error free.
- Programmers should not be able to update production systems directly (programmers should only be able to promote changes to a test environment, and then another person is required to promote those changes from the test environment to production).

### 8.12.1 Software Development Models

Secure software development requires a formal model for creating and modifying software. This process is known as the software development life cycle, or SDLC, which uses industry best practices to guide software development activities as projects with specific start and end dates and a set of required deliverables. At this time, the two most widely accepted models for software development include the following:

- **The waterfall model**—Based on traditional project management practices in which extensive planning precedes any development. Progress through a project moves forward along a well-defined path.
- **Agile development method**—A newer family of project management approaches that depend on very short sprints of activity. Agile works well in very dynamic environments where requirements change and are often revisited.

#### Waterfall Model

Many current software development methods base their models on the **waterfall model**, which is illustrated in Figure 8-6. This is a sequential process for developing software and includes the SDLC and the SLC you learned about earlier. In the waterfall model, progress flows downward, like a waterfall. The essence of the waterfall model is that no phase begins until the previous phase has been completed. The phases are as follows:

1. Requirements specification
2. Design
3. Construction
4. Integration
5. Testing and debugging
6. Installation
7. Maintenance

![[Pasted image 20260303110239.png]]
**Figure 8-6** The waterfall model.

The basic waterfall model originated in the manufacturing and construction industries and is a feature of highly structured physical environments in which late revisions are very costly, if not entirely cost prohibitive. When Winston W. Royce devised this model in 1970, no formal software development methods existed, so he adapted this hardware-oriented model to software development.

Because of perceived shortcomings of the Royce model, you will find modifications of the waterfall model. Most software development models use at least some phases similar to the waterfall model. The importance of the model is in its focus on ensuring that each phase is complete before moving to the next phase. Though this may be quite difficult in large development environments, always invest the time to properly plan and design software. Do not just start writing programs.

#### Agile Software Development

Traditional software development management is still based largely on some variation of the waterfall method. During the 1990s, some organizations began to realize that the software industry was changing in different ways. Increasing demands to develop more complex software more efficiently led to new methods of managing software development. Instead of managing large projects with long delivery schedules, many organizations looked for ways to be more responsive, so they chose to develop their software in smaller pieces. This move toward smaller development cycles eventually became known as the **agile development** method.

Agile loosely describes a method of developing software that is based on small project iterations, or **sprints**, instead of long project schedules. Organizations that use agile produce smaller deliverables more frequently and can evaluate a large project in terms of its individual pieces as they are completed. Sprints are generally one to four weeks in duration, which means there is some deliverable at least once each month. This focus on frequent delivery makes it possible to see and use pieces of a large software product as it matures over time.

The first organized meeting of agile enthusiasts was in 2001. Several organizations that were exploring this new type of software development sent representatives to a meeting in Snowbird, Utah, to collaborate and exchange ideas. The attendees created the foundational document of the agile movement—the Manifesto for Agile Software Development—which is a concise document that reflects its writers' affection for simple methods.

Here is the Manifesto for Agile Software Development (https://agilemanifesto.org/) in its entirety:

> We are uncovering better ways of developing software by doing it and helping others do it. Through this work we have come to value:
>
> **Individuals and interactions** over processes and tools
>
> **Working software** over comprehensive documentation
>
> **Customer collaboration** over contract negotiation
>
> **Responding to change** over following a plan
>
> That is, while there is value in the items on the right, we value the items on the left more.

Figure 8-7 shows the basic idea behind the agile method. Unlike the waterfall method, agile is designed to be iterative. Each time around the cycle is a single sprint, and many sprints are needed to create a complete software project. Each sprint ends at a specific point in time and should have a deliverable, which should be something such as working software that the team can demonstrate. The focus on working software helps focus the team on results.

![[Pasted image 20260303110315.png]]
**Figure 8-7** The agile software development method.

Agile is a popular technique of managing software development projects and tends to perform well in organizations that encourage ongoing communication and value short development cycles. It is important to begin developing software with security in mind from the very beginning. Agile methods encourage developers to plan for security and then test for security at the end of each sprint. Developing secure software can become an integral part of the overall development effort, that is, if the organization values and encourages security. Regardless of the development method an organization uses, attention to security is more important than any method.

> **NOTE:** You can find more information on the Manifesto for Agile Software Development and the agile method in general at https://agilemanifesto.org. Another good starting point to learn about agile is www.agilealliance.org/agile101/.

## Chapter Summary

In this chapter, you learned that security professionals must understand that security operations and administration are the basis of any solid security program and how security administration works to plan, design, implement, and monitor an organization's security plan. You learned that professional ethics are essential for every solid security plan and what you have to do to make sure a security program is compliant. You learned how the policies, standards, guidelines, and procedures of a plan work together to shape a security program and how data classification standards affect the decision-making process. You learned how to use configuration management to manage system modifications and how configuration control and change control affect the change management process. You explored the eight common steps of the SLC and the SDLC and how these steps reduce costs. Finally, you learned why software development methods require special security considerations and how user awareness is pivotal to the success of a security program.

## Key Concepts and Terms

| Term | Definition |
| :--- | :--- |
| **Accreditation** | The formal agreement by the authorizing official to accept the risk of implementing the system |
| **Agile development** | A software development method based on small project iterations called sprints |
| **Baseline** | A documented minimum level of security configuration |
| **Certification** | The process of reviewing a system to ensure it meets security requirements |
| **Change control** | The management of changes to system configurations |
| **Change control committee** | A group that oversees all proposed changes to systems and networks |
| **Compliance liaison** | An individual responsible for ensuring personnel comply with policies |
| **Configuration control** | The management of baseline settings for system devices |
| **Event log** | Records of actions created by operating systems or applications |
| **Functional policy** | Policy addressing specific functional areas like email or remote access |
| **Guideline** | Recommended actions to provide structure to a security program |
| **Internet Architecture Board (IAB)** | Organization that published RFC 1087 on Internet ethics |
| **Job rotation** | Moving employees among various duties to prevent collusion |
| **Least privilege** | Limiting access based on permissions needed to perform duties |
| **Mandatory vacation** | Required time off to detect potential fraud |
| **Need to know** | Access restricted to information required for job performance |
| **Privacy policy** | Policy specifying how an organization collects and uses personal information |
| **Procedure** | Step-by-step systematic actions to accomplish security objectives |
| **Remediation** | Fixing security vulnerabilities |
| **Security administration** | The group responsible for planning and monitoring security |
| **Security operations center (SOC)** | Physical location where security administration occurs |
| **Separation of duties** | Breaking tasks into subtasks performed by different users |
| **Sprint** | A short development cycle in agile methodology |
| **Standard** | Mandated requirements for hardware and software solutions |
| **System development life cycle (SDLC)** | Process for developing and modifying software |
| **System life cycle (SLC)** | Process including operations and disposal of systems |
| **Waterfall model** | Sequential software development process |

