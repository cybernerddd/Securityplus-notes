# Week 2 – Day 1: Network Devices & Segmentation

## Firewalls
- Packet Filtering: Inspects packets without memory.
- Stateful: Tracks active sessions.
- NGFW: Filters by apps, behaviors, malware.
- Host-based vs Network-based firewalls.

## IDS vs IPS
- IDS: Detects & alerts. Passive.
- IPS: Detects & blocks. Active.

## VPN
- Encrypts traffic over untrusted networks.
- Types: Site-to-Site, Remote Access.

## Proxy Servers
- Forward Proxy: Controls outbound traffic.
- Reverse Proxy: Hides backend servers.
- Application Proxy: Filters by app type.

## Segmentation
- VLANs: Logical separation of network traffic.
- DMZ: Public zone separated from internal systems.
- Air Gap: No physical connection to external networks.

# switched up lanes (Day 2)

## NA-006 – Using Risk Assessment Guides

- **Standards**: International security models (e.g., ISO, NIST).
- **Frameworks**: Structured approach to security (e.g., NIST CSF, COBIT).
- **Benchmarks**: Specific configuration rules (e.g., CIS Benchmarks).
- **Baselines**: Minimum acceptable security levels (e.g., strong passwords, firewall enabled).

## NA-007 – Security Control Types

### Nature of Control:
- **Administrative**: Policies and procedures (e.g., training users, hiring practices).
- **Technical**: Tech-based defense (e.g., antivirus, firewalls).
- **Physical**: Physical protection (e.g., doors, fences, guards).

### Functional Categories:
- **Preventive**: Stops threats (e.g., MFA, firewall).
- **Detective**: Finds threats (e.g., IDS, CCTV logs).
- **Corrective**: Fixes issues after attacks (e.g., restore backup).
- **Deterrent**: Makes attacker back off (e.g., warning signs).
- **Compensating**: Backup measure when others can’t apply (e.g., camera instead of MFA).

## NA-008 - Interesting security controls (Day 3)
- **Mandatory Vacation**: Helps recognize if theres an insider among employees. Detects hidden fraud.
- **Job rotation**: periodically switching people around to work in different positions.
- **Multi-person control**: preventing a single person yo perform an action that could be bad. 
- **sepaaration of duties**: single individual should not participate in all duties across the board.(i.e security should do security, sales should do sales not intermixing).
-**principle of least privilege**: only give access needed to do the job.(e.g. interns shouldn't have admin rights)

## NA-009 – Defense in Depth

- Use of **multiple layers** of security to protect systems.
- No single control should be trusted to do everything.
- Layers include:
  - **Physical**: Locks, CCTV
  - **Network**: Firewalls, IDS, segmentation
  - **Host**: EDR, antivirus
  - **App**: Input validation, auth checks
  - **Data**: Encryption, backups
  - **Policy/Admin**: User training, least privilege

**Goal**: Slow attackers down, detect early, and minimize damage.

## NA-010 – IT Security Governance (Day 4)

### Key Roles:
- **Senior Management**: Owns organizational risk, final authority.
- **Security Officer (CISO)**: Creates and enforces security policies.
- **Data Owner**: Classifies data, sets handling policies.
- **Data Custodian**: Implements technical controls and stores data.
- **System Owner**: Owns actual systems/platforms.
- **User**: Follows policies and uses resources appropriately.
- **Auditor**: Ensures compliance and reviews controls.

## NA-011 – Security Policies

- **Acceptable Use Policy (AUP)**: Defines what users can/cannot do on org systems.
- **Password Policy**: Sets complexity, length, and reset requirements.
- **Data Classification Policy**: Establishes labels like Public, Internal, Confidential.
- **Privacy Policy**: Governs how personal/user data is handled.
- **Security Awareness Policy**: Outlines user training frequency and topics.
- **Clean Desk Policy**: Requires physical removal of sensitive info from unattended workspaces.

# NA-012 – Security Frameworks and RMF (Day 5)

## 🔐 NIST SP 800-37 – Risk Management Framework (RMF)

This is a 6-step cycle used to manage cybersecurity risk in U.S. federal systems.  
It’s widely used in both government and private sectors.

### 📍 The 6 Steps of RMF (NIST 800-37):
1. **Categorize** – Identify and label systems based on impact (low/med/high)
2. **Select** – Choose appropriate security controls (from NIST 800-53)
3. **Implement** – Apply the selected controls
4. **Assess** – Evaluate control effectiveness (usually via audit or testing)
5. **Authorize** – Decide whether the system is approved to operate (ATO)
6. **Monitor** – Continuously track control performance, make updates

---

## 📚 Related Frameworks

| Framework | Purpose |
|----------|---------|
| **NIST SP 800-53** | Catalog of security controls (used in RMF step 2) |
| **NIST CSF** | High-level, business-friendly cybersecurity framework (Identify, Protect, Detect, Respond, Recover) |
| **ISO/IEC 27001** | Global standard for InfoSec management |
| **COBIT** | Aligns IT + security controls with business goals |
| **CIS Controls** | 18 prioritized best practices (used in SMBs) |
| **PCI DSS** | Credit card security standard (required by payment processors) |

---

## 🎯 Key Concept:

- **NIST 800-37** tells you *how to run a secure system lifecycle*  
- **NIST 800-53** tells you *what specific controls to apply*

# NA-013 – Quantitative Risk Calculations

## Key Formulas:

- **SLE = Asset Value × Exposure Factor**
- **ALE = SLE × ARO**
- **MTBF = MTTF + MTTR**

## Definitions:
- **MTTF** – Avg time before failure (non-repairable)
- **MTTR** – Avg time to fix something
- **MTBF** – Time between one fix and the next failure

## Example:
- Server = $10,000
- Exposure Factor = 0.3
- ARO = 2/year

→ SLE = $3,000  
→ ALE = $6,000/year  
→ If MTTF = 100 hours, MTTR = 5 hours, MTBF = 105 hours
