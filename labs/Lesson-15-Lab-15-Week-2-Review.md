[Lesson-15-Lab-15-Week-2-Review.md](https://github.com/user-attachments/files/31149240/Lesson-15-Lab-15-Week-2-Review.md)
# Lab 15 — Week 2 Review

## Objective

This optional lab reviews the hands-on concepts from **Lessons 8–14**.

There are no new Azure services introduced in this lab.

By the end, you should be able to:

- Navigate the Azure resource hierarchy.
- Recognize major Azure compute services.
- Identify Azure Storage services.
- Identify Azure networking services.
- Explore Azure Monitor and Advisor.
- Navigate Microsoft Entra ID.
- Review Azure RBAC.
- Choose the correct Azure service for mixed AZ-900 scenarios.

---

# Prerequisites

- Completed Lessons 8–14
- Web browser
- Azure account with appropriate access

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **AZ-900 Study Guide:** https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900
- **Microsoft Practice Assessment:** https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/practice/assessment?assessment-type=practice&assessmentId=23

> [!IMPORTANT]
> This is a review lab. You do not need to deploy every service. Use existing test resources or configuration screens whenever possible, and do not modify production resources, permissions, or identity settings.

---

# Part 1 — Review the Azure Resource Hierarchy

### Links

- **Azure Resource Manager Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview
- **Management Groups:** https://learn.microsoft.com/en-us/azure/governance/management-groups/overview
- **Azure Portal:** https://portal.azure.com/

Complete the hierarchy:

```text
[ __________________ ]
          |
          v
[ __________________ ]
          |
          v
[ __________________ ]
          |
          v
[ __________________ ]
```

Choose from:

- Resource
- Resource Group
- Subscription
- Management Group

## Think About It

Which level can organize multiple subscriptions?

**Answer:** _______________________________________________

Which level is a logical container for related Azure resources?

**Answer:** _______________________________________________

Which level represents the actual Azure service?

**Answer:** _______________________________________________

---

# Part 2 — Explore a Resource Group

### Links

- **Manage Resource Groups:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open the Azure Portal.
2. Search for **Resource groups**.
3. Open an existing safe test Resource Group if available.
4. Review the resources contained inside it.
5. Look at the Resource Group's:
   - Subscription
   - Location
   - Resources
   - Access control (IAM)
   - Activity Log
6. Do not delete or modify production resources.

### Optional

If you have a dedicated lab subscription, create a temporary Resource Group and delete it after the lab.

## Think About It

Can a Resource Group contain different types of Azure resources?

**Answer:** _______________________________________________

---

# Part 3 — Review Azure Compute

### Links

- **Azure Virtual Machines:** https://learn.microsoft.com/en-us/azure/virtual-machines/overview
- **Virtual Machine Scale Sets:** https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview
- **Azure App Service:** https://learn.microsoft.com/en-us/azure/app-service/overview
- **Azure Functions:** https://learn.microsoft.com/en-us/azure/azure-functions/functions-overview
- **Azure Container Instances:** https://learn.microsoft.com/en-us/azure/container-instances/container-instances-overview
- **Azure Kubernetes Service:** https://learn.microsoft.com/en-us/azure/aks/what-is-aks

## Steps

Use the Azure Portal search to locate each service without deploying it:

1. Virtual Machines
2. Virtual Machine Scale Sets
3. App Services
4. Function App
5. Container Instances
6. Kubernetes services

Complete the table:

| Need | Azure Service |
|---|---|
| Individual virtual computer | __________________ |
| Scalable group of similar VMs | __________________ |
| Managed web application hosting | __________________ |
| Event-driven serverless code | __________________ |
| Quickly run a container | __________________ |
| Kubernetes container orchestration | __________________ |

---

# Part 4 — Review Azure Networking

### Links

- **Azure Virtual Network:** https://learn.microsoft.com/en-us/azure/virtual-network/virtual-networks-overview
- **Private Endpoint:** https://learn.microsoft.com/en-us/azure/private-link/private-endpoint-overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Search the Azure Portal for **Virtual networks**.
2. Open a safe VNet if one is available.
3. Review its:
   - Address space
   - Subnets
   - Connected devices or resources if available
4. Review Microsoft's Private Endpoint documentation.
5. Do not modify production networking.

## Think About It

What is the purpose of a VNet?

**Answer:** _______________________________________________

What is the key difference between a public endpoint and a private endpoint?

**Answer:** _______________________________________________

---

# Part 5 — Review Azure Storage

### Links

- **Storage Account Overview:** https://learn.microsoft.com/en-us/azure/storage/common/storage-account-overview
- **Blob Storage:** https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction
- **Azure Files:** https://learn.microsoft.com/en-us/azure/storage/files/storage-files-introduction
- **Queue Storage:** https://learn.microsoft.com/en-us/azure/storage/queues/storage-queues-introduction
- **Table Storage:** https://learn.microsoft.com/en-us/azure/storage/tables/table-storage-overview

## Steps

If a safe Storage Account is available:

1. Open the Storage Account.
2. Locate:
   - Containers
   - File shares
   - Queues
   - Tables
3. Review each area without uploading company or sensitive data.

Complete the table:

| Data Need | Storage Service |
|---|---|
| Images and video | __________________ |
| Shared folders | __________________ |
| Application messages | __________________ |
| Structured NoSQL data | __________________ |

---

# Part 6 — SQL Database vs. Cosmos DB

### Links

- **Azure SQL Database:** https://learn.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview
- **Azure Cosmos DB:** https://learn.microsoft.com/en-us/azure/cosmos-db/introduction

Choose the best service.

### Scenario 1

An application requires a managed relational database.

**Answer:** _______________________________

### Scenario 2

A worldwide application requires a globally distributed NoSQL database.

**Answer:** _______________________________

---

# Part 7 — Monitor vs. Advisor vs. Service Health

### Links

- **Azure Monitor:** https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/overview
- **Azure Advisor:** https://learn.microsoft.com/en-us/azure/advisor/advisor-overview
- **Azure Service Health:** https://learn.microsoft.com/en-us/azure/service-health/overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Search for **Monitor** and review the service.
2. Search for **Advisor** and review available recommendations.
3. Search for **Service Health** and review available health information.
4. Do not modify production alerting or monitoring settings.

Choose the best tool:

### Scenario 1

You need to review a VM's CPU metrics.

**Answer:** _______________________________

### Scenario 2

You want recommendations for improving Azure cost or reliability.

**Answer:** _______________________________

### Scenario 3

You want to know whether Microsoft has an Azure service issue affecting your environment.

**Answer:** _______________________________

---

# Part 8 — Review Microsoft Entra ID

### Links

- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **What is Microsoft Entra ID?:** https://learn.microsoft.com/en-us/entra/fundamentals/whatis

## Steps

1. Open the Microsoft Entra admin center.
2. Review Microsoft Entra ID.
3. Locate areas such as:
   - Users
   - Groups
   - Enterprise applications
   - Authentication methods
4. Do not modify production identities or settings.

## Think About It

What is Microsoft Entra ID's primary purpose?

**Answer:** _______________________________________________

---

# Part 9 — Review Azure RBAC

### Links

- **Azure RBAC Overview:** https://learn.microsoft.com/en-us/azure/role-based-access-control/overview
- **Azure Built-In Roles:** https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles

Complete the RBAC model:

```text
WHO   = ______________________________
WHAT  = ______________________________
WHERE = ______________________________
```

Choose from:

- Security Principal
- Role Definition
- Scope

## Role Review

| Need | Role |
|---|---|
| View resources only | __________________ |
| Manage resources but not assign Azure roles | __________________ |
| Manage resources and assign Azure roles | __________________ |

---

# Part 10 — Identity Review

Choose from:

- Authentication
- Authorization
- Conditional Access
- MFA
- SSO

### Scenario 1

A user proves their identity.

**Answer:** _______________________________

### Scenario 2

Azure determines what an authenticated user is allowed to do.

**Answer:** _______________________________

### Scenario 3

An if-then policy requires additional controls under configured conditions.

**Answer:** _______________________________

### Scenario 4

A user provides two or more authentication factors.

**Answer:** _______________________________

### Scenario 5

A user authenticates once and accesses multiple authorized applications.

**Answer:** _______________________________

---

# Part 11 — Mixed Week 2 Scenarios

Choose the best Azure concept or service.

### Scenario 1

A company wants protection against a datacenter-level failure inside one Azure region.

**Answer:** _______________________________

### Scenario 2

A web application should run without the organization managing the underlying web servers.

**Answer:** _______________________________

### Scenario 3

Code should execute when a specific event occurs.

**Answer:** _______________________________

### Scenario 4

A company needs to run a container quickly without managing Kubernetes.

**Answer:** _______________________________

### Scenario 5

A large containerized application needs orchestration and scaling.

**Answer:** _______________________________

### Scenario 6

An application needs to store messages for asynchronous processing.

**Answer:** _______________________________

### Scenario 7

An administrator wants Azure to recommend ways to improve existing resources.

**Answer:** _______________________________

### Scenario 8

An administrator wants to know whether an Azure platform outage is affecting the subscription.

**Answer:** _______________________________

### Scenario 9

A user should only be able to view Azure resources.

**Answer:** _______________________________

### Scenario 10

Administrators should be required to complete MFA under configured access conditions.

**Answer:** _______________________________

---

# Part 12 — Microsoft Practice Assessment

### Links

- **AZ-900 Study Guide:** https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900
- **AZ-900 Practice Assessment:** https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/practice/assessment?assessment-type=practice&assessmentId=23

## Steps

1. Review the current Microsoft AZ-900 Study Guide.
2. Complete the Microsoft Practice Assessment.
3. Record the topics you missed.
4. Return to the corresponding lesson and lab.
5. Retake practice questions after reviewing weak areas.

### Weak Areas

1. _______________________________________________
2. _______________________________________________
3. _______________________________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

```text
Management Group
      |
Subscription
      |
Resource Group
      |
Resource
```

## Part 3

| Need | Answer |
|---|---|
| Individual virtual computer | Virtual Machine |
| Scalable group of similar VMs | Virtual Machine Scale Set |
| Managed web application hosting | Azure App Service |
| Event-driven serverless code | Azure Functions |
| Quickly run a container | Azure Container Instances |
| Kubernetes orchestration | Azure Kubernetes Service |

## Part 4

A VNet provides private networking for Azure resources. A public endpoint uses a public network path, while a private endpoint provides private connectivity using a private IP in a VNet.

## Part 5

| Need | Answer |
|---|---|
| Images and video | Blob Storage |
| Shared folders | Azure Files |
| Application messages | Queue Storage |
| Structured NoSQL data | Table Storage |

## Part 6

1. Azure SQL Database
2. Azure Cosmos DB

## Part 7

1. Azure Monitor
2. Azure Advisor
3. Azure Service Health

## Part 8

Microsoft Entra ID provides cloud identity and access management.

## Part 9

```text
WHO   = Security Principal
WHAT  = Role Definition
WHERE = Scope
```

| Need | Role |
|---|---|
| View only | Reader |
| Manage resources, not role assignments | Contributor |
| Manage resources and role assignments | Owner |

## Part 10

1. Authentication
2. Authorization
3. Conditional Access
4. MFA
5. SSO

## Part 11

1. Availability Zones
2. Azure App Service
3. Azure Functions
4. Azure Container Instances
5. Azure Kubernetes Service
6. Queue Storage
7. Azure Advisor
8. Azure Service Health
9. Reader
10. Conditional Access

</details>

---

# Lab Complete

You have completed the **Week 2 Review**.

Before moving on, make sure you can:

- Explain the Azure resource hierarchy.
- Compare Azure architecture concepts.
- Compare major Azure compute services.
- Identify the major Azure Storage services.
- Explain Azure networking fundamentals.
- Compare Azure Monitor, Advisor, and Service Health.
- Explain Microsoft Entra ID and Azure RBAC.
- Compare Authentication and Authorization.
- Explain Conditional Access, MFA, and SSO.
- Choose the correct Azure service for common business scenarios.
