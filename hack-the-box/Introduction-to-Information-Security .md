# Structure of InfoSec

---

Information Security (InfoSec) is the field responsible for protecting information and systems from unauthorized access, modification, or destruction.

It is important to understand how the digital world is structured and how its different components are connected, such as:

- `Client` → A PC or laptop used to access resources and services on the Internet.
- `Internet` → A large interconnected network of servers that provide different services and applications.
- `Servers` → Systems that provide services and applications designed to perform specific tasks, such as web servers.
- `Network` → Multiple computers or servers connected and able to communicate with each other.
- `Cloud` → Data centers that provide interconnected servers for companies and individuals.
- `Blue Team` → Responsible for defending the organization against cyber attacks.
- `Red Team` → Simulates real attacks against the organization.
- `Purple Team` → Combines Blue Team and Red Team members to improve the organization's security.

---

## Areas of Information Security

InfoSec protects the:

- `Confidentiality` → Prevents unauthorized access to information.
- `Integrity` → Protects information from unauthorized modification.
- `Availability` → Ensures that information and systems are accessible when needed.

Some of the main areas of InfoSec include:

1. Network Security
2. Application Security
3. Operational Security
4. Disaster Recovery and Business Continuity
5. Cloud Security
6. Physical Security
7. Mobile Security
8. Internet of Things (IoT) Security

---

## Security Concepts

Three important concepts in information security are:

### Risk

A `risk` represents the potential for damage to an organization's assets.

Risk considers:

- The likelihood of an event occurring.
- The severity of its impact.

Risk includes both threats and vulnerabilities.

### Threat

A `threat` is a potential cause of an incident that could harm a system or organization.

Examples include:

- Cybercriminals
- Hackers
- Fire
- Floods

Threats can exploit vulnerabilities to compromise a system.

### Vulnerability

A `vulnerability` is a weakness in a system that can be exploited by a threat.

Examples include:

- Software bugs
- Misconfigurations
- Weak passwords

A vulnerability does not necessarily mean that a system will be compromised. There must also be a threat capable of exploiting it.

### Relationship Between Them

```text
Vulnerability → Weakness in the system
Threat        → Something that can exploit the weakness
Risk          → Potential damage caused by the threat exploiting the vulnerability
```
## Roles in Information Security

There are many different roles within Information Security, each with different responsibilities.

| Role | Description |
| --- | --- |
| `Chief Information Security Officer (CISO)` | Oversees the entire information security program and establishes the overall security strategy. |
| `Security Architect` | Designs secure systems and networks. |
| `Penetration Tester` | Identifies vulnerabilities through simulated attacks in a legal and ethical manner. |
| `Incident Response Specialist` | Manages and responds to security incidents. |
| `Security Analyst` | Monitors systems for threats and analyzes security data. |
| `Compliance Specialist` | Ensures that the organization follows security standards and regulations. |

# Principles of Information Security

---

Information Security (InfoSec) is based on several fundamental principles used to protect information and systems.

## 6 Principles of Information Security

1. **Confidentiality**
   - Ensures that information is only accessible to authorized users.
   - Protects against unauthorized disclosure.
   - Common implementations: encryption and access controls.

2. **Integrity**
   - Ensures that data remains accurate and complete.
   - Protects against unauthorized modifications.
   - Common implementations: hashing and digital signatures.

3. **Availability**
   - Ensures that authorized users can access information when needed.
   - Protects against disruptions.
   - Common implementations: redundancy and disaster recovery.

4. **Non-repudiation**
   - Ensures that a person cannot deny the authenticity of a signature or a message they sent.
   - Important in legal and e-commerce contexts.
   - Common implementations: digital signatures and audit logs.

5. **Authentication**
   - Verifies the identity of a user, process, or device.
   - Ensures that only authorized entities can access resources.
   - Common implementations: passwords, biometrics, and multi-factor authentication.

6. **Privacy**
   - Focuses on properly handling sensitive personal information.
   - Helps organizations comply with data protection regulations.
   - Common implementations: data minimization and consent management.

---

### Processes in Information Security

InfoSec also involves several processes used to protect an organization's systems and data:

1. **Risk Assessment**
   - Identifies and evaluates threats and vulnerabilities.
   - Determines the potential impact of security breaches.
   - Helps prioritize security efforts.

2. **Security Planning**
   - Develops strategies to address identified risks.
   - Creates security policies and procedures.
   - Allocates resources for security initiatives.

3. **Implementation of Security Controls**
   - Puts security plans into practice.
   - Includes technical solutions and security policies.
   - Uses preventive and detective controls.

4. **Monitoring and Detection**
   - Continuously monitors security events and anomalies.
   - Uses tools such as SIEM and IDS.
   - Helps identify security incidents quickly.

5. **Incident Response**
   - Responds to detected security incidents.
   - Contains and mitigates threats.
   - Includes isolation, eradication, and recovery.

6. **Disaster Recovery**
   - Restores systems and data after major incidents.
   - Uses backups and redundancy.
   - Reduces downtime and data loss.

7. **Continuous Improvement**
   - Learns from security incidents and near-misses.
   - Updates security measures according to new threats and technologies.
   - Includes regular assessments and audits.

---

### Purpose of Information Security

The main purposes of InfoSec are:

- **Protect sensitive data**
  - Prevent unauthorized access to personal data, financial records, and trade secrets.

- **Ensure business continuity**
  - Keep critical systems and data available during incidents or disasters.

- **Maintain regulatory compliance**
  - Follow laws and industry standards related to data protection.

- **Preserve brand reputation**
  - Prevent reputational damage caused by security breaches.

- **Safeguard intellectual property**
  - Protect ideas, inventions, and creative works from theft or unauthorized use.

- **Enable secure digital transformation**
  - Allow organizations to adopt new technologies while managing security risks.

---

### Tools in Information Security

InfoSec professionals use many different tools:

- **Firewalls** — Control incoming and outgoing network traffic.
- **IDS/IPS** — Monitor and block suspicious activities.
- **SIEM** — Collect and analyze security event data.
- **Vulnerability Scanners** — Identify potential weaknesses in systems and applications.
- **Penetration Testing Tools** — Simulate attacks to identify vulnerabilities.
- **Encryption Tools** — Protect data confidentiality and integrity.
- **Access Control Systems** — Manage permissions and authentication.
- **Security Awareness Platforms** — Educate users about security best practices.

### Common Penetration Testing Tools

- **Nmap** — Network scanning and discovery.
- **Wireshark** — Network protocol analysis.
- **Metasploit** — Exploitation framework.
- **Burp Suite** — Web application security testing.
- **John the Ripper** — Password cracking.

> **Note:** Penetration testing tools must only be used with proper authorization. Unauthorized security testing can have legal consequences

# Network Security

---

Network Security is a fundamental part of Information Security that protects computer networks, devices, and the data transmitted through them from internal and external threats.

It uses different tools and techniques to detect, prevent, and defend against security threats.

## Key Elements of Network Security

| Element | Description |
|---|---|
| `Firewalls` | Act as barriers between trusted internal networks and untrusted external networks. They filter network traffic based on predefined security rules. |
| `IDS/IPS` | Monitor network traffic for suspicious activities. IDS detects threats, while IPS can also take automated actions to block them. |
| `VPNs` | Provide secure and encrypted connections over public networks, protecting data during transmission. |
| `Access Control` | Uses authentication and authorization to ensure that only legitimate users can access network resources. |
| `Encryption` | Protects sensitive data both during transmission and while stored, making it unreadable to unauthorized users. |

---

### Network Security Threats

Cybersecurity threats can include:

- **Ransomware**
- **Data theft**
- **State-sponsored espionage**
- **Hacktivism**
- **Unauthorized network access**

A successful network breach can result in:

- Financial losses
- Reputation damage
- Legal liabilities
- Operational disruptions
- Loss of sensitive information

The attack surface has also increased because of technologies such as:

- Cloud computing
- Internet of Things (IoT)
- Remote work

Because of this, comprehensive network security is essential for protecting valuable assets and maintaining business continuity.

---

### Firewalls

A firewall is an important first line of defense that filters network traffic between trusted and untrusted networks.

However, a firewall does **not** provide complete protection. Cybercriminals can use advanced techniques to bypass firewall protections, so organizations need multiple security mechanisms instead of relying on a single security control.


## Responsibility

Network security is generally managed by an organization's **IT department**, specifically the **Network Security Team**.

The Network Security Team is responsible for:

- Designing network security infrastructure.
- Implementing security controls.
- Configuring and managing security devices.
- Developing and enforcing security policies.
- Monitoring network traffic.
- Detecting potential threats.
- Responding to security incidents.

The team is often led by a **Network Security Manager**, who may report to the **CISO (Chief Information Security Officer)**.

# Application Security

---

Application Security is the process of protecting applications from security threats and vulnerabilities throughout their entire lifecycle.

The main idea is that security should be considered from the beginning of the application development process, rather than being added only after the application has already been created.

We can compare an application to a house. When building a house, security should be considered from the beginning. Doors, locks, windows, alarms, and other security measures should be included in the design. If we build the entire house first and only think about security afterward, fixing vulnerabilities can be much more difficult and expensive.

The same applies to applications. Developers should consider security while designing, developing, testing, and maintaining the application.

If security is not considered from the beginning, vulnerabilities may remain in the application and could later be exploited by attackers.

A successful attack against an application can have serious consequences for an organization, including:

- Financial losses
- Data breaches
- Damage to the company's reputation
- Loss of customer trust
- Operational disruptions
- Legal or regulatory consequences

For this reason, application security is an important part of cybersecurity. Organizations need to continuously identify vulnerabilities, test their applications, and improve their security throughout the application's lifecycle.

The goal is not only to fix vulnerabilities after they are discovered, but to build applications with security in mind from the beginning.

# Operational Security

---

Operational Security (`OpSec`) is the process of protecting an organization's critical information and assets during its day-to-day operations.

The main idea is to identify what information is important, understand what could happen to it, identify its vulnerabilities, and apply the appropriate security measures to protect it.

OpSec is a continuous process because threats and the organization's environment can change over time.

## OpSec Process

The OpSec process can be divided into several steps:

1. `Assets Identification`
   - Identify the information and assets that are important and need to be protected.
   - These can include sensitive or critical information.

2. `Threat Identification`
   - Identify what could go wrong with the important assets.
   - Determine the possible threats that could affect the organization's information.

3. `Vulnerability Identification`
   - Identify weaknesses that could allow threats to affect the organization's assets.
   - Security measures can then be implemented to reduce these risks.

4. `Access Control`
   - Determine who should have access to specific information and systems.
   - Only authorized users should have the permissions necessary for their roles.
   - Authentication and authorization mechanisms can be used to control access.

5. `Monitoring`
   - Continuously monitor the environment for unauthorized access or new threats.
   - Security measures can be adjusted when new threats or changes appear.

---

## Important Components of OpSec

`Access Control` is an important part of OpSec because organizations need to determine who can access specific information and systems.

`Asset Management` involves maintaining an up-to-date inventory of the organization's hardware, software, and data. Knowing what assets exist, where they are, and how important they are helps organizations apply appropriate security measures.

`Change Management` ensures that changes to systems and processes are performed in a controlled way. Changes should be properly tested and approved to prevent new security vulnerabilities from being introduced.

`Security Awareness Training` helps employees understand their role in maintaining security. This includes learning about phishing attacks, strong passwords, and the proper handling of sensitive information.

---

## OpSec Responsibility

The responsibility for OpSec typically falls under the Information Security team, led by the Chief Information Security Officer (`CISO`).

However, OpSec is not only the responsibility of the security team. It requires cooperation from all levels of the organization, including employees and executives.

Security teams or external security consultants can test OpSec through security assessments and penetration testing. These tests can help identify weaknesses before real attackers can exploit them.

# Disaster Recovery and Business Continuity

---

`Disaster Recovery (DR)` and `Business Continuity (BC)` are important parts of an organization's security and resilience strategy. Their purpose is to help a company continue operating when significant problems or disruptions occur.

## Disaster Recovery (DR)

`Disaster Recovery` focuses on **recovering critical systems and data after a disaster or major incident**.

A disaster could be:

- Natural disasters, such as earthquakes or floods
- Fires or other physical disasters
- Major system failures
- Cyberattacks

The main goal of DR is to **minimize downtime and data loss** and restore important systems as quickly as possible.

A DR plan can include:

- Backing up data
- Replicating systems
- Using alternate systems or locations
- Recovering critical services after an incident

## Business Continuity (BC)

`Business Continuity` is broader than Disaster Recovery. It focuses on **keeping the business operating during and after a disruption**.

For example, a company could:

- Allow employees to work from home
- Use alternative suppliers
- Move operations to a temporary office
- Use alternative systems or procedures

The goal is to ensure that the business can continue operating even when normal operations are disrupted.

## Responsibility

DR and BC are usually managed by a dedicated team, often led by a `Business Continuity Manager`.

This team works with IT, operations, and executive leadership to:

- Identify critical business functions
- Assess risks
- Create recovery strategies
- Define `Recovery Time Objectives (RTOs)`
- Define `Recovery Point Objectives (RPOs)`
- Test recovery procedures

Penetration testers can also help by identifying vulnerabilities that could affect the organization's DR and BC plans and by testing whether recovery procedures work effectively.

Regular testing is important to make sure the plans are effective and that employees know what to do during a crisis.

# Cloud Security

---

`Cloud Security` is about protecting data and applications that are stored in the cloud.

The cloud can be compared to a **shared storage facility** where we keep important belongings. Since other people also use the same facility, security measures are necessary to prevent unauthorized access.

Cloud security follows the `shared responsibility model`:

- The `Cloud Service Provider` is responsible for securing the cloud infrastructure.
- The `Customer / Administrator` is responsible for securing their own data, applications, passwords, and user access.
- `Security Teams` plan and oversee security measures, perform risk assessments, and ensure that security is maintained.

## Common Cloud Security Risks

Some of the risks mentioned in the module are:

- `Data Breach`: Unauthorized individuals gain access to sensitive information.
- `Insecure APIs`: Vulnerabilities in APIs can be exploited by attackers.
- `Misconfigured Cloud Storage`: Incorrect settings can unintentionally expose data.
- `Account Hijacking`: Attackers gain control of an account and access its data.

## Key Areas of Cloud Security

### Data Protection

`Data Protection` protects data using encryption.

Data should be protected:

- `At Rest`: When the data is stored.
- `In Transit`: When the data is being transferred.

### Identity and Access Management

`Identity and Access Management (IAM)` ensures that only authorized individuals can access cloud resources.

### Network Security

`Network Security` protects data as it moves through the network.

It includes:

- `Firewalls`
- `VPNs`

### Compliance and Governance

`Compliance and Governance` involves following laws, regulations, and industry standards related to how data is handled and secured.
