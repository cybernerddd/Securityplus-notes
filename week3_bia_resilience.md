# NA-014 – Business Impact Analysis 

## Key Metrics:
- **RTO (Recovery Time Objective)**: How fast you must recover
- **RPO (Recovery Point Objective)**: How much data loss is acceptable
- **MTTR**: Time to repair a failure
- **MTTF**: Avg time before failure (non-repairable)
- **MTBF**: Time between repeated failures (repairable systems)

## Example:
If your RTO is 2 hours, and MTTR is 4 hours → You’re not meeting your recovery objectives.

## Impact Types:
- **Life**
- **Safety**
- **Finance**
- **Reputation**
- **Property**


# NA-015 – Security Controls and Resilience

## High Availability Tactics:
- **RAID**: Drive redundancy
- **Failover**: Auto-switch to backup system
- **Load Balancing**: Split traffic to prevent overload
- **Clustering**: Redundant systems acting as one
- **Snapshots**: Instant restore point

## Backup Types:
- Full: Everything every time
- Incremental: Since last backup
- Differential: Since last full backup

## Site Types:
- Cold: Just building
- Warm: Hardware, no data
- Hot: Fully ready, live data sync

# NA-016 – Security Awareness and Training

## Types of Training:
- Role-based training
- Phishing awareness
- Social engineering prevention
- Onboarding & refresher training

## Offboarding
- knowledge transfer
- disable account (never delete account)
- Return credentials 
- Exit interview
## Delivery Methods:
- Simulated phishing campaigns
- Security posters & reminders
- Intranet video portals
- Gamified rewards for good behavior

## Purpose:
- Reduce user error
- Catch phishing early
- Build a security-first culture

# NA-017 – Third Party Agreements & Risk Management

## Key Agreements:
- SLA: Defines services, uptime, response time
- MOU: Informal cooperation agreement
- MOA: Agreement with defined responsibilities
- NDA: Confidentiality contract
- ISA: Secure system interconnection rules
- BPA: Legal partnership terms

## Purpose:
- Clarify roles and liability
- Reduce risk from vendors
- Set expectations for uptime, security, and data handling

# NA-019 – Cryptography Basics

## 🧠 What is Cryptography?
- The science of securing information using encoding techniques
- Protects data confidentiality, integrity, authentication, non-repudiation

## 🔐 Classical Algorithms Covered:
- **Caesar Cipher** – shifts letters by a fixed value (simple, weak)
- **Vigenère Cipher** – uses keyword for polyalphabetic substitution
- **Binary Encryption** – represents characters as binary and manipulates with keys

## 💡 Cryptographic Terms:
- **Plaintext** – Readable data
- **Ciphertext** – Encrypted version of plaintext
- **Key** – Secret value used to encrypt/decrypt
- **Algorithm** – The math behind the encryption

## 🔄 States of Data:
- **Data in Use** – Data in RAM/CPU while being processed
- **Data at Rest** – Stored data (disk, database)
- **Data in Transit** – Data moving over networks

## 🛡️ Key Takeaways:
- Data in use is vulnerable → protect with application security and memory protections
- Data in transit must be encrypted (TLS/SSL, VPN)
- Symmetric = 1 key (e.g., AES), Asymmetric = 2 keys (e.g., RSA)
- Hashing ensures integrity (e.g., SHA-256)


# NA-020 – Cryptographic Methods & Key Exchange

## 🔁 Symmetric vs. Asymmetric

- **Symmetric**: Same key for encryption & decryption (e.g., AES)
- **Asymmetric**: Public key encrypts, private key decrypts (e.g., RSA)

## 🔐 Key Exchange

### In-Band:
- Key is shared over same channel as data
- Used in TLS/SSL (HTTPS)
- Less secure if connection is compromised

### Out-of-Band:
- Key is shared over separate channel
- Example: Password by phone, file by email
- Higher security, used in air-gapped or sensitive systems

## ⏳ Ephemeral Keys
- Temporary session keys
- Used once, then discarded
- Enables **Perfect Forward Secrecy**
- Common in modern TLS (DHE, ECDHE)

## 💡 Key Takeaway:
Key exchange is central to encryption. Ephemeral keys + asymmetric exchange = strong secure session setup.

