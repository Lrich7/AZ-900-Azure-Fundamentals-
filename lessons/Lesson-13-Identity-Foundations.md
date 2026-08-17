[Lesson-13-Identity-Foundations.md](https://github.com/user-attachments/files/31148783/Lesson-13-Identity-Foundations.md)

# Lesson 13 — Identity Foundations

## 📖 Microsoft Learn

**Module:** Describe Core Architectural Components of Azure  
https://learn.microsoft.com/en-us/training/modules/describe-core-architectural-components-of-azure/

### Focus
- Authentication
- Authorization
- Directory Services
- Microsoft Entra ID
- External Identities

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Explain Authentication and Authorization | 3:52 | https://youtu.be/GA-yNu6aFMk |
| Describe Azure Directory Services | 14:06 | https://youtu.be/E4__JBVE25I |
| Describe Azure External Identities | 11:14 | https://youtu.be/G5_z4PFgn2o |

---

# Identity and Access

Identity is a core part of cloud security.

Before a user, application, or device can access a resource, Azure needs to determine:

1. **Who or what is requesting access?**
2. **What is that identity allowed to do?**

These questions lead to two important concepts:

```text
Authentication
WHO ARE YOU?
      |
      v
Authorization
WHAT CAN YOU DO?
```

### Exam Thinking

> **Authenticate first, authorize second.**

---

# Authentication

**Authentication** is the process of verifying the identity of a user, application, or device before access is granted.

Authentication answers:

> **Who are you?**

Common authentication methods include:

- Passwords
- Multifactor authentication (MFA)
- Biometrics
- Security keys

### Real-World Thinking

When an employee signs in with a username and password and then approves an MFA prompt, the organization is verifying that person's identity.

### Exam Thinking

> **Authentication = prove your identity.**

---

# Authorization

**Authorization** determines what an authenticated identity is allowed to access or do.

Authorization answers:

> **What are you allowed to do?**

Permissions can be controlled through:

- Roles
- Policies
- Access controls

### Real-World Thinking

Two employees may both successfully sign in, but only one may have permission to administer a particular resource.

Both users are authenticated, but their authorization is different.

### Exam Thinking

> **Authorization = determine permissions.**

---

# Authentication vs. Authorization

| Concept | Question | Purpose |
|---|---|---|
| **Authentication** | Who are you? | Verify identity |
| **Authorization** | What can you do? | Determine access and permissions |

### Easy Way to Remember

```text
Authentication = IDENTITY
Authorization  = PERMISSIONS
```

### Common AZ-900 Exam Tip

A user normally needs to be **authenticated first**. Azure can then determine what that authenticated identity is **authorized** to access.

---

# Directory Services

**Directory Services** store and organize information about identities and resources in an organization.

A directory may contain information about:

- Users
- Groups
- Devices
- Applications
- Other identity-related resources

Directory services provide centralized identity management and help support authentication and access control.

### Real-World Thinking

Instead of managing separate user accounts independently in every application, an organization can use a centralized directory to manage identities.

### Exam Thinking

> **Directory Services = centralized storage and management of identities.**

---

# Microsoft Entra ID

**Microsoft Entra ID** is Microsoft's cloud-based identity and access management service.

It was formerly known as **Azure Active Directory (Azure AD)**.

Microsoft Entra ID can help organizations manage access to resources such as:

- Microsoft 365
- Azure
- Enterprise applications
- Third-party cloud applications

## Important Capabilities

### Single Sign-On (SSO)

Allows users to authenticate and then access multiple authorized applications without repeatedly signing in to each one.

### Conditional Access

Allows organizations to evaluate access conditions and apply access requirements or controls.

### Hybrid Identity

Organizations can connect supported on-premises identity environments with Microsoft Entra ID so identities can work across cloud and on-premises environments.

### Real-World Thinking

An employee uses one work identity to access Microsoft 365 and other approved cloud applications.

Microsoft Entra ID provides the cloud identity and access-management foundation.

### Exam Thinking

> **Microsoft Entra ID = cloud identity and access management.**

---

# Microsoft Entra ID vs. Traditional Directory Services

For AZ-900, focus on the basic distinction:

| Concept | Primary Idea |
|---|---|
| **Directory Services** | Store and manage identity information |
| **Microsoft Entra ID** | Microsoft's cloud identity and access management service |

Microsoft Entra ID is a cloud-based directory and identity platform designed for modern cloud authentication and application access.

---

# External Identities

**External Identities** allow people outside an organization to securely access applications and resources when access is granted.

Examples can include:

- Partners
- Vendors
- Contractors
- Customers

Microsoft Entra External ID helps organizations provide external access while maintaining control over security and permissions.

### Real-World Thinking

A contractor needs access to one company application but should not receive the same access as a full-time employee.

An external identity can be given only the access required.

### Exam Thinking

> **External Identities = secure access for users outside the organization.**

---

# Secure Office Building Analogy

Think of identity like entering a secure office building:

```text
Authentication
Show your badge
"Who are you?"
      |
      v
Authorization
Badge controls which rooms you can enter
"What can you do?"
      |
      v
Directory Services
Employee directory stores identity information
      |
      v
External Identities
Contractor receives controlled external access
```

| Identity Concept | Office Analogy |
|---|---|
| **Authentication** | Show your badge |
| **Authorization** | Badge determines which rooms you can enter |
| **Directory Services** | Employee directory |
| **External Identities** | Contractor or guest badge |

---

# Comparing Identity Concepts

| Concept | Primary Purpose |
|---|---|
| **Authentication** | Verify identity |
| **Authorization** | Determine permissions |
| **Directory Services** | Store and manage identities |
| **Microsoft Entra ID** | Cloud identity and access management |
| **External Identities** | Access for outside users |

### Memory Trick

```text
Authentication      = Identity
Authorization       = Permissions
Directory Services  = Identity directory
Microsoft Entra ID  = Cloud identity management
External Identities = Outside users
```

---

# Choosing the Right Identity Concept

### Think Authentication when:
- A user needs to prove who they are.
- MFA, passwords, biometrics, or security keys are involved.

### Think Authorization when:
- The question is about permissions.
- An authenticated user needs access to a particular resource or action.

### Think Microsoft Entra ID when:
- The organization needs cloud identity management.
- Users need access to Microsoft 365, Azure, or enterprise applications.
- SSO or Conditional Access is discussed.

### Think External Identities when:
- Partners, vendors, contractors, or customers need controlled access.
- The user is outside the organization.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 13 Lab — Identity Foundations](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-13-Lab-13-Identity-Foundations.md)**

### Lab Focus

- Explore Microsoft Entra ID.
- Explore Users and Groups.
- Browse Enterprise Applications.
- Explore External Identities.
- Review Authentication Methods.
- Practice Authentication vs. Authorization scenarios.

> [!TIP]
> Microsoft Entra admin-center and Azure Portal exploration are kept in the separate lab.

---

# Quick Check

| Question | Answer |
|---|---|
| Proves who a user is | Authentication |
| Determines what a user can access | Authorization |
| Stores and manages identity information | Directory Services |
| Microsoft's cloud identity and access management service | Microsoft Entra ID |
| Provides controlled access for outside users | External Identities |

---

# Before Moving On

You should be able to:

- Explain Authentication.
- Explain Authorization.
- Explain the difference between Authentication and Authorization.
- Explain the purpose of Microsoft Entra ID.
- Explain Directory Services.
- Explain External Identities.
- Identify the correct identity concept from a basic scenario.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Authentication** | Who are you? |
| **Authorization** | What can you do? |
| **Directory Services** | Store and manage identities |
| **Microsoft Entra ID** | Cloud identity and access management |
| **External Identities** | Outside-user access |

> **Authenticate first, authorize second.**
