# Lab 16 — Governance

## Objective

This lab reinforces **Lesson 16 — Governance**.

By the end, you should be able to:

- Navigate Azure Policy.
- Review built-in Policy Definitions.
- Identify Policy Initiatives and Assignments.
- Review Policy Compliance.
- Explore Resource Locks.
- Explore Azure Tags.
- Compare Azure Policy and Azure RBAC.
- Choose the correct governance feature for common AZ-900 scenarios.

---

# Prerequisites

- Completed **Lesson 16 — Governance**
- Web browser
- Azure account with appropriate read access

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Azure Policy Overview:** https://learn.microsoft.com/en-us/azure/governance/policy/overview
- **Resource Locks:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/lock-resources
- **Azure Tags:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources

> [!IMPORTANT]
> Azure Policy and Resource Locks can affect real resources across subscriptions and Resource Groups. Unless you are using a dedicated lab environment, **review the configuration screens without assigning policies, creating locks, or changing production tags**.

---

# Part 1 — Explore Azure Policy

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Policy Overview:** https://learn.microsoft.com/en-us/azure/governance/policy/overview

## Steps

1. Open the Azure Portal.
2. Search for **Policy**.
3. Open **Azure Policy**.
4. Review the available navigation areas.
5. Look for:
   - Definitions
   - Assignments
   - Compliance
   - Remediation
6. Do not create or change Policy Assignments.

## Think About It

What is the primary purpose of Azure Policy?

**Answer:** _______________________________________________

Does Azure Policy primarily control user permissions or resource configurations?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Policy = enforce organizational standards and assess compliance.**

---

# Part 2 — Review Built-In Policy Definitions

### Links

- **Azure Policy Built-In Definitions:** https://learn.microsoft.com/en-us/azure/governance/policy/samples/built-in-policies
- **Azure Portal:** https://portal.azure.com/

## Steps

1. In Azure Policy, open **Definitions**.
2. Review several built-in Policy Definitions.
3. Search or filter for policies if the portal provides those options.
4. Open a definition and review its information.
5. Look for:
   - Name
   - Description
   - Category
   - Policy rule
   - Effect
6. Do not assign the policy.

## Think About It

What is a Policy Definition?

**Answer:** _______________________________________________

Name one possible Policy effect.

**Answer:** _______________________________________________

### Exam Thinking

```text
Definition = RULE
Effect     = WHAT HAPPENS
```

---

# Part 3 — Explore Initiatives

### Links

- **Azure Policy Initiative Definitions:** https://learn.microsoft.com/en-us/azure/governance/policy/concepts/initiative-definition-structure

## Steps

1. In Azure Policy **Definitions**, locate examples of **Initiative Definitions** if available.
2. Open an initiative.
3. Review the Policy Definitions grouped inside it.
4. Do not create or assign an initiative.

## Think About It

What is the purpose of an Initiative?

**Answer:** _______________________________________________

Why might an organization use an Initiative instead of assigning many policies individually?

**Answer:** _______________________________________________

### Exam Thinking

> **Initiative = collection of Policy Definitions.**

---

# Part 4 — Explore Policy Assignments and Scope

### Links

- **Azure Policy Assignment Structure:** https://learn.microsoft.com/en-us/azure/governance/policy/concepts/assignment-structure
- **Azure Policy Scope:** https://learn.microsoft.com/en-us/azure/governance/policy/concepts/scope

## Steps

1. Open **Assignments** in Azure Policy.
2. Review existing assignments if your permissions allow it.
3. Open a safe assignment without changing it.
4. Look for the assigned:
   - Policy or Initiative
   - Scope
   - Exclusions
5. Identify whether the scope is a:
   - Management Group
   - Subscription
   - Resource Group
   - Resource

## Think About It

What does a Policy Assignment do?

**Answer:** _______________________________________________

If a Policy is assigned to a Resource Group, which resources can be affected?

**Answer:** _______________________________________________

### Exam Thinking

> **Assignment = apply Policy to a scope.**

---

# Part 5 — Review Policy Compliance

### Links

- **Azure Policy Compliance:** https://learn.microsoft.com/en-us/azure/governance/policy/how-to/get-compliance-data

## Steps

1. In Azure Policy, open **Compliance**.
2. Review compliance information available to your account.
3. Look for:
   - Compliant resources
   - Non-compliant resources
   - Assigned policies
4. Do not run remediation tasks against production resources.

## Think About It

What does **non-compliant** mean?

**Answer:** _______________________________________________

Why is compliance reporting useful?

**Answer:** _______________________________________________

---

# Part 6 — Explore Resource Locks

### Links

- **Lock Azure Resources:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/lock-resources
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open a safe Resource Group or test resource.
2. Locate **Locks**.
3. Review any existing locks.
4. If there are no locks, review the **Add** screen without saving.
5. Identify the available lock types.
6. Do not create or remove a lock on production resources.

Complete the table:

| Lock Type | Can Read? | Can Modify? | Can Delete? |
|---|:---:|:---:|:---:|
| **Delete / CanNotDelete** | ______ | ______ | ______ |
| **ReadOnly** | ______ | ______ | ______ |

## Think About It

If a Delete lock is applied to a Resource Group, what happens to resources inside it?

**Answer:** _______________________________________________

Can an Owner simply ignore an applicable Resource Lock?

**Answer:** _______________________________________________

### Exam Thinking

```text
Delete Lock = NO DELETE
ReadOnly    = NO CHANGE / NO DELETE
```

---

# Part 7 — Explore Azure Tags

### Links

- **Use Tags to Organize Azure Resources:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open a safe Azure resource or Resource Group.
2. Locate **Tags**.
3. Review any existing tags.
4. If none exist, review how a key and value would be entered without saving.
5. Consider examples such as:

```text
Environment = Production
Department  = IT
Owner       = Infrastructure
CostCenter  = 1001
```

6. Do not modify production tags unless authorized.

## Think About It

What are the two parts of an Azure Tag?

**Answer:** _______________________________________________

Name two ways an organization might use Tags.

**Answer:** _______________________________________________

Do Tags grant Azure permissions?

**Answer:** _______________________________________________

### Exam Thinking

> **Tags = key-value metadata for organization and tracking.**

---

# Part 8 — Azure Policy vs. Azure RBAC

Choose:

- **Azure Policy**
- **Azure RBAC**

### Scenario 1

A user needs permission to create virtual machines.

**Answer:** ______________________________

### Scenario 2

Virtual machines are only allowed in approved Azure regions.

**Answer:** ______________________________

### Scenario 3

A user should only be able to view a Resource Group.

**Answer:** ______________________________

### Scenario 4

All resources must follow an organizational configuration standard.

**Answer:** ______________________________

### Memory Trick

```text
RBAC   = WHO CAN DO IT?
Policy = WHAT IS ALLOWED?
```

---

# Part 9 — Policy, Lock, or Tag?

Choose:

- **Azure Policy**
- **Resource Lock**
- **Tag**

### Scenario 1

A company wants to identify which department owns each Azure resource.

**Answer:** ______________________________

### Scenario 2

A production database must not be accidentally deleted.

**Answer:** ______________________________

### Scenario 3

Resources that do not follow an organizational standard should be identified.

**Answer:** ______________________________

### Scenario 4

Resources should be categorized as Production, Test, or Development.

**Answer:** ______________________________

### Scenario 5

A particular resource configuration should be denied.

**Answer:** ______________________________

### Scenario 6

Administrators should be prevented from accidentally changing or deleting a critical resource through management operations.

**Answer:** ______________________________

---

# Part 10 — Governance Review

Complete the table:

| Description | Azure Concept |
|---|---|
| Individual Policy rule | __________________ |
| Collection of Policy Definitions | __________________ |
| Applies Policy to a scope | __________________ |
| Reports whether resources meet standards | __________________ |
| Prevents accidental management deletion | __________________ |
| Key-value resource metadata | __________________ |
| Controls user permissions | __________________ |

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

Azure Policy enforces organizational standards and evaluates resource compliance. It primarily evaluates resource configurations rather than granting user permissions.

## Part 2

A Policy Definition is an individual rule. Effects can include examples such as **Audit**, **Deny**, or **Modify**.

## Part 3

An Initiative groups multiple Policy Definitions together toward a common governance goal.

## Part 4

A Policy Assignment applies a Policy Definition or Initiative to a scope. A Resource Group assignment can affect resources within that Resource Group.

## Part 5

A non-compliant resource does not meet the requirements of an applicable policy. Compliance reporting helps administrators identify resources that need attention.

## Part 6

| Lock Type | Read | Modify | Delete |
|---|:---:|:---:|:---:|
| Delete / CanNotDelete | Yes | Yes | No |
| ReadOnly | Yes | No | No |

A lock inherited from a Resource Group can affect child resources. Applicable locks restrict management operations even when a user has powerful RBAC permissions.

## Part 7

A Tag consists of a **key** and a **value**. Tags can categorize resources by environment, department, owner, cost center, or other business metadata. Tags do not grant permissions.

## Part 8

| Scenario | Answer |
|---|---|
| 1 | Azure RBAC |
| 2 | Azure Policy |
| 3 | Azure RBAC |
| 4 | Azure Policy |

## Part 9

| Scenario | Answer |
|---|---|
| 1 | Tag |
| 2 | Resource Lock |
| 3 | Azure Policy |
| 4 | Tag |
| 5 | Azure Policy |
| 6 | Resource Lock |

## Part 10

| Description | Answer |
|---|---|
| Individual Policy rule | Policy Definition |
| Collection of Policy Definitions | Initiative |
| Applies Policy to a scope | Assignment |
| Reports whether resources meet standards | Policy Compliance |
| Prevents accidental management deletion | Resource Lock |
| Key-value resource metadata | Tag |
| Controls user permissions | Azure RBAC |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Azure Policy.
- Policy Definitions, Initiatives, and Assignments.
- Policy scope and compliance.
- Azure Policy vs. Azure RBAC.
- Delete vs. Read-only Resource Locks.
- Resource Lock inheritance.
- Azure Tags.
- Policy vs. Lock vs. Tag.
- Which governance feature best fits a basic AZ-900 scenario.
