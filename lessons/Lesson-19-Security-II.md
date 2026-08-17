# Lesson 19 — Security II

## 📖 Microsoft Learn

**Module:** Secure Your Cloud Data  
https://learn.microsoft.com/en-us/training/modules/secure-your-cloud-data/

### Focus
- Network Security Groups (NSGs)
- Azure Firewall
- Azure DDoS Protection
- Azure Key Vault
- Microsoft Sentinel
- Azure Dedicated Hosts
- Encryption, Secrets, and Certificates
- Microsoft Entra ID Protection

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Functionality and Usage of NSGs | 8:32 | https://youtu.be/flCoRc1uv9o |
| Functionality and Usage of Azure Firewall | 5:02 | https://youtu.be/1-_cqpUISg4 |
| Functionality and Usage of Azure DDoS Protection | 6:30 | https://youtu.be/6cv-wdo9TJw |
| Functionality and Usage of Azure Key Vault | 7:37 | https://youtu.be/ZBXVAD4S0Tc |
| Functionality and Usage of Microsoft Sentinel | 9:36 | https://youtu.be/xaqiPXL6tz0 |
| Functionality and Usage of Azure Dedicated Hosts | 6:49 | https://youtu.be/RnNqmTH9xok |

---

# Azure Security Services

Azure provides security services that protect different parts of a cloud environment.

```text
Network Traffic
    |
    +-- Network Security Groups
    +-- Azure Firewall
    +-- Azure DDoS Protection

Sensitive Information
    |
    +-- Azure Key Vault

Security Monitoring
    |
    +-- Microsoft Sentinel

Compute Isolation
    |
    +-- Azure Dedicated Hosts

Identity Risk
    |
    +-- Microsoft Entra ID Protection
```

The key to AZ-900 questions is recognizing **what each service protects** and **which problem it is designed to solve**.

---

# Network Security Groups (NSGs)

A **Network Security Group (NSG)** controls inbound and outbound network traffic to supported Azure resources.

NSGs use **security rules** to allow or deny traffic.

Rules can evaluate information such as:

- Source
- Destination
- Port
- Protocol
- Direction
- Priority
- Allow or deny action

### Exam Thinking

> **NSG = allow or deny inbound and outbound network traffic.**

---

# Inbound and Outbound Rules

## Inbound Rules

Control traffic coming **into** a protected resource.

```text
Internet
   |
   v
[ NSG ]
   |
   v
Azure Resource
```

## Outbound Rules

Control traffic leaving a protected resource.

```text
Azure Resource
   |
   v
[ NSG ]
   |
   v
Destination
```

### Memory Trick

```text
Inbound  = Traffic coming IN
Outbound = Traffic going OUT
```

---

# NSG Rule Priority

NSG rules have a **priority**.

Rules are evaluated in priority order, and lower numbers have higher priority.

When a matching rule is found, Azure applies that rule.

### Exam Thinking

> **Lower NSG priority number = evaluated before a higher number.**

---

# Default NSG Rules

Azure NSGs include default security rules.

These provide baseline behavior for traffic within the virtual network, Azure load balancers, and other traffic.

Custom rules can be created with higher priority than default rules.

For AZ-900, you do not need to memorize every default rule number.

### Exam Thinking

> **NSGs contain default rules and can also contain custom rules.**

---

# Azure Firewall

**Azure Firewall** is a managed, cloud-based network security service that helps protect Azure network resources.

It can centrally control network traffic using firewall rules.

### Common Uses

Azure Firewall can help:

- Control network traffic.
- Filter traffic centrally.
- Apply network and application rules.
- Protect multiple workloads through centralized policy.

### Real-World Thinking

An organization has many Azure workloads and wants centralized firewall protection rather than configuring every workload independently.

Azure Firewall is designed for this type of scenario.

### Exam Thinking

> **Azure Firewall = managed, centralized network firewall.**

---

# NSG vs. Azure Firewall

Both can control network traffic, but they serve different roles.

| Feature | Main Purpose |
|---|---|
| **NSG** | Allow or deny traffic for network interfaces/subnets using security rules |
| **Azure Firewall** | Centralized managed firewall protection and traffic filtering |

### Easy Way to Remember

```text
NSG            = RESOURCE / SUBNET TRAFFIC RULES
Azure Firewall = CENTRAL NETWORK FIREWALL
```

---

# Azure DDoS Protection

A **Distributed Denial-of-Service (DDoS)** attack attempts to overwhelm an application or network resource with large amounts of traffic so legitimate users cannot access it.

**Azure DDoS Protection** helps protect Azure resources against DDoS attacks.

### Real-World Thinking

A public-facing application is targeted by a massive flood of malicious network traffic.

Azure DDoS Protection is designed to help mitigate this type of attack.

### Exam Thinking

> **Azure DDoS Protection = protect against Distributed Denial-of-Service attacks.**

---

# Firewall vs. DDoS Protection

These are different security problems.

```text
Azure Firewall
    |
    +-- Filter and control network traffic

Azure DDoS Protection
    |
    +-- Protect against traffic-flood attacks
```

### Exam Thinking

> **Firewall = filter traffic. DDoS Protection = mitigate overwhelming attacks.**

---

# Azure Key Vault

**Azure Key Vault** is a cloud service used to securely store and manage sensitive information.

It can store and manage:

- Secrets
- Cryptographic keys
- Certificates

```text
Azure Key Vault
      |
      +-- Secrets
      +-- Keys
      +-- Certificates
```

This helps prevent sensitive values from being stored directly inside application code or configuration files.

### Exam Thinking

> **Azure Key Vault = securely store secrets, keys, and certificates.**

---

# Secrets

**Secrets** are sensitive values used by applications or users.

Examples include:

- Passwords
- API keys
- Connection strings
- Access tokens

### Bad Approach

```text
Application Code
DatabasePassword = "MyPassword123"
```

### Better Approach

```text
Application
    |
    v
Azure Key Vault
    |
    v
Retrieve Authorized Secret
```

### Exam Thinking

> **Secret = sensitive credential or value.**

---

# Cryptographic Keys

Cryptographic keys are used by encryption systems to help protect data.

Azure Key Vault can securely create, store, and manage supported keys.

### Exam Thinking

> **Key = cryptographic material used to protect data.**

---

# Certificates

**Certificates** are digital credentials used to establish trust and support secure communication.

Common uses include:

- HTTPS websites
- Application authentication
- Secure network connections

Azure Key Vault can securely store and manage certificates.

### Exam Thinking

> **Certificate = establishes identity/trust and helps secure communication.**

---

# Encryption

**Encryption** converts readable information into an unreadable form so unauthorized users cannot understand it.

```text
Plaintext
   |
   v
Encryption
   |
   v
Ciphertext
```

An appropriate key is required to decrypt the protected data.

Azure commonly protects data:

- **At rest** — while stored.
- **In transit** — while moving across a network.

### Memory Trick

```text
At Rest    = STORED
In Transit = MOVING
```

### Exam Thinking

> **Encryption = protect data by making it unreadable without the appropriate key.**

---

# Key Vault Security and Recovery

Azure Key Vault integrates with Microsoft Entra ID for authentication and supports authorization mechanisms for controlling access.

Key Vault also includes recovery features such as:

- Soft delete
- Purge protection

These features can help protect important vault objects from accidental or malicious deletion.

> [!NOTE]
> Azure Key Vault capabilities, tiers, authorization options, and pricing can change. For AZ-900, focus primarily on **what Key Vault protects** rather than memorizing detailed pricing or configuration.

---

# Microsoft Sentinel

**Microsoft Sentinel** is Microsoft's cloud-native **Security Information and Event Management (SIEM)** and security orchestration, automation, and response solution.

Sentinel can collect and analyze security data from many sources.

It helps security teams:

- Detect threats.
- Investigate incidents.
- Correlate security events.
- Respond to security incidents.
- Automate supported security workflows.

### Exam Thinking

> **Microsoft Sentinel = cloud-native SIEM and security operations platform.**

---

# What Is SIEM?

**SIEM** stands for:

> **Security Information and Event Management**

A SIEM collects security information from multiple systems and helps analysts detect and investigate suspicious activity.

```text
Identity Logs --------\
Firewall Logs ---------\
Cloud Logs ------------- > Microsoft Sentinel
Application Logs -------/        |
Endpoint Logs ---------/         v
                             Detection
                             Investigation
                             Response
```

### Exam Thinking

> **SIEM = collect and analyze security events from many sources.**

---

# Azure Dedicated Hosts

**Azure Dedicated Hosts** provide physical servers dedicated to a single Azure customer for hosting Azure virtual machines.

Normally, public-cloud physical infrastructure is shared across customers while workloads remain logically isolated.

A Dedicated Host provides dedicated physical server capacity for an organization.

### Common Reasons

Organizations may use Dedicated Hosts for:

- Physical server isolation.
- Certain compliance requirements.
- Licensing requirements.
- Greater control over VM placement.

### Exam Thinking

> **Azure Dedicated Host = physical server dedicated to one customer.**

---

# Dedicated Host vs. Virtual Machine

A Virtual Machine provides a virtualized computer.

A Dedicated Host provides the **physical server** on which supported Azure VMs can run.

```text
Standard Azure VM
VM runs on shared Azure infrastructure
(logically isolated)

Dedicated Host
Physical server dedicated to one customer
```

### Exam Thinking

> **VM = virtual compute. Dedicated Host = dedicated physical host for VMs.**

---

# Microsoft Entra ID Protection

**Microsoft Entra ID Protection** helps organizations detect, investigate, and respond to identity-based risks.

It can identify signals involving:

- Risky users
- Risky sign-ins
- Suspicious identity activity

Organizations can use identity-risk information to help protect user accounts.

### Real-World Thinking

A user's sign-in behavior appears suspicious or indicates that the account may be compromised.

Identity Protection can help identify and respond to that risk.

### Exam Thinking

> **Identity Protection = detect and respond to identity risk.**

---

# Encryption vs. Secrets vs. Certificates vs. Identity Protection

These concepts solve different security problems.

| Concept | Primary Purpose |
|---|---|
| **Encryption** | Protect data from unauthorized reading |
| **Secrets** | Store sensitive credentials and values |
| **Certificates** | Establish trust and secure communications |
| **Identity Protection** | Detect identity and sign-in risks |

### Memory Trick

```text
Encryption          = PROTECT DATA
Secrets             = PROTECT CREDENTIALS
Certificates        = ESTABLISH TRUST
Identity Protection = DETECT IDENTITY RISK
```

---

# Key Vault vs. Sentinel

These services are very different.

| Service | Primary Purpose |
|---|---|
| **Azure Key Vault** | Protect secrets, keys, and certificates |
| **Microsoft Sentinel** | Detect, investigate, and respond to security threats |

### Memory Trick

```text
Key Vault = STORE SENSITIVE ITEMS
Sentinel  = WATCH SECURITY EVENTS
```

---

# Security Service Scenario Guide

### Think NSG when:
- You need inbound or outbound allow/deny network rules.
- Traffic should be controlled for a subnet or network interface.

### Think Azure Firewall when:
- You need centralized managed firewall protection.
- Network traffic needs centralized filtering.

### Think Azure DDoS Protection when:
- The concern is a large-scale traffic-flood attack.

### Think Azure Key Vault when:
- Passwords, API keys, encryption keys, or certificates must be stored securely.

### Think Microsoft Sentinel when:
- Security events from multiple systems need to be collected and analyzed.
- The organization needs SIEM capabilities.

### Think Azure Dedicated Hosts when:
- Dedicated physical server hardware is required for Azure VMs.

### Think Microsoft Entra ID Protection when:
- The concern is risky users, suspicious sign-ins, or compromised identities.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 19 Lab — Security II](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-19-Lab-19-Security-II.md)**

### Lab Focus

- Create and inspect a Network Security Group.
- Review default inbound and outbound rules.
- Create and remove a temporary NSG rule.
- Browse Azure Firewall.
- Review Azure DDoS Protection.
- Browse Azure Key Vault.
- Browse Microsoft Sentinel.
- Review Azure Dedicated Hosts.
- Practice security-service scenarios.

> [!TIP]
> Most sections are exploration-based. The NSG exercise is the only section that asks you to create a temporary resource and rule, and both can be removed when finished.

---

# Quick Check

| Need | Azure Service / Concept |
|---|---|
| Control inbound and outbound traffic | Network Security Group |
| Centralized managed firewall | Azure Firewall |
| Protect against traffic-flood attacks | Azure DDoS Protection |
| Store secrets, keys, and certificates | Azure Key Vault |
| Cloud-native SIEM | Microsoft Sentinel |
| Dedicated physical server for Azure VMs | Azure Dedicated Host |
| Protect data from unauthorized reading | Encryption |
| Detect risky identities and sign-ins | Microsoft Entra ID Protection |

---

# Before Moving On

You should be able to:

- Explain Network Security Groups.
- Explain inbound and outbound NSG rules.
- Explain Azure Firewall.
- Explain Azure DDoS Protection.
- Explain Azure Key Vault.
- Explain secrets, keys, certificates, and encryption.
- Explain Microsoft Sentinel and SIEM.
- Explain Azure Dedicated Hosts.
- Explain Microsoft Entra ID Protection.
- Know which Azure security service fits common business scenarios.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **NSG** | Allow/deny network traffic |
| **Azure Firewall** | Central managed firewall |
| **DDoS Protection** | Protect against traffic-flood attacks |
| **Key Vault** | Secrets, keys, certificates |
| **Encryption** | Protect data |
| **Sentinel** | SIEM / security operations |
| **Dedicated Host** | Dedicated physical Azure server |
| **Identity Protection** | Detect risky identities |
