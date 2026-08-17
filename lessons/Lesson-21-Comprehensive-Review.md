# Lesson 21 — Comprehensive Review

## 📚 Final AZ-900 Review

This is the final lesson in the AZ-900 course.

There are **no new Azure services or concepts** in Lesson 21.

The goal is to bring together everything from the previous lessons, identify weak areas, and prepare for the Microsoft Azure Fundamentals (AZ-900) certification exam.

---

## 🎥 Recommended Review Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Overview of Microsoft Entra | 11:34 | https://youtu.be/bSIF_GjaCmo |
| Functionality and Usage of RBAC | 9:19 | https://youtu.be/0iVyJBG06fM |
| Functionality and Usage of Azure Policy | 10:50 | https://youtu.be/z7WMqHE3R8g |
| Functionality of Microsoft Defender for Cloud | 9:47 | https://youtu.be/eWcoMi_nQt4 |
| Purpose of Service Level Agreements (SLAs) | 13:42 | https://youtu.be/3QIVbgnNrR0 |
| Benefits and Usage of Regions and Region Pairs | 13:08 | https://youtu.be/4RjPOAN54AE |
| Benefits and Usage of Storage Account Resources | 18:04 | https://youtu.be/b8BrfsxLSx8 |

> [!TIP]
> You do not need to rewatch every video. Focus on topics where your practice results show that you need reinforcement.

---

# Final Review Map

Your final review should cover the major areas studied throughout the course.

```text
AZ-900
   |
   +-- Cloud Concepts
   |
   +-- Azure Architecture & Services
   |
   +-- Management & Governance
   |
   +-- Identity & Security
   |
   +-- Monitoring
   |
   +-- Pricing & Support
```

---

# 1. Cloud Computing

You should be able to explain cloud computing in simple terms and recognize its major benefits.

Review concepts such as:

- High availability
- Scalability
- Elasticity
- Reliability
- Predictability
- Security and governance
- Manageability

### Exam Thinking

> **Cloud computing = delivery of computing services over the internet using on-demand resources.**

---

# 2. Cloud Models

Be able to compare:

- Public Cloud
- Private Cloud
- Hybrid Cloud
- Multi-Cloud

### Quick Review

| Model | Remember |
|---|---|
| **Public Cloud** | Cloud provider infrastructure shared across customers |
| **Private Cloud** | Cloud environment dedicated to one organization |
| **Hybrid Cloud** | Public cloud + private/on-premises environment |
| **Multi-Cloud** | Uses services from multiple cloud providers |

### Memory Trick

```text
Public  = PROVIDER CLOUD
Private = ORGANIZATION CLOUD
Hybrid  = MIX
Multi   = MULTIPLE PROVIDERS
```

---

# 3. Cloud Service Models

Be able to compare:

- IaaS
- PaaS
- SaaS
- Serverless

### Quick Review

| Model | Think |
|---|---|
| **IaaS** | Most customer infrastructure control |
| **PaaS** | Build/deploy apps without managing underlying infrastructure |
| **SaaS** | Use a finished application |
| **Serverless** | Run code based on demand/events without managing servers |

### Memory Trick

```text
IaaS = MANAGE MORE
PaaS = MANAGE LESS
SaaS = USE THE APP
```

---

# 4. Azure Architecture

Be able to explain:

- Azure Regions
- Region Pairs
- Availability Zones

### Quick Review

```text
Region Pair
REGION <----------> REGION

Availability Zones
       ONE REGION
           |
     +-----+-----+
     |     |     |
   Zone1 Zone2 Zone3
```

### Remember

- **Region** = geographic area containing Azure datacenters.
- **Region Pair** = region-to-region resiliency planning.
- **Availability Zone** = physically separate location inside a region.

---

# 5. Azure Resource Hierarchy

Know the hierarchy:

```text
Management Group
       |
       v
Subscription
       |
       v
Resource Group
       |
       v
Resource
```

### Remember

| Level | Purpose |
|---|---|
| **Management Group** | Organize subscriptions |
| **Subscription** | Management and billing boundary |
| **Resource Group** | Logical container for resources |
| **Resource** | Individual Azure service |

---

# 6. Azure Resource Manager vs. Azure Arc

## Azure Resource Manager

Azure's deployment and management layer for Azure resources.

## Azure Arc

Extends Azure management and governance capabilities to supported resources outside Azure.

### Memory Trick

```text
ARM = MANAGE AZURE
Arc = EXTEND AZURE MANAGEMENT
```

---

# 7. Compute Services

Be able to recognize the major compute choices.

| Need | Azure Service |
|---|---|
| Virtual computer | Virtual Machine |
| Scalable group of VMs | Virtual Machine Scale Sets |
| Managed web app hosting | Azure App Service |
| Event-driven serverless code | Azure Functions |
| Simple container execution | Azure Container Instances |
| Container orchestration | Azure Kubernetes Service |

### High-Value Comparison

```text
VM   = VIRTUAL COMPUTER
VMSS = SCALE VMs

ACI  = RUN CONTAINERS
AKS  = ORCHESTRATE CONTAINERS
```

---

# 8. Azure Networking

Review:

- Virtual Networks
- Subnets
- Public and private connectivity
- Network Security Groups
- Azure Firewall
- Azure DDoS Protection

### Quick Review

| Need | Service / Concept |
|---|---|
| Private Azure network | Virtual Network |
| Divide a VNet | Subnet |
| Allow/deny network traffic | NSG |
| Central managed firewall | Azure Firewall |
| DDoS attack protection | Azure DDoS Protection |

---

# 9. Azure Storage and Databases

Know the major Azure Storage services.

| Service | Best Fit |
|---|---|
| **Blob Storage** | Objects and unstructured data |
| **Azure Files** | Managed file shares |
| **Queue Storage** | Application messages |
| **Table Storage** | NoSQL key/attribute data |

Also remember:

```text
Azure SQL Database = RELATIONAL
Azure Cosmos DB    = NoSQL / globally distributed
```

---

# 10. Identity and Access

Review:

- Microsoft Entra ID
- Authentication
- Authorization
- Azure RBAC
- MFA
- Conditional Access
- SSO

### Quick Review

```text
Authentication = WHO ARE YOU?
Authorization  = WHAT CAN YOU DO?

Entra ID = IDENTITY
RBAC     = RESOURCE PERMISSIONS

MFA                = MULTIPLE FACTORS
Conditional Access = IF / THEN ACCESS POLICY
SSO                = SIGN IN ONCE
```

---

# 11. Governance

Review:

- Azure Policy
- Resource Locks
- Tags

### Memory Trick

```text
Policy = ENFORCE
Locks  = PROTECT
Tags   = ORGANIZE
RBAC   = PERMISSIONS
```

### Important Comparison

```text
RBAC   = WHO CAN DO IT?
Policy = WHAT IS ALLOWED?
```

---

# 12. Security

Review:

- Microsoft Defender for Cloud
- Secure Score
- Defense in Depth
- Zero Trust
- Azure Key Vault
- Microsoft Sentinel

### Quick Review

| Concept | Remember |
|---|---|
| **Defender for Cloud** | Security posture + workload protection |
| **Secure Score** | Measure security posture |
| **Defense in Depth** | Multiple security layers |
| **Zero Trust** | Never trust, always verify |
| **Key Vault** | Secrets, keys, certificates |
| **Sentinel** | SIEM / security operations |

### Zero Trust Principles

```text
VERIFY EXPLICITLY
        +
USE LEAST PRIVILEGE
        +
ASSUME BREACH
```

---

# 13. Monitoring and Optimization

Know the difference between:

- Azure Monitor
- Azure Advisor
- Azure Service Health

### Memory Trick

```text
Monitor        = WHAT IS HAPPENING?
Advisor        = WHAT SHOULD I IMPROVE?
Service Health = IS AZURE HAVING A PROBLEM?
```

---

# 14. Pricing and Cost Management

Review:

- Azure Pricing Calculator
- TCO Calculator
- Azure Cost Management
- Reservations
- Spot VMs

### Quick Review

```text
Pricing Calculator = ESTIMATE AZURE COST
TCO Calculator     = ON-PREM vs. AZURE
Cost Management    = MONITOR SPENDING
Reservation        = COMMITMENT DISCOUNT
Spot VM            = DISCOUNTED + INTERRUPTIBLE
```

---

# 15. Service Level Agreements

An **SLA** describes Microsoft's availability commitments for Azure services.

Remember:

- Higher SLA percentage = less allowable downtime.
- Service credits may apply according to SLA terms.
- Multiple dependent services can produce a lower composite SLA.

### Example

```text
99.9% × 99.9% = 99.8001%
```

### Exam Thinking

> **SLA = availability commitment.**

---

# 16. Azure Marketplace and Service Lifecycle

## Azure Marketplace

Find Microsoft and third-party solutions for Azure.

> **Marketplace = SHOP.**

## Service Lifecycle

```text
Private Preview
      |
Public Preview
      |
Generally Available (GA)
      |
Possible Retirement
```

### Remember

```text
Preview = TEST / EVALUATE
GA      = GENERAL RELEASE
Retired = MIGRATE AWAY
```

---

# High-Value AZ-900 Comparisons

Spend extra review time on concepts that sound similar.

| Don't Confuse | Key Difference |
|---|---|
| Public vs. Private Cloud | Provider cloud vs. dedicated organizational cloud |
| Hybrid vs. Multi-Cloud | Mix of environments vs. multiple cloud providers |
| IaaS vs. PaaS vs. SaaS | Customer management responsibility |
| Region Pair vs. Availability Zone | Cross-region vs. inside one region |
| Resource Group vs. Subscription | Resource container vs. management/billing boundary |
| ARM vs. Azure Arc | Azure management vs. management beyond Azure |
| VM vs. VM Scale Set | Individual VM vs. scalable group |
| ACI vs. AKS | Run containers vs. orchestrate containers |
| Blob vs. Files | Object storage vs. file shares |
| SQL vs. Cosmos DB | Relational vs. NoSQL |
| Authentication vs. Authorization | Identity vs. permissions |
| Entra ID vs. RBAC | Identity vs. Azure resource permissions |
| RBAC vs. Azure Policy | Who can do it vs. what is allowed |
| Conditional Access vs. MFA | Access policy vs. authentication factor |
| Monitor vs. Advisor | Observe vs. recommend |
| Monitor vs. Service Health | Resource telemetry vs. Azure platform issues |
| Defense in Depth vs. Zero Trust | Security layers vs. verification model |
| NSG vs. Azure Firewall | Traffic rules vs. centralized firewall |
| Key Vault vs. Sentinel | Protect sensitive items vs. security monitoring |
| Pricing Calculator vs. TCO | Azure estimate vs. on-prem comparison |
| Reservation vs. Spot VM | Commitment vs. interruptible capacity |
| Preview vs. GA | Evaluation vs. general release |

---

# 🧪 Final Review Lab

Complete the final companion review:

**[Lesson 21 Lab — Final AZ-900 Review](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-21-Lab-21-Final-AZ-900-Review.md)**

### Lab Focus

- Complete a final knowledge check.
- Work through mixed AZ-900 scenarios.
- Take Microsoft's Practice Assessment.
- Record weak areas.
- Map missed questions back to your lessons and labs.
- Create a final study plan.
- Prepare for exam day.

> [!TIP]
> This is not a deployment lab. The goal is to prove that you can identify the correct Azure concept or service without relying on your notes.

---

# Final Knowledge Check

You should be able to explain, without looking at your notes:

- Cloud Computing.
- Public, Private, Hybrid, and Multi-Cloud.
- IaaS, PaaS, SaaS, and Serverless.
- Regions, Region Pairs, and Availability Zones.
- Resource Groups, Subscriptions, and Management Groups.
- Azure Resource Manager and Azure Arc.
- Major Azure compute services.
- Major Azure storage services.
- Azure networking fundamentals.
- Microsoft Entra ID and Azure RBAC.
- Azure Policy.
- Microsoft Defender for Cloud.
- Azure Monitor, Advisor, and Service Health.
- Pricing Calculator and TCO Calculator.
- Service Level Agreements.
- The correct Azure service for common business scenarios.

---

# Recommended Final Resources

## Microsoft AZ-900 Study Guide

https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900

## Microsoft AZ-900 Certification Page

https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/

## Microsoft Practice Assessment

Use the **Practice Assessment** available from the AZ-900 certification page.

## Microsoft Learn

https://learn.microsoft.com/training/

## John Savill's Technical Training

https://www.youtube.com/@NTFAQGuy

---

# Final Goal

You are ready to move toward the AZ-900 exam when you can:

- Explain the major concepts without relying heavily on notes.
- Distinguish commonly confused Azure services.
- Choose the correct service for basic business scenarios.
- Explain why an answer is correct rather than only memorizing the answer.
- Identify weak areas from practice results and review them.
- Complete full practice assessments confidently under exam-like conditions.

> [!IMPORTANT]
> Practice scores are useful for identifying readiness and weak areas, but there is no single practice-test percentage that guarantees a passing certification result.

---

# Exam Thinking Summary

```text
READ THE REQUIREMENT
        |
        v
IDENTIFY THE KEYWORD
        |
        v
ELIMINATE WRONG SERVICES
        |
        v
COMPARE THE FINAL OPTIONS
        |
        v
CHOOSE THE SERVICE THAT
BEST MATCHES THE REQUIREMENT
```

The goal is not to memorize every Azure setting.

The goal is to understand **what each major Azure service does, why you would use it, and how it differs from similar services.**
