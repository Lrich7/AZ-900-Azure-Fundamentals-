[Lesson-14-Identity-and-Access.md](https://github.com/user-attachments/files/31148793/Lesson-14-Identity-and-Access.md)

# Lesson 14 — Identity & Access

## 📖 Microsoft Learn

**Module:** Secure Your Azure Resources with Role-Based Access Control (RBAC)  
https://learn.microsoft.com/en-us/training/modules/secure-your-azure-resources-with-rbac/

### Focus
- Microsoft Entra ID
- Role-Based Access Control (RBAC)
- Conditional Access
- Multi-Factor Authentication (MFA)
- Single Sign-On (SSO)
- Least Privilege

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Overview of Microsoft Entra | 11:34 | https://youtu.be/bSIF_GjaCmo |
| Functionality of Conditional Access, MFA and SSO | 12:29 | https://youtu.be/DFwERh9Xxk0 |
| Functionality and Usage of RBAC | 9:19 | https://youtu.be/0iVyJBG06fM |

---

# Identity and Access Management

Identity and access management helps answer two important questions:

```text
Authentication
WHO ARE YOU?
      |
      v
Authorization
WHAT ARE YOU ALLOWED TO DO?
```

Microsoft Entra ID provides cloud identity and access management, while features such as **MFA, SSO, Conditional Access, and Azure RBAC** help secure identities and resources.

---

# Microsoft Entra ID

**Microsoft Entra ID** is Microsoft's cloud-based identity and access management service.

It was formerly known as **Azure Active Directory (Azure AD)**.

Microsoft Entra ID can help organizations manage access to:

- Microsoft 365
- Azure
- Enterprise applications
- Third-party cloud applications

## Important Capabilities

### Single Sign-On (SSO)

Allows users to sign in and then access multiple authorized applications without repeatedly entering credentials.

### Conditional Access

Evaluates sign-in and access conditions and applies configured access controls.

### Hybrid Identity

Supports connecting supported on-premises identity environments with Microsoft Entra ID.

### Exam Thinking

> **Microsoft Entra ID = cloud identity and access management.**

---

# Azure Role-Based Access Control (RBAC)

**Azure Role-Based Access Control (Azure RBAC)** controls who has access to Azure resources, what they can do, and where that access applies.

Azure RBAC is an **authorization** system.

### Exam Thinking

> **Azure RBAC = control access to Azure resources through roles and scope.**

---

# The Three Main Parts of Azure RBAC

An Azure role assignment combines:

```text
WHO
Security Principal
      +
WHAT
Role Definition
      +
WHERE
Scope
```

---

## Security Principal — WHO

A **Security Principal** represents an identity requesting access.

Examples include:

- User
- Group
- Service principal
- Managed identity

### Exam Thinking

> **Security Principal = who receives the access.**

---

## Role Definition — WHAT

A **Role Definition** is a collection of permissions.

Common built-in Azure roles include:

### Owner

Can manage resources and can assign Azure roles.

### Contributor

Can create and manage resources but cannot assign Azure roles.

### Reader

Can view resources but cannot make changes.

### Easy Way to Remember

```text
Owner       = Manage + assign access
Contributor = Manage
Reader      = View
```

### Exam Thinking

> **Role Definition = what actions are allowed.**

---

## Scope — WHERE

**Scope** determines where the role assignment applies.

Azure RBAC can be assigned at different levels:

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

A role assigned at a higher scope can apply to resources below that scope.

### Exam Thinking

> **Scope = where the permissions apply.**

---

# Principle of Least Privilege

The **Principle of Least Privilege** means giving users, applications, and services only the minimum permissions required to perform their tasks.

## Why It Matters

Least privilege helps reduce:

- Accidental changes
- Unauthorized access
- Data exposure
- Damage from compromised accounts

### Real-World Thinking

If an employee only needs to view Azure resources, assigning **Reader** is safer than assigning **Owner**.

### Exam Thinking

> **Least Privilege = give only the permissions needed.**

---

# Conditional Access

**Conditional Access** is a Microsoft Entra feature that evaluates signals and applies access controls based on configured policies.

It is commonly described using **if-then** logic.

```text
IF
Sign-in meets a condition
      |
      v
THEN
Apply an access control
```

## Signals

Conditional Access can evaluate signals such as:

- User or group
- Location
- Device
- Application
- Risk-related information

## Decisions and Enforcement

A policy can apply controls such as:

- Require MFA
- Require a compliant device
- Block access

### Example

```text
IF
An administrator signs in
      |
      v
THEN
Require MFA
```

### Real-World Thinking

An organization wants administrator accounts to complete additional verification before accessing cloud resources.

Conditional Access can require MFA when the policy conditions are met.

### Exam Thinking

> **Conditional Access = if-then access policies based on signals and conditions.**

---

# Multi-Factor Authentication (MFA)

**Multi-Factor Authentication (MFA)** requires users to verify their identity using two or more authentication factors.

The common factor categories are:

### Something You Know

Example: password or PIN.

### Something You Have

Example: phone, authenticator, or security key.

### Something You Are

Example: fingerprint or facial recognition.

### Real-World Thinking

A user enters a password and then approves an authentication request using another factor.

Even if the password is compromised, the attacker may still be unable to complete authentication.

### Exam Thinking

> **MFA = two or more authentication factors.**

---

# Single Sign-On (SSO)

**Single Sign-On (SSO)** allows users to authenticate and access multiple authorized applications without repeatedly signing in to each one.

## Benefits

- Fewer repeated sign-ins
- Reduced password fatigue
- Simplified access experience
- Centralized identity management

### Real-World Thinking

An employee signs in with a work account and can then access authorized Microsoft 365 and enterprise applications without entering credentials for each application separately.

### Exam Thinking

> **SSO = sign in once, access multiple authorized applications.**

---

# MFA vs. SSO vs. Least Privilege

These concepts work together but solve different problems.

| Feature | Primary Purpose |
|---|---|
| **MFA** | Strengthen identity verification |
| **SSO** | Reduce repeated sign-ins |
| **Least Privilege** | Limit permissions to what is needed |

### Easy Way to Remember

```text
MFA             = PROVE who you are securely
SSO             = SIGN IN once
Least Privilege = ACCESS only what you need
```

---

# Company Network Analogy

Imagine signing into your company's environment:

```text
MFA
Password + another factor
      |
      v
SSO
Open multiple authorized apps
without repeated sign-ins
      |
      v
RBAC / Least Privilege
Access only the Azure resources
and actions required for your job
```

---

# RBAC vs. Conditional Access

These two concepts are easy to confuse.

| Feature | Primary Question |
|---|---|
| **Conditional Access** | Under what conditions should access be allowed or challenged? |
| **Azure RBAC** | What can this identity do to Azure resources, and at what scope? |

### Exam Thinking

```text
Conditional Access = ACCESS CONDITIONS
Azure RBAC         = RESOURCE PERMISSIONS
```

---

# Comparing Identity & Access Features

| Concept | Primary Purpose |
|---|---|
| **Microsoft Entra ID** | Cloud identity and access management |
| **Azure RBAC** | Azure resource authorization |
| **Conditional Access** | Condition-based access policies |
| **MFA** | Multiple authentication factors |
| **SSO** | One sign-in for multiple applications |
| **Least Privilege** | Minimum required permissions |

---

# Choosing the Right Feature

### Choose Azure RBAC when:
- You need to control access to Azure resources.
- You need to assign Reader, Contributor, Owner, or another role.
- A question asks who can perform an action at a particular Azure scope.

### Choose Conditional Access when:
- Access should depend on conditions or signals.
- MFA should be required under specific circumstances.
- Access should be blocked based on configured policy conditions.

### Choose MFA when:
- More than one authentication factor is required.
- Additional identity verification is needed.

### Choose SSO when:
- Users should sign in once and access multiple authorized applications.

### Think Least Privilege when:
- A user should receive only the permissions necessary for their job.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 14 Lab — Identity & Access](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-14-Lab-14-Identity-and-Access.md)**

### Lab Focus

- Explore Azure roles and role assignments.
- Review RBAC scope.
- Explore Conditional Access.
- Review authentication and MFA settings.
- Explore Enterprise Applications and SSO.
- Practice RBAC, Conditional Access, MFA, SSO, and least-privilege scenarios.

> [!TIP]
> Identity and access configuration can affect real users. The lab focuses primarily on safe exploration rather than changing production settings.

---

# Quick Check

| Need | Feature |
|---|---|
| Cloud identity management | Microsoft Entra ID |
| Control Azure resource permissions | Azure RBAC |
| Apply access rules based on conditions | Conditional Access |
| Require multiple authentication factors | MFA |
| Sign in once to multiple applications | SSO |
| Grant only necessary permissions | Least Privilege |

---

# Before Moving On

You should be able to:

- Explain the purpose of Microsoft Entra ID.
- Explain Authentication vs. Authorization.
- Explain Azure RBAC.
- Identify Security Principal, Role Definition, and Scope.
- Explain Conditional Access.
- Explain MFA.
- Explain SSO.
- Explain Least Privilege.
- Know when each identity and access feature should be used.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Microsoft Entra ID** | Cloud identity and access management |
| **Azure RBAC** | Who can do what, and where |
| **Security Principal** | Who |
| **Role Definition** | What |
| **Scope** | Where |
| **Conditional Access** | If-then access policies |
| **MFA** | Multiple authentication factors |
| **SSO** | Sign in once |
| **Least Privilege** | Minimum required permissions |
