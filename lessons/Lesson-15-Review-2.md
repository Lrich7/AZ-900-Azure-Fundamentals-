# Lesson 15 — Review 2

## 📚 Week 2 
**Lessons Covered:** Lessons 8–14

There are **no new terms** in Lesson 15.

The goal of this lesson is to review the major Azure concepts from Week 2, compare services that are easy to confuse, and practice choosing the correct Azure service for common AZ-900 scenarios.

---

# Week 2 Topics

Review the following major areas:

- Azure architecture and resource hierarchy
- Compute
- Networking
- Storage and databases
- Core Azure solutions
- Management and monitoring
- Identity and access

---

# 1. Azure Architecture

## Azure Regions

An **Azure Region** is a geographic area containing one or more Azure datacenters connected by a low-latency network.

### Remember

> **Region = geographic area containing Azure datacenters.**

---

# Availability Zones

**Availability Zones** are physically separate locations within an Azure region with independent infrastructure such as power, cooling, and networking.

```text
Azure Region
     |
     +-- Zone 1
     +-- Zone 2
     +-- Zone 3
```

### Remember

> **Availability Zone = physically separate location inside a region.**

---

# Region Pairs

Azure regions may be associated with another region in the same geography to support resiliency and disaster-recovery planning.

```text
Region A <------> Region B
```

### Remember

> **Region Pair = region-to-region resiliency.**

---

# Regions vs. Availability Zones vs. Region Pairs

| Concept | Scope | Think |
|---|---|---|
| **Region** | Geographic area | Datacenters |
| **Availability Zone** | Inside one region | Datacenter/location isolation |
| **Region Pair** | Two regions | Regional resiliency |

### Memory Trick

```text
Region Pair        = REGION <-> REGION
Availability Zones = ZONES inside ONE REGION
```

---

# 2. Azure Resource Hierarchy

Azure resources are organized into a hierarchy.

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

Used to organize and govern multiple subscriptions.

## Subscriptions

Provide a management, access, and billing boundary for Azure resources.

## Resource Groups

Logical containers used to organize related Azure resources.

## Resources

Individual Azure services such as virtual machines, storage accounts, and virtual networks.

### Exam Thinking

```text
Management Group = Organize subscriptions
Subscription     = Billing / management boundary
Resource Group   = Organize resources
Resource         = Actual Azure service
```

---

# 3. Azure Resource Manager vs. Azure Arc

## Azure Resource Manager (ARM)

**Azure Resource Manager** is Azure's deployment and management service.

It provides the management layer used to create, update, organize, and delete Azure resources.

### Remember

> **ARM = manage Azure resources.**

## Azure Arc

**Azure Arc** extends Azure management and governance capabilities to supported resources outside Azure.

This can include resources in:

- On-premises environments
- Other cloud environments
- Hybrid environments

### Remember

> **Azure Arc = extend Azure management beyond Azure.**

## ARM vs. Arc

```text
ARM = Manage Azure
Arc = Extend Azure management
      to hybrid / multicloud resources
```

---

# 4. Azure Compute

Major compute services covered during Week 2 include:

- Virtual Machines
- Virtual Machine Scale Sets
- Azure App Service
- Azure Functions
- Azure Container Instances
- Azure Kubernetes Service

---

# Virtual Machines vs. Virtual Machine Scale Sets

## Virtual Machines

Provide Infrastructure as a Service (IaaS) virtual computers.

You manage more of the operating system and software environment.

## Virtual Machine Scale Sets

Allow Azure to manage a group of similar VMs that can scale based on demand.

| Service | Best Fit |
|---|---|
| **Virtual Machine** | Individual VM / operating-system control |
| **VM Scale Set** | Multiple similar VMs that need scaling |

### Remember

```text
VM       = One or more virtual computers
VMSS     = Scalable group of similar VMs
```

---

# Azure App Service

**Azure App Service** is a managed platform for hosting web applications and APIs.

### Remember

> **App Service = host web apps without managing the underlying servers.**

---

# Azure Functions

**Azure Functions** provides serverless event-driven compute.

### Remember

> **Functions = run code when an event occurs.**

---

# Azure Container Instances vs. Azure Kubernetes Service

## Azure Container Instances (ACI)

Provides a fast way to run containers without managing virtual machines or a full orchestration platform.

## Azure Kubernetes Service (AKS)

Provides managed Kubernetes for orchestrating containerized applications.

| Service | Best Fit |
|---|---|
| **ACI** | Run containers simply |
| **AKS** | Orchestrate and manage many containers |

### Remember

```text
ACI = RUN containers
AKS = ORCHESTRATE containers
```

---

# 5. Azure Networking

## Virtual Networks

An **Azure Virtual Network (VNet)** provides private networking for Azure resources.

VNets can contain **subnets** that divide the network into smaller address ranges.

### Remember

> **VNet = private Azure network.**

---

# Public vs. Private Endpoints

## Public Endpoint

Allows access through a public IP address or public network path.

## Private Endpoint

Provides private connectivity to a supported Azure service through a private IP address in a VNet.

| Endpoint | Think |
|---|---|
| **Public** | Public network access |
| **Private** | Private VNet access |

### Remember

```text
Public Endpoint  = PUBLIC path
Private Endpoint = PRIVATE IP in VNet
```

---

# 6. Azure Storage

The four major Azure Storage services are:

- Blob Storage
- Azure Files
- Queue Storage
- Table Storage

| Storage Service | Best For |
|---|---|
| **Blob Storage** | Files, images, video, backups, unstructured objects |
| **Azure Files** | Managed shared file shares |
| **Queue Storage** | Application messages |
| **Table Storage** | Structured non-relational / NoSQL data |

### Memory Trick

```text
Blob  = OBJECTS
Files = SHARED FOLDERS
Queue = MESSAGES
Table = NoSQL DATA
```

---

# Azure SQL Database vs. Azure Cosmos DB

## Azure SQL Database

Managed relational database service based on SQL Server.

## Azure Cosmos DB

Managed NoSQL database service designed for scalable, globally distributed applications.

| Service | Think |
|---|---|
| **Azure SQL Database** | Relational |
| **Azure Cosmos DB** | Globally distributed NoSQL |

### Remember

```text
SQL    = RELATIONAL
Cosmos = GLOBAL NoSQL
```

---

# 7. Azure Management and Monitoring

Three services that are commonly confused are:

- Azure Monitor
- Azure Advisor
- Azure Service Health

## Azure Monitor

Collects and analyzes metrics, logs, and telemetry.

> **Monitor = What is happening?**

## Azure Advisor

Provides personalized recommendations for Azure resources.

> **Advisor = What should I improve?**

## Azure Service Health

Provides information about Azure service issues, planned maintenance, and advisories that may affect your environment.

> **Service Health = Is Azure having a problem?**

### Memory Trick

```text
Monitor        = OBSERVE
Advisor        = RECOMMEND
Service Health = AZURE SERVICE STATUS
```

---

# 8. Authentication vs. Authorization

## Authentication

Verifies identity.

> **Who are you?**

## Authorization

Determines permissions.

> **What can you do?**

### Remember

```text
Authentication = IDENTITY
Authorization  = PERMISSIONS
```

---

# 9. Microsoft Entra ID vs. Azure RBAC

## Microsoft Entra ID

Microsoft's cloud identity and access management service.

## Azure RBAC

Controls authorization to Azure resources through role assignments and scope.

| Concept | Think |
|---|---|
| **Microsoft Entra ID** | Identity |
| **Azure RBAC** | Azure resource permissions |

### Remember

```text
Entra ID = WHO you are
RBAC     = WHAT you can do to Azure resources
```

---

# 10. Conditional Access vs. MFA

## Conditional Access

Evaluates signals and applies configured access controls using condition-based policies.

## Multi-Factor Authentication

Requires two or more authentication factors.

| Feature | Think |
|---|---|
| **Conditional Access** | When/how access should be controlled |
| **MFA** | Additional identity verification |

### Remember

```text
Conditional Access = IF / THEN policy
MFA                = Multiple factors
```

Conditional Access can be configured to **require MFA**.

---

# 11. Single Sign-On

**Single Sign-On (SSO)** allows a user to authenticate and then access multiple authorized applications without repeatedly signing in.

### Remember

> **SSO = sign in once, access multiple authorized applications.**

---

# High-Value Week 2 Comparisons

| Don't Confuse | Key Difference |
|---|---|
| Region vs. Availability Zone | Geography vs. isolated location inside region |
| Region Pair vs. Availability Zone | Cross-region vs. inside one region |
| Resource Group vs. Subscription | Resource container vs. management/billing boundary |
| ARM vs. Azure Arc | Azure management vs. extending management beyond Azure |
| VM vs. VM Scale Set | Individual VM vs. scalable group |
| ACI vs. AKS | Run containers vs. orchestrate containers |
| Blob vs. Files | Object storage vs. file shares |
| SQL Database vs. Cosmos DB | Relational vs. NoSQL |
| Monitor vs. Advisor | Observe vs. recommend |
| Monitor vs. Service Health | Resource telemetry vs. Azure service issues |
| Authentication vs. Authorization | Identity vs. permissions |
| Entra ID vs. RBAC | Identity platform vs. Azure resource permissions |
| Conditional Access vs. MFA | Access policy vs. authentication factor requirement |

---

# 🧪 Hands-On Review Lab

Complete the optional companion review lab:

**[Lesson 15 Lab — Week 2 Review](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-15-Lab-15-Week-2-Review.md)**

### Lab Focus

- Review the Azure resource hierarchy.
- Explore a Resource Group.
- Browse Azure compute services.
- Browse Azure Storage services.
- Browse Azure Networking services.
- Explore Azure Monitor and Azure Advisor.
- Browse Microsoft Entra ID.
- Review Azure RBAC.
- Complete mixed Week 2 scenarios.

> [!TIP]
> This lab is optional. It is designed as a review of the hands-on skills from Lessons 8–14 rather than introducing new Azure services.

---

# Quick Check

| Scenario | Answer |
|---|---|
| Physically separate location inside a region | Availability Zone |
| Organizes multiple subscriptions | Management Group |
| Logical container for Azure resources | Resource Group |
| Scalable group of similar VMs | Virtual Machine Scale Set |
| Host a managed web application | Azure App Service |
| Run event-driven code | Azure Functions |
| Simple container execution | Azure Container Instances |
| Container orchestration | Azure Kubernetes Service |
| Private Azure network | Virtual Network |
| Store unstructured objects | Blob Storage |
| Managed shared file storage | Azure Files |
| Application messages | Queue Storage |
| Relational managed database | Azure SQL Database |
| Globally distributed NoSQL | Azure Cosmos DB |
| Metrics and logs | Azure Monitor |
| Azure recommendations | Azure Advisor |
| Azure outages and maintenance | Azure Service Health |
| Verify identity | Authentication |
| Determine permissions | Authorization |
| Azure resource permissions | Azure RBAC |
| Condition-based access rules | Conditional Access |
| Multiple authentication factors | MFA |
| One sign-in for multiple apps | SSO |

---

# Before Moving On

You should be able to:

- Explain the Azure resource hierarchy.
- Compare Regions, Availability Zones, and Region Pairs.
- Compare the major Azure compute services.
- Compare Azure Storage services.
- Explain Azure networking fundamentals.
- Compare Azure SQL Database and Azure Cosmos DB.
- Explain Azure Monitor, Advisor, and Service Health.
- Explain Authentication and Authorization.
- Explain Microsoft Entra ID and Azure RBAC.
- Explain Conditional Access, MFA, and SSO.
- Identify the correct Azure service for common business scenarios.

---

# Practice Resources

## Microsoft AZ-900 Study Guide

https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900

## Microsoft Practice Assessment

https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/practice/assessment?assessment-type=practice&assessmentId=23

> [!TIP]
> Use Microsoft's practice assessment to identify weak areas. Review the related lesson before attempting another practice assessment.
