[Lesson-05-Azure-Architecture-II.md](https://github.com/user-attachments/files/31083342/Lesson-05-Azure-Architecture-II.md)

# Lesson 5 — Azure Architecture II

## 📖 Microsoft Learn

**Exercise:** Manage Azure Resource Groups  
https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups

### Focus
- Resources
- Resource Groups
- Subscriptions
- Management Groups
- Azure resource hierarchy

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Resource Groups | 9:38 | https://youtu.be/g6thrYZhPZY |
| Benefits and Usage of Subscriptions | 8:19 | https://youtu.be/9vKAYW_WkLo |
| Benefits and Usage of Management Groups | 6:30 | https://youtu.be/bPdDiEtCVhM |

---

# Azure Resource Hierarchy

Azure uses a hierarchy to organize and manage resources.

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
Resources
```

At a broader level, these resources exist within an Azure tenant.

```text
Tenant
  |
  +-- Management Group
        |
        +-- Subscription
              |
              +-- Resource Group
                    |
                    +-- Resources
```

---

# Azure Resources

A **Resource** is an individual cloud service or asset that you create and manage in Azure.

Examples include:
- Virtual machines
- Storage accounts
- Storage containers
- Databases
- Virtual networks

### Real-World Thinking
If you create an Azure Virtual Machine, the VM is a resource. Its networking, storage, and related components may also be individual Azure resources.

### Exam Thinking
> **Resource = an individual Azure service or asset.**

Resources are placed inside **Resource Groups**.

---

# Resource Groups

A **Resource Group** is a logical container that holds related Azure resources.

## Key Features

### Lifecycle Management
Resources that share a common lifecycle can be grouped together. Deleting a Resource Group also removes the resources contained within it.

### Access Control
Azure Role-Based Access Control (RBAC) can be applied at the Resource Group level.

### Cost Tracking
Resource Groups can help organize and analyze costs associated with a project, application, or department.

### Metadata Location
A Resource Group has a location where its metadata is stored. Resources inside the group can exist in different Azure regions.

### Real-World Thinking
An organization could create `RG-Accounting-App` and place the application's VM, storage, network, and database resources inside it.

### Exam Thinking
> **Resource Group = logical container for related Azure resources.**

> A Resource Group does **not** require every resource inside it to be in the same Azure region.

---

# Azure Subscriptions

An **Azure Subscription** is a logical container used to organize, manage, and bill Azure resources.

## Key Concepts

### Billing Boundary
Subscriptions can provide separate billing and cost tracking.

### Access Control
RBAC and other management controls can be applied at the subscription level.

### Subscription ID
Each subscription has a unique **Subscription ID**.

### Subscription Types
Examples include Free Accounts, Pay-As-You-Go, and Enterprise Agreements.

### Real-World Thinking
A company could use separate subscriptions for **Production**, **Development**, and **Testing**, or separate subscriptions for different departments.

### Exam Thinking
> **Subscription = management and billing boundary containing Resource Groups and resources.**

---

# Management Groups

**Management Groups** are containers used to organize and manage multiple Azure subscriptions.

They allow organizations to apply governance, access, and policies across subscriptions through a hierarchy.

## Key Features

### Hierarchy
Management Groups can be arranged into a hierarchy.

### Inheritance
Subscriptions and Management Groups below a parent inherit applicable rules and permissions from higher scopes.

### Tenant Root Management Group
Every directory has a default Tenant Root Management Group at the top.

### Single Parent
Each subscription or Management Group can connect to one parent at a time.

## Main Benefits
- Apply governance across multiple subscriptions.
- Apply access controls at a higher level.
- Organize subscriptions by department, region, project, or business function.
- Reduce repetitive administration.

### Real-World Thinking

```text
Tenant Root
|
+-- Production
|   +-- Production Subscription 1
|   +-- Production Subscription 2
|
+-- Development
    +-- Development Subscription 1
    +-- Development Subscription 2
```

### Exam Thinking
> **Management Group = container used to organize and govern multiple subscriptions.**

Think **above subscriptions**.

---

# Resource Group vs. Subscription vs. Management Group

| Level | Contains / Organizes | Common Purpose |
|---|---|---|
| **Management Group** | Subscriptions and Management Groups | Governance across subscriptions |
| **Subscription** | Resource Groups and resources | Billing and management boundary |
| **Resource Group** | Azure resources | Logical organization and lifecycle management |
| **Resource** | Individual Azure service | Actual cloud workload or component |

### Easy Way to Remember

```text
Management Group = Manage MANY subscriptions
Subscription     = Billing + management boundary
Resource Group   = Group related resources
Resource         = Actual Azure service
```

---

# Why Use Multiple Subscriptions?

Organizations may use multiple subscriptions to separate:
- Billing
- Departments
- Environments
- Projects
- Access requirements
- Administrative boundaries

### Real-World Thinking
An organization might separate **Production** from **Development** to make access, billing, and management easier.

### Exam Thinking
> **Multiple subscriptions can provide separate billing and management boundaries.**

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 05 Lab — Azure Architecture II](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-05-Lab-05-Azure-Architecture-II.md)**

### Lab Focus
- Create a Resource Group.
- View your Azure Subscription.
- Explore Management Groups.
- Review moving resources between Resource Groups.
- Practice identifying the Azure resource hierarchy.

> [!TIP]
> The lab contains the Azure Portal and Microsoft documentation links needed for each activity.

---

# Quick Check

| Question | Answer |
|---|---|
| Individual Azure service or asset | Resource |
| Logical container for related resources | Resource Group |
| Billing and management boundary | Subscription |
| Organizes and governs multiple subscriptions | Management Group |
| Level directly above Resource Groups | Subscription |
| Level used to organize multiple subscriptions | Management Group |

---

# Before Moving On

You should be able to:
- Explain the purpose of a Resource.
- Explain the purpose of a Resource Group.
- Explain the purpose of a Subscription.
- Explain the purpose of a Management Group.
- Know the Azure resource hierarchy.
- Explain why organizations use multiple subscriptions.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Resource** | Individual Azure service or asset |
| **Resource Group** | Logical container for related resources |
| **Subscription** | Billing and management boundary |
| **Management Group** | Organizes and governs subscriptions |
| **Hierarchy** | Management Group → Subscription → Resource Group → Resource |
| **Inheritance** | Higher-level governance can apply to child scopes |
| **Multiple Subscriptions** | Separate billing, access, environments, or departments |
