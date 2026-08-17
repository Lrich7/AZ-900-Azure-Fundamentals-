[Lesson-18-Security-I.md](https://github.com/user-attachments/files/31148996/Lesson-18-Security-I.md)
# Lesson 18 — Security I

## 📖 Microsoft Learn

**Module:** Azure Security Fundamentals  
https://learn.microsoft.com/en-us/training/modules/azure-security-fundamentals/

**Documentation:** Microsoft Defender for Cloud  
https://learn.microsoft.com/en-us/azure/defender-for-cloud/

### Focus
- Microsoft Defender for Cloud
- Defense in Depth
- Zero Trust
- Secure Score

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Functionality of Microsoft Defender for Cloud | 9:47 | https://youtu.be/eWcoMi_nQt4 |
| Concept of Defense in Depth | 7:17 | https://youtu.be/CHKS2FcEMek |
| Describe the Concept of Zero Trust | 8:13 | https://youtu.be/JX3w4to-qgo |

---

# Azure Security Fundamentals

Cloud security is not based on a single security product or control.

Azure security uses multiple technologies, processes, and security principles to help protect:

- Identities
- Networks
- Compute resources
- Applications
- Data
- Cloud environments

Three important concepts for this lesson are:

```text
Microsoft Defender for Cloud
        |
        +-- Security posture
        +-- Recommendations
        +-- Workload protection

Defense in Depth
        |
        +-- Multiple security layers

Zero Trust
        |
        +-- Never trust
        +-- Always verify
```

---

# Microsoft Defender for Cloud

**Microsoft Defender for Cloud** is a cloud-native application protection platform that helps organizations improve security posture and protect cloud workloads.

It can provide security capabilities across:

- Azure
- Hybrid environments
- Supported multicloud environments

Defender for Cloud combines capabilities for:

- **Cloud Security Posture Management (CSPM)**
- **Cloud Workload Protection (CWP)**

### Exam Thinking

> **Microsoft Defender for Cloud = improve cloud security posture and protect cloud workloads.**

---

# Cloud Security Posture Management

Security posture describes the overall security condition of an organization's environment.

Defender for Cloud can assess configurations and identify opportunities to improve security.

## Posture Management Capabilities

Examples include:

- Security recommendations
- Secure Score
- Regulatory compliance information
- Security configuration assessment

### Real-World Thinking

An administrator wants to know which Azure resources have security weaknesses or configurations that should be improved.

Defender for Cloud can provide recommendations and help prioritize security improvements.

### Exam Thinking

> **Posture Management = assess and improve security configuration.**

---

# Cloud Workload Protection

Defender for Cloud can provide enhanced protection for supported workloads.

Examples can include:

- Virtual machines
- Containers
- Databases
- Storage
- Other supported cloud workloads

### Real-World Thinking

Security posture management helps identify weaknesses.

Workload protection helps protect workloads against active threats.

### Easy Way to Remember

```text
CSPM = Improve SECURITY POSTURE
CWP  = Protect CLOUD WORKLOADS
```

---

# Security Recommendations

Microsoft Defender for Cloud can analyze resources and provide **security recommendations**.

Recommendations can help administrators identify actions that may improve security.

Examples might involve:

- Configuration improvements
- Missing protections
- Security best practices
- Identity or network security
- Workload protection

### Exam Thinking

> **Recommendations = actions Defender for Cloud suggests to improve security.**

---

# Secure Score

**Secure Score** provides a numerical measurement of security posture and helps identify recommended actions that can improve security.

A higher score generally indicates that more recommended security controls have been implemented.

```text
Assess Environment
       |
       v
Identify Recommendations
       |
       v
Improve Security Controls
       |
       v
Improve Secure Score
```

### Important

Secure Score is a **measurement and improvement tool**.

It does not mean an environment is completely secure simply because it has a high score.

### Real-World Thinking

An IT team wants a simple way to track whether its Azure security posture is improving.

Secure Score can provide a measurable indicator and related recommendations.

### Exam Thinking

> **Secure Score = measure and improve security posture.**

---

# Regulatory Compliance

Microsoft Defender for Cloud can provide a **Regulatory Compliance** view that helps organizations assess resources against supported security and compliance standards.

This can help administrators identify:

- Passed controls
- Failed controls
- Areas requiring attention

### Important Distinction

Defender for Cloud can help assess compliance posture, but using a Microsoft security service does not automatically make an organization compliant with every regulation.

### Exam Thinking

> **Regulatory Compliance = assess cloud resources against supported compliance standards.**

---

# Microsoft Defender Plans

Microsoft Defender for Cloud includes foundational security posture capabilities and can offer additional Defender plans for enhanced workload protection.

Depending on the plan and resource type, enhanced protection can apply to supported workloads such as:

- Servers
- Storage
- Databases
- Containers

> [!NOTE]
> Available Defender plans, features, trials, and pricing can change. For AZ-900, focus on the purpose of Defender for Cloud rather than memorizing current prices.

---

# Defense in Depth

**Defense in Depth** is a security strategy that uses multiple layers of security controls.

Instead of depending on one security measure, protection is placed at several levels.

If one security layer fails, additional layers can continue protecting the environment.

### Exam Thinking

> **Defense in Depth = multiple layers of security protection.**

---

# Defense in Depth Layers

A common way to visualize Defense in Depth is:

```text
        DATA
         |
    APPLICATION
         |
      COMPUTE
         |
      NETWORK
         |
     PERIMETER
         |
 IDENTITY & ACCESS
         |
 PHYSICAL SECURITY
```

Each layer protects a different part of the environment.

---

## 1. Physical Security

Protects physical datacenters, buildings, hardware, and infrastructure.

Examples:

- Controlled building access
- Security personnel
- Physical monitoring

---

## 2. Identity & Access

Protects identities and controls access.

Examples:

- Microsoft Entra ID
- MFA
- Azure RBAC
- Conditional Access

### Think

> **Who is requesting access, and what are they allowed to do?**

---

## 3. Perimeter

Protects the boundary between trusted resources and external networks.

Examples can include:

- Firewalls
- Filtering
- DDoS protections

### Think

> **Protect the network edge.**

---

## 4. Network

Protects communication between resources.

Examples can include:

- Network segmentation
- Network security controls
- Private connectivity

### Think

> **Control traffic between resources.**

---

## 5. Compute

Protects virtual machines, containers, and other workloads.

Examples can include:

- Patching
- Endpoint protection
- Workload security

---

## 6. Application

Protects software and application code.

Examples can include:

- Secure development practices
- Vulnerability management
- Application security controls

---

## 7. Data

Protects information wherever it is stored or transmitted.

Examples can include:

- Encryption
- Access controls
- Backup and recovery

### Exam Thinking

> **Data is commonly shown as the innermost layer because the other security layers ultimately help protect organizational information.**

---

# Why Defense in Depth Matters

Consider a workload protected by:

```text
Physical Datacenter Security
          +
Identity Protection
          +
Network Security
          +
VM Protection
          +
Application Security
          +
Data Encryption
```

An attacker defeating one control does not automatically defeat every other security layer.

### Memory Trick

> **Defense in Depth = MANY LAYERS.**

---

# Zero Trust

**Zero Trust** is a security model based on the idea:

> **Never trust, always verify.**

Zero Trust does not automatically trust a request simply because it comes from inside a corporate network.

Users, devices, applications, and requests should be appropriately verified and authorized.

---

# Zero Trust Principles

Zero Trust is commonly associated with three principles:

## Verify Explicitly

Make access decisions using available signals and information.

Examples can include:

- Identity
- Device
- Location
- Service
- Risk

## Use Least Privilege Access

Give identities only the access they need.

## Assume Breach

Design security with the assumption that a security incident could occur.

Limit the potential impact and prevent attackers from moving freely through the environment.

### Memory Trick

```text
VERIFY EXPLICITLY
        +
USE LEAST PRIVILEGE
        +
ASSUME BREACH
```

### Exam Thinking

> **Zero Trust = verify every request rather than trusting based on network location.**

---

# Zero Trust vs. Defense in Depth

These concepts complement each other but are not the same.

| Concept | Main Idea |
|---|---|
| **Defense in Depth** | Use multiple security layers |
| **Zero Trust** | Never automatically trust; continuously verify access |

### Easy Way to Remember

```text
Defense in Depth = HOW MANY LAYERS?
Zero Trust       = SHOULD WE TRUST THIS REQUEST?
```

---

# Defender for Cloud vs. Secure Score

These terms are related but not interchangeable.

## Microsoft Defender for Cloud

The broader cloud security service.

## Secure Score

A measurement within Microsoft's security ecosystem that helps represent security posture and prioritize improvements.

```text
Defender for Cloud
       |
       +-- Security posture
       +-- Recommendations
       +-- Secure Score
       +-- Regulatory Compliance
       +-- Workload protection
```

### Exam Thinking

> **Defender for Cloud = security platform. Secure Score = security posture measurement.**

---

# Choosing the Right Security Concept

### Think Microsoft Defender for Cloud when:
- You need cloud security posture management.
- You need security recommendations.
- You need workload protection for supported cloud resources.
- You want to review regulatory compliance information.

### Think Secure Score when:
- You need a numerical security-posture measurement.
- You want to track security improvement.

### Think Defense in Depth when:
- The scenario mentions multiple layers of security.
- One security control should not be the only protection.

### Think Zero Trust when:
- The scenario says no user or device should be trusted automatically.
- Every access request should be verified.
- Least privilege and assume-breach principles are involved.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 18 Lab — Security I](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-18-Lab-18-Security-I.md)**

### Lab Focus

- Browse Microsoft Defender for Cloud.
- Review Secure Score.
- Explore Security Recommendations.
- Review Regulatory Compliance.
- Browse Microsoft Defender plans.
- Map Defense in Depth layers.
- Practice Zero Trust scenarios.
- Compare Defender for Cloud, Secure Score, Defense in Depth, and Zero Trust.

> [!TIP]
> The lab is primarily exploration. You do not need to purchase or enable additional Defender plans to complete it.

---

# Quick Check

| Need | Concept |
|---|---|
| Cloud security posture and workload protection | Microsoft Defender for Cloud |
| Numerical security posture measurement | Secure Score |
| Multiple layers of security | Defense in Depth |
| Never trust, always verify | Zero Trust |
| Suggested security improvements | Security Recommendations |
| Assess resources against supported standards | Regulatory Compliance |

---

# Before Moving On

You should be able to:

- Explain Microsoft Defender for Cloud.
- Explain cloud security posture management.
- Explain the purpose of Secure Score.
- Explain Security Recommendations.
- Explain Defense in Depth.
- Identify the major Defense in Depth layers.
- Explain Zero Trust.
- Recognize Verify Explicitly, Least Privilege, and Assume Breach.
- Compare Defense in Depth and Zero Trust.
- Know how Defender for Cloud helps secure Azure resources.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Defender for Cloud** | Cloud security posture and workload protection |
| **CSPM** | Assess and improve security posture |
| **Workload Protection** | Protect cloud workloads |
| **Secure Score** | Measure security posture |
| **Security Recommendations** | Suggested security improvements |
| **Defense in Depth** | Multiple security layers |
| **Zero Trust** | Never trust, always verify |
| **Verify Explicitly** | Evaluate each access request |
| **Least Privilege** | Minimum necessary access |
| **Assume Breach** | Design as though compromise can occur |
