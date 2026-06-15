# **CHAPTER 5: Access Controls**

## **Lesson Overview**

Access controls are the fundamental mechanisms that safeguard resources—both physical and digital—from unauthorized use. They form the cornerstone of information security by determining who can interact with what resources and in what manner. This chapter delves into the core principles, models, and technologies of access control systems. We will explore the complete cycle of access management, from identifying a user to holding them accountable for their actions. You will learn about various authentication methods, formal security models that guide system design, and the practical challenges of implementing controls in modern environments like cloud computing. Understanding access controls is essential for designing secure systems, enforcing security policies, and protecting sensitive data from threats.

## **Learning Objectives**
Upon completing this chapter, you will be able to:
1.  **Define** the core concepts, components, and technologies of access control systems.
2.  **Describe** the formal models of access control (e.g., DAC, MAC, RBAC) and their applications in protecting confidentiality and integrity.
3.  **Explain** how identity is managed through the processes of identification, authentication, authorization, and accountability.
4.  **Contrast** the concepts of recognition (identification) and authentication.
5.  **Develop** and **maintain** effective system access controls, including policies for credentials, permissions, and monitoring.

**ACCESS CONTROLS** are methods used to restrict or allow access to certain items, such as automobiles, homes, office buildings, computers, and even a smartphone. Your first experience with access controls might have been as a child when you locked a sibling out of your room or used a locker at school. Similarly, the key to your car fits only your car so that only you can unlock and start it. The same is true of your house or apartment. You might be one of the many people who also use a special code to unlock your smartphone or tablet so no one can unlock the secured device without the code. Or maybe you cannot view certain channels on your television or even retrieve your voicemail messages without a security code.

Thus, **access control** is the process of protecting resources so that they are used only by those allowed to use them in order to protect resources from unauthorized use or a threat. Just as the lock-and-key systems for a house or car are access controls, so are the personal identification numbers (PINs) on a bank or credit card.

Businesses use access controls to manage what their personnel can and cannot do, including who users (people or computer processes) are, what users can do, which resources they can interact with, and what operations they can perform. Access can be granted to physical assets, such as buildings or rooms, or to computer systems and data. To achieve this goal, access control systems use several methods, including passwords, hardware tokens, biometrics, and certificates.

### **Chapter 5 Topics**
This chapter covers the following topics and concepts:
* What the four parts of access control are
* What the two types of access control are
* How to define an authorization policy
* What identification methods and guidelines are
* What authentication processes and requirements are
* How recognition and authentication differ
* What accountability policies and procedures are
* What formal models of access control are
* What threats there are to access controls
* What some effects of access control violations are
* What centralized and decentralized access controls are

### **Chapter 5 Goals**
When you complete this chapter, you will be able to:
* Define access control concepts and technologies
* Describe the formal models of access control
* Describe how identity is managed by access control
* Contrast recognition and authentication
* Develop and maintain system access controls

## **Four-Part Access Control**
Before an asset can be protected, the entity wishing to protect the asset must know some information about the intended user and how that user should be allowed to interact with the asset. The four parts of access control provide this information along with the assurance that access is sufficiently managed:

1.  **Identification**: Who is asking to access the asset? ==who is asking to access this asset?==
2.  **Authentication**—Are the requestors’ identities verified to be the claimed identities (i.e., are the users who they claim to be)? 
3.  **Authorization**: What, exactly, can the requestors access? And what can they do?
4.  **Accountability**: How can actions be traced to an individual? ==It is important to be able to identify a person who accesses or makes changes to data or systems for later reporting and research purposes, which is a process known as **accountability.**==

![[Pasted image 20251201193207.png]]

The preceding four parts are divided into two phases:
*   **Policy definition phase** The authorization definition process operates in this phase to determine who has access and what systems or resources they can use.
*   **Policy enforcement phase** The identification, authentication, authorization execution, and accountability processes operate in this phase to grant or reject requests for access based on the authorizations defined in the first phase.

## **Two Types of Access Controls**
Access controls generally fall into one of two categories:
*   **Physical access controls**: Control access to physical resources, such as buildings, parking lots, and protected areas. For example, a key to the door of an office controls the physical access to that office.
*   **Logical access controls**: Control access to a computer system or network. As an example, a username and password allow personnel to use an organization’s computer system and network resources.

>**NOTE** Sometimes the difference between access control and access controls can be confusing. Just remember that access control is something that is done to protect resources, whereas the way to protect resources from unauthorized access is by using different types of access controls.

### **Physical Access Control**
An organization’s facilities manager is often responsible for physical access control, meaning access to physical resources, which might be enabled through a security card (also known as a smart card) programmed with an employee’s ID number. Employees might need to swipe this card through a card reader to open a gate to the parking lot, send an elevator to the appropriate floor, or unlock a door leading to an office. The organization’s authorization policy is what determines who is allowed physical access and to what places. Without this authorization, here, in the form of a security card, people would not get past the front gate. Moreover, if an organization shares its office building with other organizations, authorized personnel might even have a second card that grants access into the building after hours.

![[Pasted image 20251201193345.png]]

### **Logical Access Control**
Security administrators use logical access controls to decide who can get into a system and what tasks they can perform, as does a system manager, to influence how staff personnel use a system. Examples of system controls for a human resources (HR) system include the following:

*   Deciding which users can log into a system HR employees may be the only employees who are allowed to reach sensitive information stored on an HR server.
*   Monitoring what the user does in that system Certain HR employees might be allowed to only view documents, whereas other HR employees might be able to both view and edit those documents.
*   Restraining or influencing the user’s behavior on that system An HR staffer who repeatedly tries to view restricted information might be denied access to the entire system.

## **The Security Kernel**
The **security kernel** is the central part of a computing environment’s hardware, software, and firmware that enforces access control for computer systems. It provides a central point of access control, implements the reference monitor concept, and mediates all access requests and permits access only when the appropriate rules or conditions are met. Following are the steps the security kernel takes in enforcing access control:

1.  The subject (a user) requests access to an object (an asset). The security kernel then intercepts the request.
2.  The security kernel refers to its rules base, also known as the security kernel database. It uses these rules in this database to determine access rights, which are set according to the policies the organization has defined.
3.  The kernel allows or denies access based on the defined access rules.

All access requests handled by the system are logged for later tracking and analysis.

![[Pasted image 20251201184309.png]]

It is easy to see that the overall security of any system’s access control depends on the security of the operating system. Most of the popular computer operating systems (e.g., Windows®, Linux®/UNIX®, and macOS®) provide extensive security features, which allow administrators to create very secure systems. However, the popular operating systems for many mobile devices (e.g., Android™ and iOS®) lack some of these security features, which is justified by the argument that mobile devices do not need the same level of security features as servers or full-featured client computers. However, as mobile devices become more powerful and ubiquitous, the need for tighter security increases. Furthermore, the rapid rise in the number of Internet of Things (IoT) devices makes it clear that even unattended devices, such as doorbells and refrigerators, are targets for attackers and need stronger security as well. Even though most operating systems provide extensive security guarantees, some computing environments need even more, such as systems that handle extremely sensitive information (e.g., classified information on government servers); therefore, several operating systems have included supplemental controls to address the additional security needs of such systems. These operating systems, referred to as trusted operating systems (TOS), provide features that satisfy specific government requirements for security. One of the most widely used set of criteria for TOS design is the **Common Criteria for Information Technology Security Evaluation (Common Criteria)**, which you will read about later in this chapter.

## **Access Control Policies**
An **access control policy** is a set of rules that allows a specific group of users to perform a specific set of actions on a specific set of resources. If users are not authorized, they do not have access to system functions or system resources. Access control policies are important to reduce and control security risks, and both automated processes and humans must adhere to them.

To manage access control policies well, you must understand their four central components:
*   **Users**—Users are the people who use the system or processes that perform some service for other people or processes. A more general term for users is *subjects*.
*   **Resources**—Resources are the protected objects in the system. They can be accessed only by authorized subjects and used only in authorized ways.
*   **Actions**—Activities that authorized users can perform on the resources.
*   **Relationships**—Relationships are optional conditions that exist between users and resources. They are permissions granted to an authorized user, such as read, write, and execute.

### **Authorization Policies**
The first step toward controlling access is to create a policy that defines authorization rules. **Authorization** is the process of deciding who has access to which computer and network resources. In most organizations, authorization is based on job roles, background screening, and any government requirements. These conditions or policies are decided primarily by either a group membership policy or an authority-level policy.

The most detailed authorization policy is based on individual users. In this type of policy, each user has specific assigned privileges, which allow administrators to define approved resource access at a very detailed level. However, maintaining a user-based authentication approach is very difficult because it requires a lot of administration time to stay current.

In a *group membership policy*, authorization is defined by what group(s) users are in, which reduces the administrator’s workload by grouping similar users together. For example, perhaps only the security cards of members of the IT department give access to the room where computer equipment is stored. If personnel are not members of this IT group, their security card does not let them enter this room to retrieve a new monitor. If they want to access the computer equipment storage room, they must first contact the IT department, which likely assigns a member of the IT group to help them.

In an *authority-level policy*, users need a higher degree of authority to access certain resources. For example, perhaps only a senior-level member of the IT group has permission to enter the room that houses servers, which makes sense, because servers are often more valuable than computer monitors.

## **Methods and Guidelines for Identification**

Once you define authorization rules in an authorization policy, you can enforce the rules. Each time a user requests access to a resource, the access controls either grant or deny access based on the authorization policy.

The first step in enforcing an authorization policy is to determine the identity of the subject, which is a process called **identification**. This process allows a subject, which can be a user, a process, or some other entity, to claim to be a specific identity. Several methods are commonly used to identify subjects, and the chosen method depends on the security requirements and capabilities of the computing environment. The next section covers various methods and guidelines for how a subject identifies itself to a system.

### **Identification Methods**

The most common method to identify a user to a system is a username, which can be in the form of a user ID, an account number, or some other assigned identifier. Some applications identify a user using a smart card, which often looks like a plastic credit card. Smart cards make it easy for subjects to provide complex identification credentials without having to remember them. Just as you might slide your credit card through an electronic card reader to make a purchase, you can swipe a smart card through card readers, which grant access to such things as parking facilities, buildings, and rooms.

Another access control method for identifying subjects is **biometrics**, which can be used to recognize humans based on one or more physical or behavioral traits or to validate identities. Examples of biometrics include fingerprints, face or voice recognition, DNA matching, handwriting, retina scans, and even the way a person types.

### **Identification Guidelines**

To ensure that all actions carried out in a computer system can be associated with a specific user, each user must have a unique identifier. The guarantee that every action is associated with a unique identity is called *nonrepudiation*, which means that it is important for each user to have a unique user account. An account policy should prohibit generic accounts and user account sharing and include unique identifiers (IDs) for distinguishing between multiple users with the same name. The process of associating an action with a user for later reporting or analysis is called *accounting*, which, when done properly, must include nonrepudiation.

Moreover, the data used to identify subjects should be kept current and closely monitored; the IDs of users who leave the organization or who are inactive for an extended time, disabled; and standard naming conventions, which should not relate to job functions, applied. The process for issuing, managing, and retiring IDs should be documented and secure.

## **Processes and Requirements for Authentication**

So far in this chapter, you have learned about methods to define authorization rules and identify users. The next step is **authentication**. In this part of access control, users validate, or prove, the identity they claimed during identification. Authentication answers the question, are subjects who they claim to be? Because anyone can claim to be any identity, authentication verifies that the subject requesting access is really the claimed identity (authentic) and the same subject who has been granted access. Without authentication, you could never really know if subjects are who they say claim to be.

### **Authentication Types**
Following are the seven types of authentication:
1.  **Knowledge** → Something you (the user) know, such as a password, passphrase, or PIN.
2.  **Ownership** → Something you have, such as a smart card, key, badge, or token.
3.  **Characteristics** → Some attribute that is unique to you, such as your fingerprints, retina, or signature. Since the characteristics involved are often physical, this type of authentication is sometimes defined as *something you are*.
4.  **Action/performance** → Some action that you can perform, such as reproducing a signature, sometimes defined as *something you can do*.
5.  **Behavior** → Some observable trait or behavior that is unique to you, sometimes defined as *something you exhibit*.
6.  **Location** → Somewhere you are, such as your physical location when attempting to access a resource.
7.  **Relationship** → A trusted individual with whom you have a relationship, encouraging trust by association, sometimes defined as *someone you know*.


> A combination of username and password is considered single-factor authentication even though it appears to require two steps. The username satisfies the identification step, and the password satisfies the authentication step. Using a single type of authentication may not be adequate for access to more sensitive systems, applications, or data, in which case, two-factor or multifactor authentication might be required, such as swiping a card (something you have) to enter a building and then typing a PIN (something you know) to ensure the security of a valuable resource.

The use of controls from only one category is known as *single-factor authentication*. However, because each type of authentication can easily be compromised on its own, systems that contain sensitive or critical information should use at least two authentication types, which is called *two-factor authentication (2FA)*, or **multifactor authentication (MFA)**, to provide a higher level of security than using only one.

### **Authentication by Knowledge**

Authentication by knowledge is based on something you (the user) know, such as a password, passphrase, or PIN. Passwords are the oldest and most common method of authentication for computer systems as well as being the weakest; therefore, they should not be used alone to protect valuable resources. Moreover, as the value of a resource increases, so should the strength of the access controls protecting it, which makes MFA a requirement for protecting access to valuable resources.

Because of their simplicity and popularity, passwords are common targets of cyberattacks. The most often used are brute-force and dictionary attacks, which can easily crack weak passwords, such as those that are very short or contain dictionary words.
*   A *brute-force attack* involves trying every possible combination of characters, whereas modern password crackers take a more effective approach. First, they measure the entropy (i.e., a measure of randomness) of characters and then test low-entropy, then medium-entropy, and finally high-entropy words.
*   A *dictionary password attack* works by hashing all the words in a list of possible passwords (often supplemented with suffixes such as 01, 02, 4u, and so on) and then comparing the hashed value with the system password file to discover a match. The prepared list of possible passwords is called a *dictionary*. Hackers are familiar with all the usual tricks, such as spelling a name backward or simple substitution of characters (e.g., 3 for *e*, 0 for *o*, $ for *s*, and so on).
*   Because most systems store a hash of the password, attackers first precompute these dictionary words and build a table, known as a *rainbow table*. Then, they look up the stored hashed version of the password in the table to discover the word that generated it. Rainbow tables are widely available. For example, AccessData’s forensic investigator’s tool, known as the Forensic Toolkit® (FTK®), features a rainbow table with a million words, which, according to FTK’s website, detects 28 percent of user passwords.


>A shorter password life span means more protection for the user because it lowers the chance that an attacker can compromise and use the password before it expires. To create stronger password controls for users, consider a 30-day password-change policy.

#### **Password Account Policies.**

In addition to encouraging password best practices, an account policy should include clear password requirements. Following is a list of suggested account policy password requirements (the specifics of these items should be customized for a particular organization).

**Complexity**
*   Passwords must contain at least eight alphanumeric characters.
*   Passwords must contain a combination of uppercase and lowercase letters and numbers.
*   Passwords must contain at least one special character within the first seven characters of the password.
*   Passwords must contain a nonnumeric letter or symbol in the first and last character positions.
*   Passwords must not contain the username.
*   Passwords must never include the name of the user or the names of any close friends or relatives.
*   Passwords must never use an employee’s ID number, Social Security number, birth date, telephone number, or any personal information that can easily be guessed.
*   Passwords must never include common words from an English dictionary (or a dictionary of another language with which the user is familiar).
*   Passwords must never employ commonly used proper names, including the name of any fictional character or place.
*   Passwords must never contain any simple pattern of letters or numbers, such as *qwertyxx*.

**Expiration.** Passwords that protect sensitive data expire every 90 days (30 days for highly sensitive accounts) and must be changed.

**Recovery.** Forgotten passwords can be recovered after providing alternate authentication credentials via the organization’s internal password recovery utility.

**Disablement.** User accounts will be disabled immediately when a user is no longer associated with the organization or no longer requires provided access.

**History.** Password history is stored, and users’ passwords cannot be changed to any of the 10 previous passwords that they have used.

#### **Account Lockout Policies.**

Many systems are configured to disable a user ID after a certain number of consecutive failed logon attempts, often three to five attempts. The number of failed logon attempts that trigger an account action is called the *threshold*. The user may be locked out for a few minutes, a few hours, or until the account is reset by a security administrator. This practice helps guard against attacks in which the attackers make several attempts to guess a password, but it also enables an intruder to lock out users, which is a form of denial of service (DoS) attack, by entering groups of incorrect passwords.

#### **Audit Logon Events.**

One method of keeping track of who is accessing a computing environment is to audit logon events, a practice that provides a record of when every user logs on or off a computer. If an unauthorized user steals a user’s password and logs on to a computer, you can determine when that security breach occurred. When you audit failure events in the logon event category (also known as ***failure auditing***), you can see whether the failure event was due to unauthorized users or attackers attempting to log on to a computer or system, the latter of which is an example of intrusion detection.

1. tracking access
2. detecting breaches 
3. failure auditing

### **Authentication by Ownership**
Authentication by ownership is based on something you have, such as a smart card, a key, a badge, or either a synchronous or asynchronous token.

#### **Synchronous Tokens.**

**Synchronous** **tokens** can be either a physical device, such as a system that uses continuous, time-based, or event-based authentication, or software, such as an authenticator app. All synchronous tokens use an algorithm at both the authentication server and the device to calculate a number, which is then displayed on the device’s screen. Users then enter the number as a logon authenticator, just as they would enter a password.

With a time-based synchronization system, the current time is used as the input value. The token generates a new dynamic password (usually every minute) that is displayed in the window of the token. To gain access, the password is entered with the user’s PIN at the workstation, and no token keyboard is required. This system necessitates that the clock in the token remain in sync with the clock in the authentication server. Should the clocks drift out of sync, the server can search three or four minutes on each side of the time to detect an offset, but, if the difference becomes too great, the clocks must be resynchronized.

>**NOTE** Synchronous tokens can be used in proximity devices that cause both the PIN and the password to be entered automatically.

An event-based synchronization system avoids the time-synchronization problem by increasing the value of a counter with each use. The counter is the input value. Users press a button to generate a one-time password and then enter this password with their PIN at the workstation to gain access. One common problem with event-based synchronization systems, though, is when a user creates a password using the token but does not use the password to log on, which causes the counter in the server and the counter in the token to become out of sync.

The third type of synchronous token is continuous authentication, which is used by systems that continuously validate the user’s identity, something that is often done with proximity cards or other devices that continuously communicate with the access control system. With continuous authentication, if the user walks away from the desktop and steps outside the range of the access control detector, the system locks the desktop.

#### **Asynchronous Tokens.**
An asynchronous token device uses challenge–response technology that involves a dialogue between the authentication server and the remote entity that it is trying to authenticate, a process that requires a numeric keyboard. Initial implementations of asynchronous tokens required a physical device that looked like a credit card–sized calculator, but later solutions relied on smaller devices the size of a key fob. With this asynchronous token, the authentication server issues a challenge number, which users enter, after which the token software computes a response to the value provided by the authentication server. Users then reply to the server with the value displayed on the token. Many of these systems also protect the token from misuse by requiring the user to enter a PIN along with the initial challenge value.

![[Pasted image 20251201185200.png]]


Here are the steps in an asynchronous challenge–response session:

1.  The user initiates a logon request.
2.  The authentication server provides a challenge (a random number that is the input value) to the user.
3.  The user enters the challenge received from the server and a secret PIN known only to the user into the calculation device (a credit card–sized calculator or a software program on a computer or smartphone).
4.  The token (or program) generates the response (the password) to the challenge, which appears in the window of the token.
5.  The user provides the correct password to the authentication server.
6.  Access is granted. Without the asynchronous token device and the right PIN, a correct answer to the challenge cannot be generated.

Another type of asynchronous token is a Universal Serial Bus (USB) token, which uses public key infrastructure (PKI) technology (e.g., a certificate signed by a trusted certification authority) but does not provide a one-time password. This token is a hardware device that is plugged into a computer’s USB port and is encoded with the user’s digital signature. Because the presence of the digital signature on the token is enough to provide proof of possession (something you have), nothing needs to be typed in.

>**NOTE** One problem with smart cards is that some users leave them unattended in the reader, which means that any user is authorized as long as the smart card remains in the reader.

### **Authentication by Characteristics/Biometrics**

Biometrics involves measuring various unique parts of a person’s anatomy or physical activities and can be used for both identification (i.e., physical biometrics, also called recognition) and authentication (i.e., logical biometrics). Even though many people associate biometrics with recognition (it is possible to build a massive database of personal biometrics data and then use that to determine someone’s identity), that is not its more common use, which is as a technique to validate (i.e., authenticate) a claimed identity. Instead of scanning a face and asking “Who is this?,” a better general use of biometrics is to scan a face and ask “Does this face match the characteristics of the claimed identity?” Following are the two categories into which the common biometric measures can be separated:

*   **Static (e.g., physiological) measures**—Physiological biometrics measure *what you are*, examples of which include reading fingerprint patterns, iris granularity, retina blood vessels, facial geometry, and hand geometry.
	
*   **Dynamic (e.g., behavioral) measures**—Behavioral biometrics measure *what you do*, examples of which include voice inflections, keyboard strokes, and signature motions. Note that biometrics of this type are sometimes separated into their own category (i.e., authentication by action).

#### **Concerns Surrounding Biometrics.**

There are three primary concerns with biometrics:
*   **Accuracy**: Each biometric device has at least two error rates associated with it: the **false rejection rate (FRR**), which is the rate at which valid subjects are rejected, and **the false acceptance rate (FAR)**, which is the rate at which invalid subjects are accepted. The point at which the two rates are equal is called the **crossover error rate (CER)**, which is the measure of the system’s accuracy expressed as a percentage. In practice, biometric devices that protect very sensitive resources, such as top-secret military facilities, are generally configured to accept a high level of false rejections, whereas systems that protect less sensitive resources, such as a public-use entry to a low-security building, may grant access to potentially unauthorized personnel so as not to excessively slow down access.
	
*   **Acceptability**: Certain biometric measurements, such as retinal scans, are more objectionable to some users than other biometric measurements, such as signature dynamics. Therefore, understanding the community of users and their comfort level with biometrics is crucial to acceptability. Reasons for low acceptability can be related to hygiene concerns (i.e., multiple people touching readers) or to perceived privacy violations.
	
*   **Reaction time**: Each biometric device requires time for the system to check an identity and respond; therefore, reaction time must be fast for most checkpoints because anything too slow hinders productivity and access. With the increased reliance on cloud-based or other remote services, network performance often plays into authentication techniques. For example, consider facial recognition at airport security checkpoints. If the system needs 30 seconds to identify each passenger, then passenger checkpoint lines would become far longer than they already are.

#### **Types of Biometrics.**
There are many types of biometrics, including the following:

*   **Fingerprint**: This biometric records fingerprints, the pattern of ridges and valleys on the tip of a finger, and is considered to be highly accurate for verifying a user.
	
*   **Palm print**: This biometric examines the physical structure of the palm and is also considered to be highly accurate. The system reaction time is five to seven seconds, and people tend to accept this type of scan.
	
*   **Hand geometry**: With this type of biometric, a camera takes a picture of the palm of the hand and, using a 45-degree mirror, the side of the hand. An analysis is then made using the length, width, thickness, and contour of the fingers. Hand geometry measurements are highly accurate. System response time is one to three seconds, and people tend to also accept these scans.
	
*   **Vein analysis**: Because human skin is not completely opaque, analysis can also extend under the skin to the specific arrangement of veins in fingers and hands, which is unique to an individual. However, researchers are examining whether certain vascular and connective tissue diseases may change vein patterns and thus result in false negative results.
	
*   **Retina scan**: This type of biometric analyzes the blood vessel pattern of the rear portion of the eyeball area, known as the retina, using a low-level light source and a camera. Even though a retina scan is very accurate for identification and authentication, it is susceptible to changes in a person’s physical condition, such as those caused by diabetes, pregnancy, and heart attacks, the emergence of which require users to enroll in the system again. Many people do not like retina scans because they feel the scans are intrusive and unsanitary and because they fear they will have to reveal private medical data. Response time averages between four and seven seconds.
	
*   **Iris scan**: This type of biometric uses a small video recorder to record unique patterns in the colored portion of the eye, known as the iris, caused by such things as striations, pits, freckles, rifts, and fibers. These scans are very accurate for identification and authentication and are well accepted. Moreover, iris scanning devices provide the capability for continuous monitoring to prevent session hijacking. Response time is one to two seconds.
	
*   **Facial recognition**: With facial recognition biometrics, video cameras measure certain features of the face, such as the distance between the eyes, the shape of the chin and jaw, the length and width of the nose, or the shape of cheekbones and eye sockets. Fourteen out of about 80 or so common features that can be measured are selected, which are then used to create a facial database. Facial recognition is accurate for authentication because face angle can be controlled, and, because it is passive and nonintrusive, it can continuously authenticate. Currently, however, it is less accurate for identification of individuals in a moving crowd.
    
*   **Voice pattern**: With voice pattern biometrics, audio recorders and other sensors capture as many as seven parameters of nasal tones, larynx and throat vibrations, and air pressure from the voice. However, these biometrics are not accurate for authentication because voices can be too easily replicated by computer software and accuracy can be further diminished by background noise. Response time is typically slow because it can take over 10 seconds to find a match. Most users will accept this type of biometric, but, because of the relatively long response time, it is not yet popular for everyday use.
	
*   **Keystroke dynamics**: This biometric involves a user typing a selected phrase onto a reference template, during which the keystroke dynamics measure each keystroke’s dwell time (i.e., how long a key is held down) and flight time (i.e., the amount of time between keystrokes). Keystroke dynamics are considered very accurate and lend themselves well to two-factor authentication. Because the technology is easy to use when someone is logging on, it combines the ID processes of *something you should know* with *something you own*. Moreover, keystroke dynamics are well accepted and can provide constant authentication.
	
*  **Signature dynamics**: With this type of biometric, sensors in a pen, stylus, or writing tablet are used to record pen stroke speed, direction, and pressure. These dynamics can be very accurate, and most users accept them.
	
*  **Gait analysis**: This type of metric compares the physical movements of people while walking or running to match their unique actions. Although injury or degeneration over time affects people’s gait, the overall way in which they walk is generally unique to them.

>Academic research into biometric algorithms expanded at a rapid pace starting in the mid-2010s, and, because of recent advances in machine learning algorithms (i.e., AI), biometrics matching processes are getting faster and more accurate very quickly. Based on this growing body of research, it has become possible to develop highly accurate biometric techniques that are fast enough for mass deployment.
#### **Advantages and Disadvantages of Biometrics.**

| **Advantages of Biometrics**                         | **Disadvantages of Biometrics**                                                                             |
| :--------------------------------------------------- | :---------------------------------------------------------------------------------------------------------- |
| A person must be physically present to authenticate. | Physical characteristics might change over time.                                                            |
| There is nothing for the user to remember.           | Physically disabled users may have difficulty with accessibility, especially for performance-based systems. |
| Biometric traits are difficult to fake or replicate. | Not all techniques are equally effective; selecting the best one for a specific use case can be difficult.  |
| Lost IDs or forgotten passwords are not problems.    | The authentication response time may be too slow, causing delays.                                           |

### **Authentication by Location and Authentication by Action**

| Aspect                | Authentication by Location                                                                                                                                               | Authentication by Action                                                                                                                                            |
| :-------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Core Concept**      | Uses the user's physical or network location as a factor to verify authenticity.                                                                                         | Uses the unique patterns in how a user performs an action as a factor to verify authenticity.                                                                       |
| **Commonly Called**   | *Somewhere you are*                                                                                                                                                      | *Something you do* (often considered a subset of behavioral biometrics)                                                                                             |
| **How It Works**      | The system checks the location of the access attempt (e.g., via GPS, IP address, network cell tower) against an expected or allowed location.                            | The system measures and analyzes the unique characteristics of a user's action, such as rhythm, speed, pressure, or pauses.                                         |
| **Primary Purpose**   | To provide contextual assurance. A login from an unexpected location can trigger denial or require additional verification.                                              | To verify identity based on habitual behavior that is difficult for others to replicate precisely.                                                                  |
| **Example**           | A debit card transaction is attempted at a fuel pump in Topeka, KS, but the associated online login IP address is from Tampa, FL. The mismatch may deny the transaction. | A system measures a user's keystroke dynamics—the unique dwell time (how long a key is held) and flight time (time between keystrokes) when typing a passphrase.    |
| **Another Example**   | A taxi-hailing app uses the customer's smartphone GPS location to validate that a pickup request is coming from a plausible, non-spoofed location.                       | Signature dynamics analysis, which measures the speed, pressure, and stroke order of a handwritten signature.                                                       |
| **Key Consideration** | Should **only** be used as part of **Multifactor Authentication (MFA)**, not as a standalone factor. Location data can sometimes be spoofed.                             | Often overlaps with behavioral biometrics. Its effectiveness depends on the consistency of the user's behavior and the system's ability to measure subtle patterns. |

## **Single Sign-On**

A **single sign-on (SSO)** strategy ==allows users to sign on to a computer or network once and then be allowed into all computers and systems where they are authorized, thus making it unnecessary to enter multiple user IDs or passwords.== SSO reduces human error, which is a major part of system failures. Thus, SSO is highly desirable but also difficult to put in place.

### **Advantages and Disadvantages of SSO**

| Advantages of SSO                                                                                                                                                                                          | Disadvantages of SSO                                                                                                                                                                  |
| :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Efficiency:** The user logs on only once to access multiple authorized systems, streamlining the process.                                                                                                | **Catastrophic Compromise:** A single compromised password grants an intruder access to **all** systems linked to the SSO account.                                                    |
| **Stronger Passwords:** Users are more likely to create and remember a single, complex password.                                                                                                           | **Dependency on Strong Authentication:** Using only a static password with SSO is risky. It requires **Multifactor Authentication (MFA)** or dynamic passwords for adequate security. |
| **Continuous Session Monitoring:** The SSO server can monitor workstation activity and enforce consistent time-out policies, automatically disconnecting inactive sessions to prevent unauthorized access. | **Integration Challenges:** Implementing SSO with unique, custom, or legacy systems in a network can be difficult and complex.                                                        |
| **Centralized Security Policies:** Provides a central point to enforce security policies like failed logon attempt thresholds and account lockouts, protecting against brute-force attacks.                | **Script Security:** While administration scripts simplify management, they can also expose sensitive data and often lack robust, multi-factor security controls.                     |
| **Centralized Administration:** Ensures consistent application and updates of security policies and procedures across all connected systems from one management point.                                     | **Single Point of Failure:** The central authentication server becomes a critical target; if it fails, it can block **all** system access for users.                                  |

### **SSO Processes**
Examples of SSO processes include the Kerberos, SESAME, and LDAP methods. Following is a discussion of each one.

#### **Kerberos.**

==Kerberos is a computer network authentication protocol that allows nodes communicating over a nonsecure network to prove their identity to one another in a secure manner;== it is also a suite of free software published by the **Massachusetts Institute of Technology (MIT)** that applies the Kerberos protocol. It is designed primarily as a client/server model and provides mutual authentication between the user and the server. Moreover, Kerberos protocol messages are protected against eavesdropping and replay attacks.

The Kerberos process begins with users sending their ID and access request through the Kerberos client software on the workstation to the KDC. At the KDC, the authentication server verifies that the user and the requested service are in the KDC database, and, if they are, it sends a ticket, which is the user’s unique time-stamped key for the requested service. If the ticket is not used within the designated time, it will not work. Included in the ticket are the user ID and the session key as well as the ticket for the object encrypted with the object’s key shared with the KDC.

With Kerberos, security depends on careful execution and maintenance. Therefore, life spans for authentication credentials should be as short as possible, using time stamps to reduce the threat of replayed credentials, and the KDC must be physically secured because it—particularly the authentication server—is a potential single point of failure. To reduce the risk, redundant authentication servers can be used. Finally, the KDC should be hardened, meaning it should have a secured operating system and application, and should not allow any non–Kerberos network activity.

#### **SESAME.**

The Secure European System for Applications in a Multi-vendor Environment (SESAME) is a research and development project funded by the European Commission and developed to address weaknesses in Kerberos. It supports SSO, but, unlike Kerberos, it improves key management by using both symmetric and asymmetric keys to protect interchanged data, making it essentially an extension of Kerberos. Moreover, it offers public key cryptography and role-based access control abilities.

#### **LDAP.**

The Lightweight Directory Access Protocol (LDAP) is an open source (i.e., does not rely on any specific vendor’s product) protocol for defining and using distributed directory services. One of the core services LDAP provides is handling access control credentials, which makes it easy for administrators to manage logon and access credentials on computers and devices across a network. Although LDAP does not provide a complete SSO solution, it is a part of many SSO solutions. Because LDAP routinely exchanges sensitive information across networks, it is essential to secure the messages; one of the most common ways to do this is to use LDAP over SSL (LDAPS), which uses SSL/TLS for all message exchanges across the network.

## **Policies and Procedures for Accountability**

At this point, you have learned how users are **identified (step 1)**, **authenticated (step 2)**, and **authorized (step 3)**. Now it’s time for the last part of the access control process: accountability. **Accountability** involves tracing an action to a person or process to know who made the changes to the system or data, which is important for conducting audits and investigations as well as tracing errors and mistakes. Accountability answers the question, “==Can you hold users responsible for what they do on the system?”==

### **Log Files**

Log files, which are a key ingredient to accountability, are records that detail **==who logged on to the system, when they logged on, and what information or resources they used.==** In the early days of computing, logs were used on systems that were shared by several users in order to be able to charge them for their time and by companies, such as CompuServe and AOL, to record Internet use when it was charged by the hour. On today’s networks, time-based billing has given way to either a fixed fee or a fee based on bandwidth usage, but, now, logging is used for more than just billing; it is also a valuable tool to detect, prevent, or monitor access to a system.

### **Monitoring and Reviewing**

One of the main reasons for tracking user access activities is to detect questionable actions and respond to them, which means that you should use software that monitors activity logs and generates alerts when it finds suspicious activity. Moreover, continuous monitoring is an important part of a secure access control system, but not all suspicious activity is obvious. At times, the only way to detect account policy violations is to review user actions over a period of time, a requirement that should be included in the account policy. Such periodic reviews help to validate that user access definitions are correct as well as helping to find inappropriate activity or excessive permissions. Of course, every policy should outline steps to take to respond to any violations, but knowing how to respond to violations is just as important as finding them in the first place.

### **Data Retention, Media Disposal, and Compliance Requirements**

Many current laws require that organizations take measures to secure many types of data, one example being the **==Health Insurance Portability and Accountability Act (HIPAA)==**, which protects the privacy of personal health data and gives patients certain rights to that information. Another example is the **==Fair and Accurate Credit Transactions Act (FACTA)==**, which requires any entity that keeps consumer data for business purposes to destroy personal data before discarding it. More recently, t**==he California Consumer Protection Act (CCPA)==** and **==the European Union’s General Data Protection Regulation (GDPR)==** place requirements on how long to retain data and when disposal is mandatory.

These and similar laws require the protection of private data with proper security controls and outline the prescribed ways to handle, store, and dispose of data. If these rules and regulations are not followed, intruders can, for example, simply dive into dumpsters or break into information systems to get sensitive data.

### **Procedures**

Organizations can apply access controls in various forms, providing different levels of restriction and at different places within the computing system. A combination of access controls provides a system with layered, defense-in-depth (DiD) protection, an approach that makes it harder for attacks to succeed because attackers must compromise multiple security controls to reach a resource. Security personnel should ensure that they never rely on a single control, instead protecting every critical resource with multiple controls.

#### **Security Controls**

Any mechanism intended to avoid, stop, or minimize a risk of attack for one or more resources is a *security control*, of which there are several types based on their purpose. Most organizations need a diverse mix of security controls to protect their systems from all types of attacks. 

| CONTROL TYPE          | DESCRIPTION                                                                                                                                                                                                                                                                                                                                                                                                                         |
| :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Administrative**    | These are policies approved by management and passed down to staff in the form of rules. They are a first line of defense to inform users of their responsibilities. Examples include policies on password length.                                                                                                                                                                                                                  |
| **Logical/technical** | These are additional policies that are controlled and enforced automatically and are intended to reduce human error. For example, a computer can check passwords to make sure they follow the rules.                                                                                                                                                                                                                                |
| **Hardware**          | This includes equipment that checks and validates IDs, such as **Media Access Control (MAC)** filtering on network devices; smart card use for multifactor authentication; and security tokens, such as **radio frequency identification (RFID)** tags. In this instance, MAC (not the same as the mandatory access controls discussed later in the chapter) is a hardware address that uniquely identifies each node of a network. |
| **Software**          | These controls are embedded in the operating system and application software. They include the **Microsoft Windows standard New Technology File System (NTFS)** permissions, user accounts requiring logon, and rules restricting services or protocol types. These items are often part of the ID and validation phase.                                                                                                            |
| **Physical**          | These are devices that prevent physical access to resources, including such things as security guards, ID badges, fences, and door locks.                                                                                                                                                                                                                                                                                           |

## **Formal Models of Access Control**

Most users have encountered access control restrictions (some of the most visible being those protecting access to computer resources), such as when they have typed an incorrect password and been denied access. Because many ways are available for restricting access to resources, it is helpful to refer to models to help design effective access controls. Following are some of the formal models of access control:

*   **Discretionary access control (DAC)**: With DAC, the owner of the resource decides who gets in and changes permissions as needed; permissions can be transferred.
*   **Mandatory access control (MAC)**: With MAC, permission to access a system or any resource is determined by the sensitivity of the resource and the security level of the subject. Because permissions cannot be transferred, MAC is stronger than DAC.
*   **Nondiscretionary access control**: Nondiscretionary access controls are closely monitored by the security, not the system, administrator.
*   **Rule-based access control**: A list of rules, maintained by the data owner, determines which users have access to objects. 

Other models are based on the work of Biba, Clark–Wilson, and Bell–LaPadula; these models describe the use of access controls and permissions to protect confidentiality or integrity.

### **Discretionary Access Control**
The Common Criteria defines **discretionary access control (DAC)** as follows:

> [A] means of restricting access to objects based on the identity of subjects and/or groups to which they belong. The controls are discretionary in the sense that a subject with certain access permission is capable of passing that permission (perhaps indirectly) on to any other subject.

The Common Criteria also notes the following:

> [S]ecurity policies defined for systems used to process classified or other sensitive information must include provisions for the enforcement of discretionary access control rules. That is, they must include a consistent set of rules for controlling and limiting access based on identified individuals who have been determined to have a need to know for the information.


#### **Operating Systems–Based DAC**
Operating systems are primarily responsible for controlling access to system resources, such as files, memory, and applications, through access controls, whose maintenance is one of the main jobs of security administrators. Access controls are effective when they ensure that only authorized users can access resources and efficient when they ensure that users can access all the resources they need, but creating access controls that are both effective and efficient can be challenging. Organizations must decide how they will design and maintain access controls to best meet their needs. Following are a few points organizations must consider in developing access control policies:

*   **Access control method**: Today’s operating systems contain access control settings for individual users (rule based) or for groups of users (role based). Which method an organization uses depends on its size and the specific access rights needed for individuals or roles.
*   **New user registration**: Creating new user accounts can be time consuming but must be done quickly so new people can do their jobs. Thus, this process must be standardized, efficient, and accurate.
*   **Periodic review**: Over time, users often get special permission to complete a particular project or perform a special task; therefore, it is important that these permissions be reviewed periodically to ensure they stop when they are no longer needed. Reviewing these permissions periodically solves problems of compliance and auditing by making sure people can access only required areas.

#### **Application-Based DAC**
Application-based DAC denies access based on context or content through the application by presenting only options that are authorized for the current user. For example, an automatic teller machine (ATM) menu limits access by displaying only the options that are available to a specific user. You can apply security controls using these types of DACs based on user context or resource contents:

*   In a *context-based system*, access is based on user privileges as defined in the user’s own data records. This type of access is usually granted to persons acting in a certain job role or function.
*   In a *content-dependent system*, access is based on the value or sensitivity of data items in a table. This type of access system checks the content of the data being accessed and allows, for example, a manager of Department A to see employee records for personnel that contain an *A* in the department field but not records containing any other value in that field.

### **Mandatory Access Control**
**Mandatory access control (MAC)** is another method of restricting access to resources. You determine the level of restriction by how sensitive the resource is, which is represented by a sensitivity label, or classification. Individuals must then be formally authorized (i.e., obtain clearance) to access sensitive information. Security policies defined for systems that are used to process classified information (or any other sensitive information) must include provisions for enforcing MAC rules; that is, they must include a set of rules that controls who can access what information.

>**NOTE**: Remember, sensitivity labels, or classifications, are applied to all objects (i.e., resources), whereas privilege- or clearance-level labels are assigned to all subjects (i.e., users or programs).

Under MAC, the owner and the system jointly make the decision to allow access. The owner provides the need-to-know element because not all users with a privilege or clearance level for sensitive material need access to all sensitive information. The system then compares the subject and object labels that go with the terms of the Bell–LaPadula confidentiality model, which is covered later in the chapter. Based on that comparison, the system either grants or denies access.

Another element of MAC is temporal isolation, or more commonly described as time-of-day restriction, which restricts access of objects to specific times. First, the sensitivity level of objects is classified, and then access is allowed to those objects only at certain times. Temporal isolation is often used in combination with role-based access control.

### **Nondiscretionary Access Control**

In nondiscretionary access control, access rules are closely managed by the security administrator and not by the system owner or ordinary users for their own files. Nondiscretionary access control can be used on many operating systems and is more secure than discretionary access control because the system does not rely only on users’ compliance with organizational policies. For example, even if users obey well-defined file protection policies, a Trojan horse program could change the protection to allow uncontrolled access, which is a kind of exposure that is not possible under nondiscretionary access control.

Security administrators have enough control in nondiscretionary access control to make sure that, to preserve confidentiality, sensitive files are write-protected for integrity and readable only by authorized users. Thus, because users can run only those programs they are expressly allowed to run, the chances are reduced that a corrupted program will be used.

Nondiscretionary access control helps ensure that system security is enforced and tamperproof; therefore, if an organization needs to manage highly sensitive information, it should seriously consider using nondiscretionary access control, which does a better job of protecting confidentiality and integrity than DAC. The data owner, who is often the user, does not make access decisions, which allows some of the benefits of MAC without the added administrative overhead.
### **Access Control Lists**

Most operating systems provide several options for associating lists, called **access control lists (ACLs)**, with objects, with different ACL-enabling options provided on the various types of operating systems. For example, Linux and macOS have read, write, and execute permissions, which can be applied to file owners, groups, or global users, whereas Windows has share and security permissions, both of which enable ACLs to define access rules. Share permissions are used to get to resources by a network share, whereas security permissions are used to get to resources when the user is logged on locally. Some Windows permissions include the following:
*   **Share permissions**: Full, change, read, and deny
*   **Security permissions**: Full, modify, list folder contents, read-execute, read, write, special, and deny

In both share and security permissions, *deny* overrides every other permission, but what happens if no ACL exists for a resource? In that case, most authorization systems will use *implicit deny*, which means that, if no rule to grant access exists, access is automatically denied. This approach is more restrictive than implicitly granting access and then adding restrictions, but is more secure.

Because of the greater number of choices when using ACLs as opposed to file permissions, Windows ACLs are said to be more *fine grained* because they allow a greater level of control. shows an ACL.

![[Pasted image 20251201191113.png]]

### **Role-Based Access Control**
Another type of access control is **role-based access control (RBAC)**, which bases access control approvals on the jobs the user is assigned. The security administrator assigns each user to one or more roles, or some operating systems use groups instead. The resource owner decides which roles have access to which resources. Microsoft Windows uses global groups to manage RBAC. 

![[Pasted image 20251201191144.png]]

Starting with a clear list of role definitions that fit an organization is key to RBAC; therefore, before you can assign access rules to a role, you must define and describe the roles in an organization. The process of defining roles, approvals, role hierarchies, and constraints is called *role engineering*. The real benefit of RBAC over other access control methods is its ability to represent the structure of the organization and force compliance with control policies throughout it.
### **Content-Dependent Access Control**
Content-dependent access control is based on what is contained in the data, which requires the access control mechanism (i.e., the arbiter program, which is part of the application, not the operating system) to look at the data to decide who should get to see it. The result is better granularity than the other access control methods provide, whereby access is controlled to the record level in a file rather than simply to the file level. The cost of this access control granularity is higher, however, because it requires the arbiter program, which uses information in the object being accessed, for example, what is in a record. The decision usually comes to a simple if-then question, for example, “If high-security flag equals yes, then check security level of user.” Managers might have access to the payroll database to review data about specific employees, but they might not have access to the data about employees of other managers.

![[Pasted image 20251201191234.png]]

### **Constrained User Interface**

| **Method of Constraint**                              | **Key Mechanism**                                                                                                                                                                                               | **Example**                                                                                                                                                                 |
| :---------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Menus**                                             | Limits user awareness and access by only displaying menu options for which the user is authorized. Options for restricted data or functions are simply not shown.                                               | A user logs into an application and sees a simplified menu without administrative tabs or links to confidential reports.                                                    |
| **Database Views (View-Based Access Control - VBAC)** | Creates a customized "view" or window into a database for each user or group, filtering out rows and columns they are not permitted to see. A feature called **multitenancy** extends this for cloud databases. | In a company database, a manager from Department A can only view employee records where the department field is "A," while records for Department B are invisible to them.  |
| **Physically Constrained Interface**                  | The hardware device itself presents a limited, fixed set of input options, physically preventing the user from requesting unauthorized actions.                                                                 | An ATM machine provides a specific set of buttons for withdrawal, deposit, or balance inquiry, with no ability to type arbitrary commands.                                  |
| **Encryption**                                        | Constrains access by making data unreadable without the correct decryption key. This both restricts access and hides information from unauthorized users.                                                       | Sensitive files are stored in encrypted form. Even if a user gains access to the storage location, they cannot read the file contents without the proper cryptographic key. |
## **Other Access Control Models**
Other access control models, such as the Bell–LaPadula model, the Biba integrity model, the Clark–Wilson integrity model, and the Brewer–Nash model, have helped shape today’s access controls. You will learn about each model in the following sections.

| **Model**                        | **Primary Security Focus**                                  | **Core Principles / Rules**                                                                                                                                                                                                                                                                              | **Key Approach**                                                                                                                                                                                                                             |
| :------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Bell–LaPadula**                | **Confidentiality** of data (e.g., classified information). | • **No Read Up:** A subject cannot read an object of a higher classification (Simple Security Property).<br>• **No Write Down:** A subject cannot write to an object of a lower classification (*-Property).                                                                                             | Prevents unauthorized disclosure by controlling information flow based on security labels (clearance for subjects, classification for objects).                                                                                              |
| **Biba Integrity Model**         | **Integrity** of data.                                      | • **No Read Down:** A subject cannot read an object of a lower integrity level (Simple Integrity Axiom).<br>• **No Write Up:** A subject cannot write to an object of a higher integrity level.<br>• **No Invocation Up:** A subject cannot request services from a subject of a higher integrity level. | Prevents corruption of high-integrity data by untrusted sources and limits the influence of less-trusted subjects.                                                                                                                           |
| **Clark–Wilson Integrity Model** | **Integrity**, with a focus on commercial/business systems. | 1. Prevents **unauthorized users** from making changes.<br>2. Prevents **authorized users** from making improper changes.<br>3. Maintains **internal and external consistency**.                                                                                                                         | Enforces integrity via **well-formed transactions** (programs) and **separation of duties**. Users access data only through certified programs (Access Triples: subject-program-object), and data items have constraints to ensure validity. |

## **Effects of Breaches in Access Control**

The failure to control access can give an advantage to an organization’s opposition, which might be a military force, a business interested in competitive intelligence, or even a neighbor. The following list details some of the losses that can occur:
*   Disclosure of private information
*   Corruption of data
*   Loss of business intelligence
*   Danger to facilities, staff, and systems
*   Damage to equipment
*   Failure of systems and business processes

Not all incidents have the same effect, which makes some incidents easier to spot than others. For example, losses due to disclosure of business secrets, including business intelligence, often go unnoticed for quite some time. Moreover, by the time corruption of data is discovered, a database and all its backups might be rendered useless, which can easily cause failures in systems and business processes.

Some types of DoS attacks are short lived and can be found quickly and stopped before they cause serious damage. Other types of DoS attacks can inflict more severe damage on an organization because they take longer to evolve and can affect the ability of a business to serve its customers, which may cause some of them to then take their business elsewhere.

## **Threats to Access Controls**

Threats to access controls come in many forms, and a list of them can never be complete because new threats evolve all the time. An example is the peer-to-peer (P2P) risk in which P2P users share their Documents folder with each other by accident, which can expose sensitive documents to other users.

Access controls can be compromised in several ways, including the following:

| **Threat**                                          | **Mechanism & Risk**                                                                                                                                                                                                                             |
| :-------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Gaining Physical Access**                         | Direct access to a device or storage media (e.g., stolen laptop, USB drive) renders logical controls useless. Allows data theft/copying, installation of keyloggers or malware, equipment damage, and potential Denial-of-Service (DoS) attacks. |
| **Eavesdropping by Observation (Shoulder Surfing)** | Visually capturing sensitive information from an authorized user's screen, desk documents, or whiteboards. Modern risk includes recording via smartphone cameras and audio/video devices.                                                        |
| **Bypassing Security**                              | Attackers use alternative, unsecured access paths that developers may overlook (e.g., direct database connection, local server login, mapped network drives) to circumvent primary security measures like a web application's login.             |
| **Exploiting Hardware and Software**                | Installing malicious programs like **Trojan horses** on a compromised system to gain persistent, hidden control, often without the knowledge of the system owner or administrator.                                                               |
| **Reusing or Discarding Media**                     | Recovering sensitive data from improperly sanitized or discarded storage media (hard drives, DVDs, USB sticks). Secure destruction (shredding, degaussing) is required to prevent this.                                                          |
| **Electronic Eavesdropping (Wiretapping)**          | Intercepting data transmissions by physically tapping into network cables. Wireless networks and insecure access points significantly increase this risk.                                                                                        |
| **Intercepting Communication (Sniffing / MITM)**    | Capturing network traffic as it passes (**sniffing**). A **Man-in-the-Middle (MITM)** attack intercepts and potentially alters communication between two parties, making them believe they are directly connected.                               |
| **Accessing Networks**                              | Exploiting unprotected network connection points (active but unused wall ports) or insecure wireless access points to gain unauthorized network entry.                                                                                           |
| **Exploiting Applications**                         | Taking advantage of software vulnerabilities, such as **buffer overflows**, where excess input allows execution of malicious code, leading to system compromise.                                                                                 |

## **Effects of Access Control Violations**
You have seen some of the ways attackers can compromise access controls. But what happens if an attacker is successful at compromising access controls, and what might the impact be? An access control violation can have the following harmful effects on an organization:
*   Loss of customer confidence
*   Loss of business opportunities
*   New legislation and regulations imposed on the organization
*   Bad publicity
*   More oversight
*   Financial penalties
## **Centralized and Decentralized Access Control**

Centralized access control is an access control approach in which a single common entity, such as an individual, a department, or a device, decides who can get into systems and networks, which means that access controls are managed centrally, rather than locally. Owners decide which users can get to which objects, and ==the central administration supports the owners’ directives. Centralized authentication services are applied and enforced through the use of **authentication, authorization, and accounting (AAA) servers**.==

The benefits of using AAA servers include the following:
*   Involves less administration time because user accounts are maintained on a single host
*   Reduces design errors because different access devices use similar formats
*   Reduces security administrator training because administrators have to learn only one system
*   Improves and eases compliance auditing because all access requests are handled by a single system
*   Reduces help-desk calls because the user interface is consistent

>**NOTE** Centralized access control is generally simpler to manage than local control, but the drawback is that, if it fails, large numbers of users can be affected and unable to get into the computer system.

### **Types of AAA Servers**
The following sections will provide information on the leading types of AAA servers: RADIUS, the most popular; TACACS+; the DIAMETER protocol; and the SAML standard.

| **Feature**                | **RADIUS (Remote Authentication Dial-In User Service)**                                                                                                           | **TACACS+ (Terminal Access Controller Access Control System Plus)**                                                                                                                                               | **DIAMETER**                                                                                                                                                                                            |
| :------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Primary Role**           | The most popular AAA service for network access authentication.                                                                                                   | An IETF standard protocol for detailed, centralized authentication and authorization, often used in network device administration.                                                                                | An advanced, extensible protocol based on RADIUS, designed for next-generation AAA services.                                                                                                            |
| **Configuration**          | Uses **two** separate configuration files:<br>1. Client config (address & shared secret).<br>2. User config (identification & authentication data).               | Uses a **single** configuration file to control server operations, define users/attributes, and manage authentication/authorization procedures.                                                                   | Built on a modular **base protocol** (defines format, transport, error handling) with **extensions** for specific AAA transaction types.                                                                |
| **Transport Protocol**     | Uses **UDP** (User Datagram Protocol).                                                                                                                            | Uses **TCP** (Transmission Control Protocol).                                                                                                                                                                     | Primarily uses **UDP** but is designed with more reliability features than RADIUS. It can also operate in a **P2P mode**.                                                                               |
| **Authentication Process** | 1. NAS decrypts the user's UDP request.<br>2. NAS authenticates the source.<br>3. NAS validates against the user file.<br>4. NAS responds (allow/deny/more info). | 1. Client sends a TCP request with a cleartext header and encrypted body (user ID, password, key).<br>2. Server replies with permit/deny and connection attribute/value pairs.                                    | Flexible process defined by its base protocol and specific extensions. Designed to support complex authentication, authorization, and accounting transactions.                                          |
| **Key Features / Notes**   | • Simpler, widely adopted.<br>• Combines authentication and authorization.<br>• Uses a shared secret for security.                                                | • **Separates** authentication, authorization, and accounting processes.<br>• Originally Cisco proprietary, now an open standard.<br>• Provides more granular control over authorization (attribute/value pairs). | • Designed to overcome RADIUS limitations (e.g., better scalability, error handling, security).<br>• Supports new applications and mobile environments.<br>• More flexible and extensible architecture. |

#### **SAML**
**Security Assertion Markup Language (SAML)** is an open standard used for exchanging both authentication and authorization data. It is based on **Extensible Markup Language (XML)** and was designed to support access control needs for distributed systems. SAML is often used in web application access control. However, it is not a complete centralized AAA system but rather a data format specification. We include it in this section because systems that use SAML do depend on a central trusted authority to issue security tokens.

## **Cloud Computing**
One of the strongest trends in enterprise development is incorporating shared services from external sources and migrating internal data and functionality to hosted computing environments. One such practice is using computing services that are delivered over a network, which is called **cloud computing**. The computing services may be located within the organization’s network or provided by servers that belong to some other network and organization. There are several cloud models available to meet the needs of a diverse user environment, but all cloud services generally fall into one of the following categories:
*   **Private cloud**—All the hardware and software required to provide services, including the network infrastructure, is operated for a single organization. The components may be managed by the organization or by a third-party provider, and the actual infrastructure can be located within or outside the organization’s network.
*   **Community cloud**—This type of infrastructure provides services for several organizations, which all share the cloud environment and use it for their specific needs. The infrastructure can be managed by one of the participating organizations or by a third party.
*   **Public cloud**—This type of cloud infrastructure is available to unrelated organizations or individuals and is generally available for public use and managed by a third-party provider.
*   **Hybrid cloud**—This type of cloud infrastructure contains components of more than one type of cloud, including private, community, and public clouds. Hybrid clouds are useful for extending the limitations of more restrictive environments and are often used to provide resiliency and load balancing by distributing workload among several infrastructures or segments.

In the most general case, a **cloud service provider (CSP)** maintains several (sometimes many) data centers with racks of server computers. Each server runs multiple virtual machines and is able to provide services to many clients simultaneously. CSPs offer different services to their customers over the Internet. Common cloud services include the following:
*   **Infrastructure as a Service (IaaS)**: IaaS provides users with access to a physical or virtual machine, to which users load their own operating systems. They then manage all aspects of the machine, just as though it were a local computer.
*   **Platform as a Service (PaaS)**: PaaS provides the user with access to a physical or a virtual machine running any of a number of popular operating systems. Unlike IaaS, with PaaS, the CSP manages the operating system and the underlying hardware. Instead of connecting to a local server, the user connects to a virtual server in the cloud, and, once the connection is made, the user treats the cloud instance just like any other computer. The user can install and run software as though the server were in the local data center.
*   **Software as a Service (SaaS)**: In the SaaS model, users access software from cloud clients, of which the most basic type is the web browser. Rather than needing to install or manage any software, all users have to do is connect to the correct server and use the software as though it were running in their local network. Examples of popular SaaS include Google Apps™ service, Microsoft Office 365™, and SalesForce®.

There are several advantages to using cloud services over traditional in-house software, and most of the advantages include cost savings. Following are some of those cost-saving advantages:

*   **No need to maintain a data center**: The CSP maintains multiple data centers and handles all the logistics and details of making services available anywhere on the Internet.
*   **No need to maintain a disaster recovery site**: Since the CSP already maintains services and data at multiple sites, multiple copies of data in the cloud are always available.
*   **Outsourced responsibility for performance and connectivity responsibility**: All clients must do is have access to the Internet. The CSP is responsible for making sure everything works as promised in its contracts.
*   **On-demand provisioning**: Cloud customers can increase and decrease the computing power and storage space they purchase based on current needs, a feature that can save organizations substantial amounts of money over maintaining unused hardware. It also means that the organization can respond to increased demand without having to buy and set up new servers.

Cloud computing does have its disadvantages, though. For example, moving services outside the organization makes it more difficult to control the entire environment. Cloud disadvantages include the following:

*   **Greater difficulty in keeping private data secure**: Data stored in the cloud is more accessible to both authorized users and attackers. Cloud environments are essentially untrusted. Therefore, data owners must enforce extra precautions to ensure access controls are sufficient to protect their data.
 
*   **Greater danger of private data leakage**: One of the advantages of cloud computing is that the CSP ensures that an organization’s data is always available. One way it does this is by keeping multiple current copies of data in different locations. Every additional copy of private data increases the possibility that data may leak to unauthorized users.

*   **Greater demand for constant network access**: Access to cloud services depends on the network connection to those services, which means a user who does not have reliable or fast Internet access may encounter difficulties with cloud services. This concern is greatest for mobile users who travel in and out of areas of reliable coverage or who do not have reliable Internet access.

*   **Greater need for clients to trust outside vendors**—Releasing private data to a CSP requires some level of trust in that provider. However, trusting a third party with sensitive data may violate some laws, regulations, or vendor requirements. Therefore, before moving data to a cloud, all constraints must carefully be examined due to outside requirements. Although the safest policy is to treat the cloud as an untrusted environment, there has to be some basic level of trust with a CSP.

One of the most difficult problems organizations encounter today is keeping private data secure in the cloud, the main difficulty being that data moves from a trusted location inside an organization’s infrastructure to an untrusted cloud environment. Users can connect from virtually anywhere in the world to cloud resources, which means that the need to identify and authorize users is even more important than with legacy on-premises resources. The basis of access control is nonrepudiation, which means the access controls can associate an identity to a resource request and that association is not disputable. Because users can connect to cloud services from anywhere (including insecure networks and devices), the question is, who should be responsible for identification, authorization, and authentication? To address that question, the **==Cloud Security Alliance (CSA)==**, a nonprofit organization with a mission to promote best practices for using cloud computing securely, published a guide on cloud security, *Security Guidance for Critical Areas of Focus in Cloud Computing*. The report describes the challenges of cloud computing this way:

> Managing information in the era of cloud computing is a daunting challenge that affects all organizations; even those that are not seemingly actively engaged in cloud-based projects. It begins with managing internal data and cloud migrations and extends to securing information in diffuse, cross-organization applications and services. Information management and data security in the cloud era demand both new strategies and technical architectures.

CSA also developed the Cloud Controls Matrix (CCM), which is a framework that defines 133 cloud security control objectives and organizes those objectives into 16 domains. The CCM also maps each control objective to appropriate standards, regulations, and control frameworks.


Cloud computing punctuates the need for good access and identity management. Although many CSPs offer IAM services, applications may need to integrate on-premises and cloud-based identity management across multiple cloud environments. A cloud access security broker (CASB) provides these integrated identity and access management services for cloud-based applications and storage. You can think of a CASB as being an SSO solution that spans multiple clouds. A CASB does move a bit toward centralization, but in the interest of providing users with a rich and secure experience.

There is no easy solution to the problem of managing access control in cloud environments, and researchers are constantly exploring novel ways to ease the burden on organizations. Today, the best approaches are to extend the existing concepts presented in the chapter. Some of the access controls will likely exist in cloud environments. The most important rule is to always use a defense-in-depth strategy and never rely on only a single control to protect any resource.

## **KEY CONCEPTS AND TERMS**

| **Term**                                                    | **Definition**                                                                                                                                                 |
| :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Access Control**                                          | The process of protecting resources by restricting access to only authorized users.                                                                            |
| **Access Control List (ACL)**                               | A list attached to an object (e.g., a file) that specifies which subjects (users, processes) are granted access and what operations they can perform.          |
| **Access Control Policy**                                   | A set of rules that defines which users can perform what actions on which resources.                                                                           |
| **Accountability**                                          | The security principle that ensures actions can be traced to the individual who performed them, enabling audit and investigation.                              |
| **Authentication**                                          | The process of verifying a subject's claimed identity (e.g., using a password, token, or biometric).                                                           |
| **Authentication, Authorization, and Accounting (AAA)**     | A framework for centrally managing network access: verifying identity (Authentication), granting permissions (Authorization), and tracking usage (Accounting). |
| **Authorization**                                           | The process of determining what an authenticated user is allowed to do with a specific resource.                                                               |
| **Biometrics**                                              | Authentication based on unique physical or behavioral characteristics (e.g., fingerprint, iris scan, keystroke dynamics).                                      |
| **Chinese Wall**                                            | A security model (Brewer-Nash) that dynamically restricts access to prevent conflicts of interest (e.g., an auditor accessing data from competing clients).    |
| **Cloud Computing**                                         | The delivery of computing services (servers, storage, software) over a network, typically the internet.                                                        |
| **Cloud Service Provider (CSP)**                            | A company that offers cloud computing services (e.g., AWS, Microsoft Azure, Google Cloud).                                                                     |
| **Common Criteria**                                         | An international standard (Common Criteria for Information Technology Security Evaluation) for certifying the security of computer systems and products.       |
| **Constrained User Interface**                              | A method of restricting user access by limiting the options presented (e.g., graying out menu items, using a kiosk-mode browser).                              |
| **Decentralized Access Control**                            | An access control model where authority and administration are distributed to local managers or departments.                                                   |
| **DIAMETER**                                                | A next-generation AAA protocol, based on RADIUS, designed to be more robust and flexible for modern networks.                                                  |
| **Discretionary Access Control (DAC)**                      | An access control model where the owner of a resource decides who can access it and can transfer those permissions.                                            |
| **Identification**                                          | The process by which a subject claims an identity (e.g., by providing a username).                                                                             |
| **Logical Access Control**                                  | Controls that restrict access to computer systems, networks, files, and data (e.g., passwords, encryption).                                                    |
| **Mandatory Access Control (MAC)**                          | A strict access control model where the system enforces access based on security labels (clearance levels and classifications).                                |
| **Multifactor Authentication (MFA)**                        | Authentication that requires two or more distinct factors (e.g., something you know, have, and are).                                                           |
| **Physical Access Control**                                 | Controls that restrict access to physical spaces and assets (e.g., locks, badges, gates).                                                                      |
| **Privacy**                                                 | The right of individuals to control or influence how their personal information is collected and used.                                                         |
| **Remote Authentication Dial-In User Service (RADIUS)**     | A widely used AAA protocol for managing network access authentication.                                                                                         |
| **Role-Based Access Control (RBAC)**                        | An access control model where permissions are assigned to roles, and users are assigned to roles, simplifying management.                                      |
| **Security Kernel**                                         | The core part of a system's hardware, software, and firmware that enforces access control policies (implements the reference monitor concept).                 |
| **Single Sign-On (SSO)**                                    | An authentication scheme that allows a user to log in once and gain access to multiple, related systems without re-authenticating.                             |
| **Smart Card**                                              | A physical card with an embedded microprocessor chip used for authentication (something you have).                                                             |
| **Terminal Access Controller Access System Plus (TACACS+)** | A Cisco-developed AAA protocol that separates authentication, authorization, and accounting processes, often used for network device administration.           |
| **Token**                                                   | A physical or software device used for authentication (something you have), often generating a one-time password.                                              |
