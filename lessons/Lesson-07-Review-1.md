[Lesson-07-Week-1-Review.md](https://github.com/user-attachments/files/31148621/Lesson-07-Week-1-Review.md)

# Lesson 7 — Review 1

## 📚 Review 1

Lesson 7 introduces **no new key terms**. The goal is to review and connect the concepts from **Lessons 1–6**.

### Focus
- CapEx vs. OpEx and consumption-based pricing
- Public, Private, Hybrid, and Multi-Cloud
- High Availability, Scalability, Reliability, and Predictability
- IaaS, PaaS, and SaaS
- Regions, Region Pairs, and Availability Zones
- Azure Resource Hierarchy
- Azure Resource Manager (ARM)
- Azure Arc

---

# 1. CapEx vs. OpEx

## Capital Expenditure (CapEx)
**CapEx** is money spent upfront to purchase physical infrastructure or other long-term assets.

Examples include servers, networking equipment, and datacenter equipment.

### Real-World Thinking
Buying physical servers for an on-premises datacenter requires a significant upfront investment.

### Exam Thinking
> **CapEx = upfront spending on physical infrastructure.**

## Operational Expenditure (OpEx)
**OpEx** is ongoing spending for services or products as they are consumed.

### Real-World Thinking
Instead of purchasing a server, an organization can consume Azure resources and pay based on usage.

### Exam Thinking
> **OpEx = ongoing spending based on consumption or usage.**

---

# 2. Consumption-Based Pricing

Cloud computing commonly uses a **consumption-based model**. You pay for resources and services as you use them rather than purchasing all infrastructure upfront.

### Exam Thinking
> **Consumption-based pricing = pay for what you use.**

---

# 3. Cloud Deployment Models

| Model | Description |
|---|---|
| **Public Cloud** | Cloud resources provided by a third-party cloud provider |
| **Private Cloud** | Cloud environment dedicated to one organization |
| **Hybrid Cloud** | Combines public and private cloud environments |
| **Multi-Cloud** | Uses services from multiple cloud providers |

### Easy Way to Remember

```text
Public  = Provider's cloud
Private = Organization's dedicated cloud
Hybrid  = Public + Private
Multi   = Multiple cloud providers
```

---

# 4. Cloud Benefits

| Benefit | Remember |
|---|---|
| **High Availability** | Keep services available despite disruptions |
| **Scalability** | Adjust resources to meet demand |
| **Reliability** | Recover from failures and continue operating |
| **Predictability** | Anticipate performance and costs |

---

# 5. IaaS vs. PaaS vs. SaaS

| Model | Main Idea | Example |
|---|---|---|
| **IaaS** | Customer manages more of the environment | Azure Virtual Machines |
| **PaaS** | Provider manages the platform | Azure App Service / Azure SQL Database |
| **SaaS** | Customer uses finished software | Microsoft 365 |

**Azure Functions** is a serverless compute service commonly described as Function as a Service (FaaS).

### Easy Way to Remember

```text
IaaS = Manage the MOST
PaaS = Manage the APPLICATION
SaaS = USE the SOFTWARE
```

### Exam Thinking
> **Azure VM = IaaS**  
> **Azure App Service = PaaS**  
> **Azure SQL Database = PaaS**  
> **Azure Functions = Serverless / FaaS**  
> **Microsoft 365 = SaaS**

---

# 6. Regions, Region Pairs, and Availability Zones

| Concept | Remember |
|---|---|
| **Azure Region** | Geographic area containing Azure datacenters |
| **Region Pair** | Region-to-region resiliency and disaster-recovery planning |
| **Availability Zone** | Physically separate location inside an Azure region |

```text
Region            = Geographic area
Region Pair       = Region <--> Region
Availability Zone = Separate location inside a region
```

---

# 7. Azure Resource Hierarchy

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

| Level | Purpose |
|---|---|
| **Management Group** | Organizes and governs subscriptions |
| **Subscription** | Billing and management boundary |
| **Resource Group** | Logical container for related resources |
| **Resource** | Individual Azure service or asset |

### Exam Thinking
> **Management Group → Subscription → Resource Group → Resource**

---

# 8. Azure Resource Manager vs. Azure Arc

## Azure Resource Manager (ARM)
Azure Resource Manager is Azure's management and deployment layer for Azure resources.

## Azure Arc
Azure Arc extends Azure management and governance capabilities to supported resources outside Azure.

### Easy Way to Remember

```text
ARM       = Manage Azure resources
Azure Arc = Extend Azure management beyond Azure
```

---

# 🧪 Hands-On Review

Lesson 7 is a **review lesson**, so a separate Lab 07 is not necessary.

Instead, revisit the hands-on work from the earlier lessons.

### Recommended Review Activities
- Create or inspect a Resource Group.
- Browse Azure Regions and Availability Zones.
- Review the Azure Resource Hierarchy.
- Browse Azure Arc in the Azure Portal.
- Identify the service model for Azure Virtual Machines, Azure App Service, Azure Functions, and Azure SQL Database.

### Existing Labs to Revisit
- **[Lesson 02 Lab — Cloud Models and Azure Arc](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-02-Lab-02-Cloud-Models-and-Azure-Arc.md)**
- **[Lesson 03 Lab — Cloud Service Models](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-03-Lab-03-Cloud-Service-Models.md)**
- **[Lesson 04 Lab — Azure Architecture I](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-04-Lab-04-Azure-Architecture-I.md)**
- **[Lesson 05 Lab — Azure Architecture II](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-05-Lab-05-Azure-Architecture-II.md)**
- **[Lesson 06 Lab — Azure Architecture III](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-06-Lab-06-Azure-Architecture-III.md)**

> [!TIP]
> For a review lesson, repeating selected activities from the existing labs is more useful than creating another lab that duplicates the same work.

---

# 📝 Microsoft Exam Review

- **AZ-900 Study Guide:** https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900
- **Microsoft Certification Practice Assessments:** https://learn.microsoft.com/en-us/credentials/certifications/practice-assessments-for-microsoft-certifications

---

# Week 1 Quick Check

1. What is the difference between CapEx and OpEx?
2. What does consumption-based pricing mean?
3. What is the difference between Public, Private, Hybrid, and Multi-Cloud?
4. What is the difference between High Availability and Scalability?
5. What is the difference between Reliability and Predictability?
6. What is the difference between IaaS, PaaS, and SaaS?
7. Is Azure Virtual Machines IaaS, PaaS, or SaaS?
8. Is Azure App Service IaaS, PaaS, or SaaS?
9. What service model is Azure Functions associated with?
10. Is Azure SQL Database IaaS or PaaS?
11. What is the difference between an Azure Region and an Availability Zone?
12. What is the purpose of a Region Pair?
13. Put these in order: Resource, Subscription, Management Group, Resource Group.
14. What does Azure Resource Manager do?
15. What is the purpose of Azure Arc?

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

1. **CapEx** is upfront capital spending; **OpEx** is ongoing operational spending.
2. Pay based on the resources or services consumed.
3. Public uses a provider's cloud; Private is dedicated to one organization; Hybrid combines public and private; Multi-Cloud uses multiple cloud providers.
4. High Availability focuses on keeping services available; Scalability adjusts capacity to demand.
5. Reliability focuses on recovering from failures; Predictability helps anticipate performance and cost.
6. IaaS provides infrastructure, PaaS provides a managed platform, and SaaS provides finished software.
7. **IaaS**
8. **PaaS**
9. **Serverless / FaaS**
10. **PaaS**
11. A Region is a geographic area; an Availability Zone is a physically separate location inside a region.
12. Regional resiliency and disaster-recovery planning.
13. **Management Group → Subscription → Resource Group → Resource**
14. ARM provides Azure's management and deployment layer.
15. Azure Arc extends Azure management to supported resources outside Azure.

</details>

---

# Before Moving On

You should be able to:
- Explain the cloud consumption model.
- Compare Public, Private, Hybrid, and Multi-Cloud.
- Compare CapEx and OpEx.
- Compare IaaS, PaaS, and SaaS.
- Explain Regions, Region Pairs, and Availability Zones.
- Explain the Azure Resource Hierarchy.
- Explain Azure Resource Manager.
- Explain the purpose of Azure Arc.
- Identify the major Week 1 concepts from short exam-style scenarios.

---

# Week 1 Exam Thinking Summary

```text
CapEx             = Upfront purchase
OpEx              = Ongoing expense
Consumption       = Pay for what you use
Hybrid Cloud      = Public + Private
IaaS              = Most customer management
PaaS              = Managed platform
SaaS              = Finished software
Region            = Geographic area
Availability Zone = Separate location within a region
Region Pair       = Region-to-region resiliency
Resource Group    = Logical resource container
Subscription      = Billing/management boundary
Management Group  = Governance across subscriptions
ARM               = Azure management layer
Azure Arc         = Azure management beyond Azure
```
