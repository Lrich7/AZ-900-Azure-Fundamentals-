[Lesson-16-Governance.md](https://github.com/user-attachments/files/31148826/Lesson-16-Governance.md)
# Lesson 16 — Governance

## 📖 Microsoft Learn

**Documentation:** Azure Policy Overview  
https://learn.microsoft.com/en-us/azure/governance/policy/overview

### Focus
- Azure Policy
- Resource Locks
- Resource Tags
- Azure Policy vs. Azure RBAC

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Functionality and Usage of Azure Policy | 10:50 | https://youtu.be/z7WMqHE3R8g |
| Functionality and Usage of Resource Locks | 6:16 | https://youtu.be/eF_KilJRxbE |
| Functionality and Usage of Tags | 5:06 | https://youtu.be/eaf63hE_6SQ |

---

# Azure Governance

**Governance** is about controlling, organizing, and maintaining Azure resources according to an organization's requirements.

Three important governance tools are:

- **Azure Policy** — enforce standards and evaluate compliance.
- **Resource Locks** — protect resources from accidental changes or deletion.
- **Tags** — organize and categorize resources using metadata.

```text
Azure Governance
      |
      +-- Azure Policy
      |      Enforce standards
      |
      +-- Resource Locks
      |      Protect resources
      |
      +-- Tags
             Organize resources
```

### Exam Thinking

```text
Policy = ENFORCE
Locks  = PROTECT
Tags   = ORGANIZE
```

---

# Azure Policy

**Azure Policy** is an Azure governance service used to create, assign, and manage rules that enforce organizational standards and assess compliance.

Policies can evaluate Azure resources to determine whether they meet organizational requirements.

## Common Uses

Azure Policy can help organizations:

- Enforce organizational standards.
- Audit resource configurations.
- Restrict certain resource configurations.
- Require specific settings.
- Assess compliance across Azure environments.
- Remediate certain non-compliant resources.

### Real-World Thinking

A company requires all Azure resources to follow specific organizational rules.

Instead of relying on administrators to remember every requirement, Azure Policy can evaluate resources against those standards.

### Exam Thinking

> **Azure Policy = enforce organizational standards and assess compliance.**

---

# Azure Policy Components

Azure Policy uses several important components.

## Policy Definitions

A **Policy Definition** describes the rule that Azure should evaluate.

Definitions are expressed using JSON and contain conditions and effects.

Examples of effects include:

- Audit
- Deny
- Modify

### Exam Thinking

> **Policy Definition = the individual rule.**

---

# Policy Initiatives

An **Initiative** is a collection of multiple Policy Definitions grouped together toward a common goal.

```text
Initiative
    |
    +-- Policy Definition 1
    +-- Policy Definition 2
    +-- Policy Definition 3
```

### Real-World Thinking

Instead of assigning many individual security policies separately, an organization can group related policies into an initiative.

### Exam Thinking

> **Initiative = group of Policy Definitions.**

---

# Policy Assignments

A **Policy Assignment** applies a Policy Definition or Initiative to a particular scope.

Assignments can target scopes such as:

- Management Groups
- Subscriptions
- Resource Groups
- Individual resources

### Exam Thinking

> **Policy Assignment = apply a policy to a scope.**

---

# Azure Policy Scope

Policy assignments can be applied at different levels of the Azure resource hierarchy.

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

Policies assigned at a parent scope can affect resources beneath that scope.

Organizations can also configure exclusions where appropriate.

### Exam Thinking

> **Policy scope determines where the policy applies.**

---

# Policy Evaluation and Compliance

Azure Policy evaluates resources to determine whether they comply with assigned policies.

Evaluation can occur when resources are:

- Created
- Updated
- Re-evaluated during compliance checks

Azure Policy provides compliance information so administrators can identify resources that do not meet organizational standards.

### Real-World Thinking

An administrator can use the Azure Policy compliance view to identify resources that do not meet required configurations.

---

# Policy Remediation

Some policies support **remediation** of existing non-compliant resources.

Remediation tasks can help bring supported resources into compliance rather than only identifying the problem.

### Exam Thinking

```text
Audit       = Identify a problem
Deny        = Prevent a configuration
Modify      = Change supported properties
Remediation = Help correct existing non-compliance
```

---

# Resource Locks

**Resource Locks** help prevent accidental changes or deletion of important Azure resources.

There are two primary lock types:

- **Delete** (`CanNotDelete`)
- **Read-only** (`ReadOnly`)

---

# Delete Lock

A **Delete lock** allows authorized users to read and modify the resource but prevents deletion.

### Real-World Thinking

A production resource should still be configurable by administrators, but it should not be accidentally deleted.

A Delete lock can provide that protection.

### Exam Thinking

> **Delete / CanNotDelete = changes allowed, deletion blocked.**

---

# Read-Only Lock

A **Read-only lock** allows authorized users to read the resource but prevents updates and deletion through the management plane.

### Exam Thinking

> **ReadOnly = read allowed, changes and deletion blocked.**

---

# Resource Lock Scope and Inheritance

Locks can be applied at supported scopes such as:

- Subscription
- Resource Group
- Individual resource

A lock applied at a parent scope can be inherited by resources beneath that scope.

```text
Resource Group
   LOCKED
      |
      +-- VM
      |
      +-- Storage Account
      |
      +-- VNet
```

The child resources inherit the lock.

### Exam Thinking

> **Parent-level locks can affect child resources.**

---

# Resource Locks and Permissions

Resource Locks are different from Azure RBAC.

An administrator may have permission to manage a resource through RBAC, but an applicable Resource Lock can still prevent a locked management operation.

This includes users with powerful roles such as Owner.

### Important Distinction

Resource Locks primarily affect **control-plane management operations**.

They do not necessarily prevent data-plane operations inside the resource.

### Example

A lock on a Storage Account may prevent management operations against the Storage Account itself while not necessarily preventing an authorized application from writing data into storage.

### Exam Thinking

> **Resource Lock = protection against management-plane changes or deletion.**

---

# Azure Tags

**Tags** are custom metadata labels that help organize, categorize, and track Azure resources.

Tags use **key-value pairs**.

```text
Key           Value
-------------------------
Environment   Production
Department    Finance
Owner         IT
CostCenter    1001
```

## Common Uses

### Cost Management

Tags can help categorize resources for reporting and cost analysis.

### Environment Tracking

Examples:

```text
Environment = Production
Environment = Development
Environment = Test
```

### Ownership

Tags can identify the team, department, or owner responsible for a resource.

### Organization

Tags provide metadata that can make large Azure environments easier to organize and understand.

### Real-World Thinking

A company wants to distinguish production resources from development resources and identify which department is responsible for each resource.

Tags can provide that metadata.

### Exam Thinking

> **Tags = key-value metadata used to organize and categorize Azure resources.**

---

# Tags Are Not Security

Tags help organize resources, but they do not grant or deny permissions.

```text
Tags   = LABEL resources
RBAC   = CONTROL permissions
Policy = ENFORCE standards
```

### Exam Thinking

> **A tag describes a resource. It does not secure the resource.**

---

# Azure Policy vs. Azure RBAC

This is an important AZ-900 distinction.

## Azure RBAC

Controls **who** can perform actions on Azure resources.

## Azure Policy

Controls **what configurations are allowed or required** and evaluates compliance.

| Feature | Primary Question |
|---|---|
| **Azure RBAC** | Who can perform this action? |
| **Azure Policy** | Is this resource configuration allowed or compliant? |

### Example

```text
RBAC
"Can Alex create a VM?"

Policy
"If Alex creates a VM, what configurations are allowed?"
```

### Memory Trick

```text
RBAC   = WHO CAN DO IT?
Policy = WHAT IS ALLOWED?
```

---

# Policy vs. Locks vs. Tags

| Feature | Primary Purpose |
|---|---|
| **Azure Policy** | Enforce standards and assess compliance |
| **Resource Locks** | Prevent accidental deletion or modification |
| **Tags** | Organize and categorize resources |

### Easy Way to Remember

```text
POLICY = Rules
LOCKS  = Protection
TAGS   = Labels
```

---

# Choosing the Right Governance Tool

### Choose Azure Policy when:
- Resources must follow organizational standards.
- You need compliance reporting.
- A configuration should be audited or denied.
- A setting should be required across many resources.

### Choose Resource Locks when:
- An important resource must not be accidentally deleted.
- A resource should be protected from management changes.

### Choose Tags when:
- Resources need labels.
- Costs need to be categorized.
- Resources need to be identified by environment, department, owner, or another business value.

### Choose Azure RBAC when:
- You need to control who can perform actions.
- A user or group needs specific Azure resource permissions.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 16 Lab — Governance](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-16-Lab-16-Governance.md)**

### Lab Focus

- Browse Azure Policy.
- Review built-in Policy Definitions.
- Explore Initiatives and Assignments.
- Review Policy Compliance.
- Browse Resource Locks.
- Explore Tags.
- Compare Azure Policy and Azure RBAC.
- Practice Policy vs. Lock vs. Tag scenarios.

> [!TIP]
> Governance settings can affect many Azure resources. The lab focuses on safe exploration rather than modifying production policies or locks.

---

# Quick Check

| Need | Azure Feature |
|---|---|
| Enforce organizational standards | Azure Policy |
| Group multiple Policy Definitions | Initiative |
| Apply a Policy to a scope | Assignment |
| Prevent accidental deletion | Resource Lock |
| Organize resources with metadata | Tags |
| Control who can perform actions | Azure RBAC |
| Control what configurations are allowed | Azure Policy |

---

# Before Moving On

You should be able to:

- Explain the purpose of Azure Policy.
- Explain Policy Definitions, Initiatives, and Assignments.
- Explain Policy scope and compliance.
- Explain the difference between Azure Policy and Azure RBAC.
- Explain Delete and Read-only Resource Locks.
- Explain lock inheritance.
- Explain the purpose of Tags.
- Identify when to use Policies, Locks, Tags, and RBAC.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Azure Policy** | Enforce standards and compliance |
| **Policy Definition** | Individual rule |
| **Initiative** | Group of policies |
| **Assignment** | Apply policy to scope |
| **Resource Lock** | Protect resource management operations |
| **Delete Lock** | Prevent deletion |
| **Read-Only Lock** | Prevent changes and deletion |
| **Tags** | Key-value organizational metadata |
| **Azure RBAC** | Who can perform actions |
| **Azure Policy vs. RBAC** | What is allowed vs. who can do it |
