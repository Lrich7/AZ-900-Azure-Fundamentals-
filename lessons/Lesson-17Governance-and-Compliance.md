[Lesson-17-Governance-and-Compliance.md](https://github.com/user-attachments/files/31148840/Lesson-17-Governance-and-Compliance.md)
# Lesson 17 — Governance & Compliance

## 📖 Microsoft Learn

**Documentation:** Azure Governance  
https://learn.microsoft.com/en-us/azure/governance/

### Focus
- Governance Hierarchy
- Azure Blueprints (Legacy)
- Cloud Adoption Framework
- Microsoft Purview
- Microsoft Trust Center
- Azure Compliance Documentation
- Azure Sovereign Regions
- Online Services Terms (OST)
- Data Protection Addendum (DPA)
- Microsoft Privacy Statement

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Governance Hierarchy Constructs | 6:13 | https://youtu.be/ge8r_Z0LKxM |
| Functionality and Usage of Azure Blueprints *(Legacy)* | 5:22 | https://youtu.be/SJbDcvkySCY |
| Describe Cloud Adoption Framework | 2:03 | https://youtu.be/VHQxbIynlN4 |
| Purpose of Microsoft Purview | 10:47 | https://youtu.be/mXjXcBr1ajY |
| Describe Microsoft Privacy Statement, OST and DPA | 3:28 | https://youtu.be/5mqroH3E3gw |
| Purpose of Trust Center and Azure Compliance Documentation | 5:42 | https://youtu.be/QkVlogulVX4 |
| Purpose of Azure Sovereign Regions | 5:15 | https://youtu.be/PdAEPAnT2uI |

---

# Governance and Compliance

Governance helps organizations control how cloud resources are organized and managed.

Compliance focuses on meeting legal, regulatory, industry, and organizational requirements.

Azure and Microsoft provide tools, frameworks, documentation, and specialized environments to help organizations manage these responsibilities.

```text
Governance & Compliance
        |
        +-- Governance hierarchy
        +-- Cloud Adoption Framework
        +-- Microsoft Purview
        +-- Trust Center
        +-- Compliance documentation
        +-- Legal / privacy documents
        +-- Sovereign cloud environments
```

---

# Governance Hierarchy

Azure governance can be applied through the Azure resource hierarchy:

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

## Management Groups

Help organize and govern multiple Azure subscriptions.

## Subscriptions

Provide management, access, and billing boundaries.

## Resource Groups

Logical containers for related Azure resources.

## Resources

The individual Azure services being managed.

### Exam Thinking

> **Governance applied higher in the hierarchy can affect resources beneath that scope.**

---

# Azure Blueprints — Legacy Concept

**Azure Blueprints** is a legacy Azure governance service that allowed organizations to define repeatable sets of governed Azure resources and configurations.

Blueprints could include artifacts such as:

- Azure Policy assignments
- Azure RBAC role assignments
- ARM templates
- Resource Groups

> [!IMPORTANT]
> Azure Blueprints is a **legacy concept**. Microsoft has announced retirement for **January 31, 2027**, and newer Azure governance and deployment approaches include **Template Specs** and **Deployment Stacks**.

For AZ-900, understand the **concept and historical purpose** rather than spending significant study time learning to deploy Blueprints.

---

# Blueprint Definitions

A **Blueprint Definition** described what should be deployed and governed.

It could contain multiple artifacts and versions.

### Exam Thinking

> **Blueprint Definition = reusable governance package.**

---

# Blueprint Artifacts

Artifacts were the individual components included inside a Blueprint.

Examples included:

- Policy assignments
- Role assignments
- ARM templates
- Resource Groups

```text
Blueprint
    |
    +-- Policy Assignment
    +-- RBAC Assignment
    +-- ARM Template
    +-- Resource Group
```

---

# Blueprint Assignments

A **Blueprint Assignment** applied a published Blueprint version to a target scope.

Blueprints also supported versioning and resource-locking capabilities.

### Exam Thinking

```text
Definition = WHAT the blueprint contains
Artifacts  = COMPONENTS inside it
Assignment = APPLY the blueprint
```

---

# Cloud Adoption Framework

The **Microsoft Cloud Adoption Framework for Azure** is a collection of guidance, best practices, documentation, and tools designed to help organizations plan and manage cloud adoption.

It helps connect business goals with technology decisions.

## Core Methodologies

### Strategy

Define business motivations, goals, and expected outcomes.

### Plan

Create the cloud adoption plan and prepare people, skills, and the digital estate.

### Ready

Prepare the Azure environment and landing zones.

### Adopt

Migrate, modernize, or build workloads.

### Govern

Establish governance controls, policies, and risk management.

### Secure

Protect cloud assets and environments.

### Manage

Operate and optimize workloads over time.

### Memory Flow

```text
Strategy
   |
   v
Plan
   |
   v
Ready
   |
   v
Adopt
   |
   v
Govern
   |
   v
Secure
   |
   v
Manage
```

### Real-World Thinking

A company knows it wants to move to Azure but needs guidance for planning the migration, preparing the environment, establishing governance, and operating workloads afterward.

The Cloud Adoption Framework provides structured guidance for that journey.

### Exam Thinking

> **Cloud Adoption Framework = guidance and best practices for adopting and managing Azure.**

---

# Microsoft Purview

**Microsoft Purview** provides data governance, security, and compliance capabilities for organizational data.

It can help organizations understand, discover, classify, and govern data across supported environments.

## Data Mapping and Scanning

Purview can scan supported data sources and collect metadata to help organizations understand their data estate.

## Data Catalog

A catalog can help users discover and understand available data assets.

## Data Lineage

Lineage helps show where data comes from and how it moves or changes.

## Data Classification

Purview can help identify and classify sensitive information.

### Real-World Thinking

A large organization has data spread across many systems and needs to understand:

- What data exists
- Where it is located
- Whether it contains sensitive information
- How data moves between systems

Microsoft Purview provides data-governance capabilities for this type of environment.

### Exam Thinking

> **Microsoft Purview = data governance, discovery, classification, and compliance.**

---

# Microsoft Trust Center

The **Microsoft Trust Center** provides information about Microsoft's security, privacy, and compliance practices.

It helps customers understand how Microsoft approaches protection and regulatory requirements across its cloud services.

## Major Areas

### Security

Information about Microsoft's security practices and protections.

### Privacy

Information about Microsoft's privacy practices and commitments.

### Compliance

Information about standards, regulations, and compliance programs.

### Related Resources

Microsoft also provides resources such as the **Service Trust Portal**, where eligible customers can access audit reports and compliance-related documentation.

### Exam Thinking

> **Microsoft Trust Center = information about Microsoft's security, privacy, and compliance practices.**

---

# Azure Compliance Documentation

**Azure Compliance Documentation** describes Azure compliance offerings, standards, regulatory requirements, and certifications.

Organizations can use this information to understand Azure's compliance capabilities and how they relate to their own regulatory responsibilities.

### Real-World Thinking

A company operating in a regulated industry needs to determine whether Azure supports a particular compliance standard.

Azure Compliance Documentation is a logical place to investigate.

### Exam Thinking

> **Azure Compliance Documentation = information about Azure compliance standards and certifications.**

---

# Azure Sovereign Regions and Clouds

Azure provides specialized cloud environments designed to address particular government, sovereignty, compliance, and data-residency requirements.

These environments can be physically and logically separated from the public Azure cloud.

### Real-World Thinking

A government organization may have regulatory requirements that cannot be satisfied by using the standard public cloud environment.

A specialized sovereign or government cloud may be appropriate.

### Exam Thinking

> **Sovereign Azure environments = specialized clouds for government, sovereignty, or regulatory requirements.**

---

# Microsoft Privacy Statement

The **Microsoft Privacy Statement** explains Microsoft's privacy practices, including how Microsoft collects, uses, and handles personal data across its products and services.

### Exam Thinking

> **Privacy Statement = Microsoft's general privacy practices.**

---

# Online Services Terms (OST)

The **Online Services Terms (OST)** is the term used in the original course material for Microsoft's legal terms governing online services.

It addresses areas such as:

- Service usage
- Customer rights
- Licensing
- Microsoft's responsibilities

### Exam Thinking

> **OST = legal terms for Microsoft's online services.**

---

# Data Protection Addendum (DPA)

The **Data Protection Addendum (DPA)** describes Microsoft's commitments and obligations regarding processing and protecting customer and personal data in its cloud services.

It supports organizations evaluating privacy and data-protection responsibilities.

### Exam Thinking

> **DPA = how Microsoft handles and protects customer data.**

---

# Compliance Documentation vs. Sovereign Regions vs. OST vs. DPA

These terms answer different questions.

| Question | Resource |
|---|---|
| Does Azure meet a compliance standard? | Azure Compliance Documentation |
| Is there a specialized cloud for regulatory or government requirements? | Azure Sovereign environment |
| What are the legal terms for using Microsoft's online services? | OST |
| How does Microsoft process and protect customer data? | DPA |

### Easy Way to Remember

```text
Compliance Documentation = PROOF / STANDARDS
Sovereign Environment    = SPECIAL LOCATION / CLOUD
OST                      = RULES / TERMS
DPA                      = DATA PROTECTION
```

---

# Trust Center vs. Compliance Documentation

These are related but have different emphasis.

## Microsoft Trust Center

Broad information about Microsoft's:

- Security
- Privacy
- Compliance

## Azure Compliance Documentation

More specifically helps customers understand Azure's compliance offerings, standards, and certifications.

### Memory Trick

```text
Trust Center              = TRUST INFORMATION
Compliance Documentation = COMPLIANCE DETAILS
```

---

# Cloud Adoption Framework vs. Azure Policy

Do not confuse adoption guidance with technical governance enforcement.

| Feature | Purpose |
|---|---|
| **Cloud Adoption Framework** | Guidance for planning and managing cloud adoption |
| **Azure Policy** | Enforce standards and assess Azure resource compliance |

### Exam Thinking

```text
CAF    = GUIDANCE
Policy = ENFORCEMENT
```

---

# Governance & Compliance Scenario Guide

### Think Cloud Adoption Framework when:
- An organization needs structured cloud-adoption guidance.
- The question involves strategy, planning, readiness, adoption, governance, security, or management.

### Think Microsoft Purview when:
- The question involves discovering or governing organizational data.
- Data cataloging, classification, or lineage is involved.

### Think Microsoft Trust Center when:
- The organization wants information about Microsoft's security, privacy, or compliance practices.

### Think Azure Compliance Documentation when:
- The organization needs information about Azure compliance standards or certifications.

### Think Sovereign Azure environments when:
- Government, sovereignty, specialized regulatory, or data-residency requirements are central to the scenario.

### Think DPA when:
- The question focuses on Microsoft's handling and protection of customer data.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 17 Lab — Governance & Compliance](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-17-Lab-17-Governance-and-Compliance.md)**

### Lab Focus

- Review the Azure governance hierarchy.
- Read the Cloud Adoption Framework overview.
- Browse Microsoft Purview.
- Browse the Microsoft Trust Center.
- Explore Azure Compliance Documentation.
- Review sovereign Azure environments.
- Compare compliance, privacy, and governance scenarios.

> [!TIP]
> This lab is primarily research and exploration. No Azure resources need to be deployed.

---

# Quick Check

| Need | Resource |
|---|---|
| Guidance for adopting Azure | Cloud Adoption Framework |
| Data governance and discovery | Microsoft Purview |
| Microsoft security, privacy, and compliance information | Microsoft Trust Center |
| Azure compliance standards and certifications | Azure Compliance Documentation |
| Specialized government/regulatory cloud | Sovereign Azure environment |
| Legal terms for online services | OST |
| Customer-data protection commitments | DPA |
| Legacy repeatable governance package | Azure Blueprints |

---

# Before Moving On

You should be able to:

- Explain the Azure governance hierarchy.
- Explain the purpose of the Cloud Adoption Framework.
- Recognize the major Cloud Adoption Framework methodologies.
- Explain the purpose of Microsoft Purview.
- Explain the Microsoft Trust Center.
- Explain Azure Compliance Documentation.
- Explain Azure Sovereign environments.
- Distinguish OST and DPA.
- Understand that Azure Blueprints is a legacy service and is no longer a primary AZ-900 focus.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Cloud Adoption Framework** | Cloud adoption guidance |
| **Microsoft Purview** | Data governance |
| **Trust Center** | Security, privacy, compliance information |
| **Compliance Documentation** | Standards and certifications |
| **Sovereign Azure** | Specialized government/regulatory cloud |
| **OST** | Online service terms |
| **DPA** | Customer-data protection |
| **Azure Blueprints** | Legacy governance concept |
