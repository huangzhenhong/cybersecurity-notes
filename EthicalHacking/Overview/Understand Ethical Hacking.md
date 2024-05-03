# Ethical Hacking

知己知彼，百战不怠；不知彼而知己，一胜一负；不知彼，不知己，每战必殆。 

If you know the enemy and know yourself, you need not fear the result of a hundred battles. If you know yourself but not the enemy, for every victory gained you will also suffer a defeat. If you know neither the enemy nor yourself, you will succumb in every battle. 

If it wasn't hard, everyone would do it, hard it what makes it great.

[Code of Ethics](https://www.eccouncil.org/code-of-ethics/)

![Code of Ethics](..\images\code-of-ethics.png)

## Classifying Information Security

### Fundamentals of Information Security
- Authenticity: We go through a verification process that requires a user to prove their identity or their claim to the rightful ownership of an account before access is actually denied;
- Integrity: Data is safe not altered
- Availability: Data is available whenever user wants it
- Confidentiality: Guarding against thief and unauthorized access of data
- Non-repudiation: Guaranteeing the data is not altered during transition

### Classifications
- Passive attacks(Sniffing or Evesdropping Attacks)
- Active attacks (DoS, Man in the Middle, SQL Injection)
- Close-in attacks (Social Engineering)
- Insider attacks (Misuse privileges)
- Distribution attacks

## Understanding the Attackers and Their Methods

### Hacking Frameworks 

Thinking like an attacker.

#### Cyber Kill Chain Methodology
- Reconnaissance: Getting as much information as I can about the intended victim;
- Weaponization: Analyzing the information that I gathered during the reconnaissance phase and identify the volunabilities and techniques that I can use to gain the access; 
- Delivery: deliverying the payload(link, email or usb drives etc.)
- Exploitation 
- Installation
- Command and Control (C&C)
- Action on Objectives

#### MITRE ATT&CK

https://attack.mitre.org/

Documents common tactics, techniques and procedures
- Tactics: The adversary's strategic goal 
- Techniques: The actions an adversary takes 
- Procedures: Carries out techniques or sub-techniques

#### Diamond Model of Intrusion Analysis
Provides a structure for identifying correlated groups of events 
![Diamond Model of Intrusion Analysis](..\images\diamond-model-of-intrusion-analysis.png)

- Tactics: The ways that the attackers operate during the different phases of the attack
- Techniques: Specific techniques which used by attackers during the execution
- Procedures: The sequences of actions that performed by the attackers to achieve certain goals.

#### Adversary Behavioral Identification 
- Internal Reconnaissance
    - Enumeration
        - OS
        - Services
        - Apps and versions
        - Hosts
        - Processes
        - User accounts
        - IP addresses
        - Host names
- PowerShell
- CLI processes
- Suspicious proxy events
- HTTP user agent
- C&C servers: C&C allows attackers to issue commands to hundreds of systems with one entry
- DNS Tunneling
    - Talk with C&C's
    - Bypass security controls
    - Monitor requests
    - DNS payloads
    - Destinations
- Web-shells: Attackers can control web servers by creating a shell within the website itself
- Data staging

#### Indicators of Compromise (IoC)
- Unauthorized software and files
- Suspicious emails 
- Suspicious registry and file system changes
- Unknown ports and protocol usage 
- Excessive bandwidth usage 
- Rogue hardware
- Service disruption and defacement
- Suspicious or unauthorized account usage

## Comparing Hacking and Ethical Hacking

### What is Hacking
- Exploiting systems vulnerabilities and security controls to gain access to system resources and features, outside the creator's original purpose.

### Types of Hackers
- Black Hats 
- White Hats 
- Gray Hats
- Suicide Hackers
- Script Kiddies
- Spy Hackers / Cyber Terrorists / State Sponsored Hackers

### Your Job (You can not stop them)
- Discourage 
- Detour
- Misdirect
- Slowdown

### Phases
- 1. Reconnaissance 
    - Passive
        - No direct interaction with the target
        - Research the company
    - Active
        - Direct interaction with the target
        - Engage and scans the network
- 2. Scanning
    - Gather info
        - ID systems
        - Vulnerabilities 
    - Tools Used
        - Port scanners 
        - Vulnerability scanners
- 3. Gaining Access 
- 4. Maintaining Access
    - PWNing the system (total control)
    - Use system as a launch pad
    - Inject backdoor/trojans
        - Used to revisit
        - Used to sniff/monitor network
    - Use resources
    - Harden up
- 5. Clearing Tracks
    - Destroy proof
    - Hide my stuff
    - Cyber blind

### What's Ethical Hacking
Involves the use of hacking methods and tools to discover weaknesses for system security

### What skills should an ethical hacker have?
- Expert with programs and networks
- Proficient with vulnerability research
- Mastery with diverse hacking techniques
- Follow a strict code of conduct
- Explicit permissions in writing
- Use the same tactics and stategies
- Just because you can, doesn't mean you can
- Report all of your results

## Describing Information Security Controls

### What Ethical Hackers Do

#### What ethical hackers do for companies
- Review systems and infrastructure
- Test current security (Penetration Test)
- Create solutions
    - Scope - define assests, networks and systems that can be targeted
    - Governance - Internal team in charge of polices and procedures
- Retest

#### You HAVE to answer questions like: 
- What can be seen?
- What is being monitored?
- What can be done?
- Is there adequate protection?
- Are compliances met?

### What is Defense in Depth

Defense in depth is a security strategy that involves multiple layers of security mechanisms to protect your information and systems. The idea is that if one layer of defense is breached, other layers will still provide protection. It's like having multiple barries to entry, each requiring different tools or methods to bypass.

For example, in a network security context, defense in depth might involve using firewalls, intrusion detection systems, and antivirus software at different points in the network. This approach makes it harder for attackers to penetrate the network and increases the chances of detecting and stopping them before they can cause harm.

In summary, defense in depth is about using a combination of security measures to create a stronger overall security posture.

### The levels of Defense in Depth

- 1. Policy, Procedures and Awareness: This level involves establishing security policies, standards, and procedures. It includes things like defining acceptable use policies, incident response procedures, and security awareness training for employees.
- 2. Physical Security: This level involves securing physical access to your facilities. It includes measures such as locks, access control systems, and security guards.
- 3. Perimeter Security: This level focuses on securing the external boundary of your network or physical location. It includes measures such as firewalls, intrusion detection systems, and access control mechanisms.
- 4. Network Security: This level involves securing the internal network against attacks. It includes things like network segmentation, virtual private networks (VPNs), and secure Wi-Fi protocols.
- 5. Host and Endpoint Security: This level focuses on securing individual devices such as computers, laptops, and mobile devices. It includes measures such as antivirus software, host-based firewalls, and device encryption.
- 6. Application Security: This level involves securing the software applications used in your environment. It includes measures such as secure coding practices, regular security testing (e.g., penetration testing), and patch management.
- 7. Data Security: This level focuses on securing data at rest, in transit, and in use. It includes measures such as encryption, data loss prevention (DLP) tools, and access controls.
- 8. Monitoring and Response: This level involves monitoring your environment for security breaches and responding to them in a timely manner. It includes things like security information and event management (SIEM) systems, log monitoring, and incident response procedures.

![Defense In Depth](../images/defense-in-depth.png)

#### Consider this 
- Never ignore the edge
- Follow the workflow
- Zero Trust Security Posture

### What is the Risk?

In the context of cybersecurity, risk refers to the potential for a security incident to result in harm to an organization's information, systems, or operations. This harm can take many forms, including financial loss, damage to reputation, legal consequences, and disruption of operations.
```
Risk = Threats * Vulnerabilities * Impact
```

### Threat Modeling

Threat modeling is a structured approach for identifying and prioritizing potential threats to a system, application, or organization. It helps organizations understand the potential vulnerabilities in their systems and prioritize their efforts to mitigate those vulnerabilities.

#### The process of threat modeling typically involves the following steps:

- Identifying Assets: Identify the assets that need to be protected, such as data, systems, and applications.
- Identifying Threats: Identify potential threats that could exploit vulnerabilities in the assets. This could include threats from malicious actors, natural disasters, or other sources.
- Identifying Vulnerabilities: Identify the vulnerabilities in the system that could be exploited by the threats. This could include software vulnerabilities, configuration weaknesses, or human factors.
- Assessing Risks: Assess the risks associated with each threat, taking into account the likelihood of the threat occurring and the potential impact it could have.
- Mitigation Strategies: Develop and prioritize mitigation strategies to address the most significant risks. This could include implementing security controls, improving processes, or reducing the attack surface.
- Review and Update: Regularly review and update the threat model to account for changes in the system or threat landscape.

Threat modeling is an important part of a comprehensive security program, as it helps organizations proactively identify and address security risks before they can be exploited by attackers.

### Incident Management

#### The "Why" of Incident Management
- Better service quality
- Proactive
- Reduces impact
- Meets availability
- More efficient and productive
- Customer/user satisfaction

### The Incident Handling and Response (IH&R)
- Prepare for Event Handling and Reaction 
    - Establish an incident response team with defined roles and responsibilities.
    - Develop an incident response plan that outlines the steps to be taken in the event of a security incident.
    - Conduct regular training and exercises to ensure that the incident response team is prepared to respond effectively.
- Incident Recording and Assignment
- Triage
- Notification
- Containment
    - Isolate the affected systems or networks to prevent further damage or spread of the incident.
    - Implement temporary fixes or workarounds to mitigate the immediate impact of the incident.
- Forensic Examination
- Eradication
    - Identify and remove the root cause of the incident from the affected systems.
    - Patch vulnerabilities, update configurations, or take other actions to prevent the incident from recurring.
- Recovery
    - Restore affected systems and services to normal operation.
    - Validate that the systems are functioning correctly and that the incident has been fully resolved.
- Post-incident Actions
    - Lessons Learned:
        - Conduct a post-incident review to analyze the incident response process and identify areas for improvement.
        - Update the incident response plan and implement any necessary changes to improve future incident response efforts.
    - Reporting and Communication:
        - Report the incident to appropriate stakeholders, including senior management, legal, and regulatory authorities as required.
        - Communicate with affected parties, such as customers or employees, as appropriate.

### Can AI and ML Stop Attacks?
- Authentication and password protection 
- Phishing
- Threat detection
- Vulnerability management
- Behavioral analysis
    - AI-based antivirus
    - Botnets
    - Fraud
    - Network security

## Differentiate Information Security Laws and Standards

### The standard for credit card processing
Payment Card Industry Data Security Standard (PCI DSS)
- Build and maintain a secure network
- Protect cardholder data 
- Maintain a Vulnerability Management Program(VMP)
- Strong access controls
- Monitor and test
- Information security policy

### ISO/IEC 27001:2013
- Security requirements and goals
- Cost-effective 
- Compliance
- New and existing InfoSec processes
- Status of InfoSec activities
- Provide InfoSec information to cusomers

### Health Insurance Portability and Accountability Act (HIPPAA)
- Electronic transaction and code set standards
- Privacy rule
- Security rule
- National identifier
- Enforcement rule

### Sarbanes-Oxley (SOX)

The Sarbanes-Oxley Act of 2002, often abbreviated as SOX, is a U.S. federal law enacted in response to a series of high-profile corporate scandals, such as those involving Enron, WorldCom, and Tyco International. The purpose of SOX is to protect investors by improving the accuracy and reliability of corporate disclosures.

Key provisions of the Sarbanes-Oxley Act include:

- Public Company Accounting Oversight Board (PCAOB): SOX established the PCAOB to oversee the auditing of public companies and to regulate the accounting industry.
- Corporate Responsibility: The act requires senior executives to take individual responsibility for the accuracy and completeness of corporate financial reports.
- Auditor Independence: SOX prohibits auditors from providing certain non-audit services to their audit clients, to ensure their independence and objectivity.
- Internal Controls: Companies are required to establish and maintain adequate internal controls over financial reporting and to regularly assess the effectiveness of these controls.
- Enhanced Financial Disclosures: SOX requires companies to provide more detailed and timely financial disclosures, including off-balance sheet transactions and pro forma figures.
- Whistleblower Protection: The act includes provisions to protect whistleblowers who report corporate fraud or misconduct.

SOX has had a significant impact on corporate governance and financial reporting practices in the United States. While it has been praised for improving transparency and accountability, some critics argue that it imposes unnecessary costs and regulatory burdens on companies.

### General Data Protection Regulation (GDPR)
- Lawfulness, transparency and fairness
- Purpose Limitation 
- Storage Limitation  
- Data minimization 
- Accuracy
- Accountability
- Integrity and confidentiality

### Data Protection Act 2018 (DPA)

The Data Protection Act 2018 is a piece of legislation in the United Kingdom that governs the processing of personal data. It was enacted to supplement the General Data Protection Regulation (GDPR) and provide additional details on how the GDPR should be implemented in the UK.


