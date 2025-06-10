# Week 1 - Threats & Security Concepts

**DAY 1 PURPOSE OF SECURITY- THE CIA TRIAD**

## CIA Triad
- **Confidentiality**: Prevent unauthorized access to sensitive info (e.g., encrypting data, strong passwords).
- **Integrity**: Ensure data hasn’t been tampered with (e.g., hashing files, digital signatures).
- **Availability**: Make sure systems/data are always usable when needed (e.g., using RAID, generators, cloud backups).


## Threat Actors
- Script kiddies : people with low knowledge, they hack systems with prebuilt tools. A good fire walling and good measures can stop them
- Hacktivists : Theyre intent and motivation is what you gotta know.
- Nation-state actors : Also known as Advanced Persistent threats(APTs), theyre well resourced groups that are directly or indirectly funded by government to commit cyberattacks.
- Insider threats : This is not always an employee. it can be a claaner or a customer, anyone who comes into the infrastructure or works in there.


## Types of Attacks
- Malware: Virus, Worm, Trojan
- Social Engineering: Phishing, Vishing, Pretexting
- Network Attacks: DDoS, MITM


## DAY 2 RISK AND RISK MANAGEMENT 
- **Risk** : the potential to cause harm
- **Assests** : are tangible & intangible part of an infrastructure that provides benefits to the organization. And assest can be a computer or a server and can also be an employee. people can be assests 
- **Threat** : Is someone or something that can cause harm to our infrastructure. It can be a volcano or an earthquake or an unauthorized individual walking into the server room.
- **Vulnerability** : Is an open door in an asset that can be exploited. it can be open doors to a server room or an threat actor exploiting...
- **impact** : the damage at which a risk can hit
- Threats exploit vulnerabilities to harm assets
### Threat * vulnerability = risk 
<!--- Go check up NIST SP 800-30 (talks about all threats and vulnerabilities a security could face)-->


## Day 3 – Social Engineering

- **Phishing**: Fake emails/messages to trick users.
- **Spear Phishing**: Targeted phishing with personal info. Email from your boss or something.
- **Vishing**: Voice phishing.
- **Smishing**: SMS-based phishing.
- **Pretexting**: Attacker lies to get info.
- **Tailgating**: Following someone into a secure area.
- **Shoulder Surfing**: Watching people enter info.
- **Dumpster Diving**: Digging through trash for data.

## Security Controls

**Types of Controls**
- **Administrative**: Policies and rules
- **Technical**: Software/hardware protection
- **Physical**: Physical security measures

**Control Categories**
- **Preventive**: Stop attack (e.g., firewall)
- **Detective**: Detect attack (e.g., IDS)
- **Corrective**: Recover from attack (e.g., restore backup)
- **Deterrent**: Discourage attack (e.g., signs)
- **Compensating**: Alternate control (e.g., cameras when no MFA)

## Day 4 Threat groups, vulnerabily assessments, Mitigations.
- **Adversarial** : Human based attacks. i.e hackers, insiders or malicious actors trying to break in
- **Environmental** : Natural disasters or weather . i.e floods, fire etc
- **structural** : These are failures in tech. e.g hardware & software crashed ...
- **Accidental** : Human errors. e.g, mistakingly deleting files or misconfigurations.

- **Threat Assessment** identifies potential attackers/harm sources. Goal is, Who might attack us?
- **Vulnerability Assessment** scabs for weaknesses. the goal is, Where are we exposed?

# Mitigation : What we do to reduce the risk impact or eliminate risk.

| **Risk Type** | **Mitigation** |
|---------------| ---------------|
| Unauthorized Access | RBAC, MFA |
| Malware Infection | Anti virus | 
| Power loss | Backup generator, UPS |
| Data loss | Backup, RAID, snapshots |
| Insider threats | Monitoring, Audit logs, user behavior analytics |

###Risk acceptance
Thats a situation where the risk we're facing is smaller to the cost for mitigation, that way we just accept the risk. E.g,  A small business decides not to buy a $10,000 advanced firewall because the data they're protecting isn't highly sensitive, and their existing controls (like basic router security) are “good enough” for the actual threat level.

## Day 5 – Risk Response Strategies

- **Avoidance**: Remove the risk (e.g., disabling features or blocking USB drives).
- **Transference**: Shift the risk to a third party (e.g., buying cyber insurance).
- **Mitigation**: Reduce the impact of the risk (e.g., using antivirus, applying patches).
- **Acceptance**: Accept the risk if the cost to fix is higher than the risk itself.

**Example**: A company accepts the risk of running a legacy application because it would cost too much to upgrade it — even though it’s vulnerable.


## Day 6 – Common Ports and Protocols 

| Port | Protocol | Description |
|------|----------|-------------|
| 20, 21 | FTP | File Transfer Protocol |
| 22 | SSH | Secure remote shell access |
| 23 | Telnet | Insecure remote login |
| 25 | SMTP | Send emails |
| 53 | DNS | Domain name resolution |
| 67/68 | DHCP | Assign IP addresses |
| 80 | HTTP | Unsecured web traffic |
| 110 | POP3 | Basic email retrieval |
| 143 | IMAP | Email sync |
| 443 | HTTPS | Secured web traffic |
| 445 | SMB | File sharing on Windows |
| 3389 | RDP | Remote Desktop access |
