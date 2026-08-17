# Lab 13 — Identity Foundations

## Objective

This lab reinforces **Lesson 13 — Identity Foundations**.

By the end, you should be able to:

- Navigate Microsoft Entra ID.
- Explore Users and Groups.
- Explore Enterprise Applications.
- Explore External Identities.
- Review Authentication Methods.
- Distinguish Authentication from Authorization.
- Identify the correct identity concept for common AZ-900 scenarios.

---

## Prerequisites

- Completed **Lesson 13 — Identity Foundations**
- Web browser
- Microsoft account with access to an Azure / Microsoft Entra tenant

### Start Here

- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **Azure Portal:** https://portal.azure.com/
- **Microsoft Entra ID Documentation:** https://learn.microsoft.com/en-us/entra/fundamentals/whatis

> [!IMPORTANT]
> This is an exploration lab. Do **not** create, delete, invite, disable, or modify users, groups, authentication methods, applications, or security settings in a production tenant.

---

# Part 1 — Explore Microsoft Entra ID

### Links

- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **What is Microsoft Entra ID?:** https://learn.microsoft.com/en-us/entra/fundamentals/whatis

## Steps

1. Open the **Microsoft Entra admin center**.
2. Sign in with an account that has appropriate access.
3. Locate **Microsoft Entra ID**.
4. Review the tenant overview.
5. Look for navigation areas involving:
   - Users
   - Groups
   - Enterprise applications
   - External identities
   - Authentication methods
6. Do not change any tenant settings.

## Think About It

What is the primary purpose of Microsoft Entra ID?

**Answer:** _______________________________________________

Is Microsoft Entra ID primarily a cloud identity service or a compute service?

**Answer:** _______________________________________________

### Exam Thinking

> **Microsoft Entra ID = cloud identity and access management.**

---

# Part 2 — Explore Users

### Links

- **Microsoft Entra Users:** https://learn.microsoft.com/en-us/entra/fundamentals/how-to-manage-user-profile-info
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. In the Microsoft Entra admin center, locate **Users**.
2. Open **All users** if your permissions allow it.
3. Review the types of information shown for user accounts.
4. Open a safe account only if appropriate.
5. Review the available account information without making changes.
6. Do not create, delete, disable, or modify users.

## Think About It

Why would an organization manage users centrally in a directory?

**Answer:** _______________________________________________

What type of identity information can a directory associate with a user?

**Answer:** _______________________________________________

---

# Part 3 — Explore Groups

### Links

- **Microsoft Entra Groups:** https://learn.microsoft.com/en-us/entra/fundamentals/concept-learn-about-groups
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. Locate **Groups**.
2. Open **All groups** if available.
3. Review existing group names and types.
4. Do not modify group membership.
5. Think about why assigning access to a group can be easier than managing every user separately.

## Think About It

Why are groups useful for access management?

**Answer:** _______________________________________________

Would it usually be easier to assign the same access to 50 users individually or through an appropriate group?

**Answer:** _______________________________________________

---

# Part 4 — Explore Enterprise Applications

### Links

- **Enterprise Applications:** https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/what-is-enterprise-apps
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. Locate **Enterprise applications**.
2. Review the application list if your permissions allow it.
3. Do not change assignments or application settings.
4. Review Microsoft's Enterprise Applications documentation.
5. Look for concepts involving:
   - Application access
   - User assignments
   - Single Sign-On

## Think About It

How can Microsoft Entra ID help users access cloud applications?

**Answer:** _______________________________________________

What does **Single Sign-On (SSO)** help reduce?

**Answer:** _______________________________________________

---

# Part 5 — Explore External Identities

### Links

- **Microsoft Entra External ID Overview:** https://learn.microsoft.com/en-us/entra/external-id/external-identities-overview
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. Locate **External Identities**.
2. Review the available options without making changes.
3. Review Microsoft's External ID documentation.
4. Think about users such as:
   - Partners
   - Vendors
   - Contractors
   - Customers

## Think About It

Why might a company need External Identities?

**Answer:** _______________________________________________

Should an external contractor automatically receive all the same access as an internal employee?

**Answer:** _______________________________________________

### Exam Thinking

> **External Identities = controlled access for outside users.**

---

# Part 6 — Explore Authentication Methods

### Links

- **Authentication Methods:** https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-methods
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. Locate the **Authentication methods** area.
2. Review the available authentication-method information.
3. Do not enable, disable, or change authentication policies.
4. Review Microsoft's authentication-method documentation.
5. Identify examples such as:
   - Password
   - Microsoft Authenticator
   - Security keys
   - Other supported methods

## Think About It

What question does authentication answer?

**Answer:** _______________________________________________

Why can using more than one authentication factor improve account security?

**Answer:** _______________________________________________

### Exam Thinking

> **Authentication = Who are you?**

---

# Part 7 — Authentication vs. Authorization

For each scenario, choose:

- **Authentication**
- **Authorization**

### Scenario 1

A user enters a password to prove their identity.

**Answer:** ______________________________

### Scenario 2

Azure checks whether a user has permission to view a resource.

**Answer:** ______________________________

### Scenario 3

A user approves an MFA request during sign-in.

**Answer:** ______________________________

### Scenario 4

An administrator assigns permissions that allow a user to manage a resource.

**Answer:** ______________________________

### Scenario 5

A security key is used during sign-in.

**Answer:** ______________________________

### Scenario 6

An authenticated user is denied access because they do not have the required permission.

**Answer:** ______________________________

### Memory Trick

```text
Authentication = WHO ARE YOU?
Authorization  = WHAT CAN YOU DO?
```

---

# Part 8 — Identity Scenarios

Choose from:

- **Authentication**
- **Authorization**
- **Directory Services**
- **Microsoft Entra ID**
- **External Identities**

### Scenario 1

A company needs a centralized system to store and manage user and group identities.

**Answer:** ______________________________

### Scenario 2

An employee must prove their identity before signing in.

**Answer:** ______________________________

### Scenario 3

A signed-in employee needs permission to administer a resource.

**Answer:** ______________________________

### Scenario 4

An organization needs Microsoft's cloud identity and access-management service for users and applications.

**Answer:** ______________________________

### Scenario 5

A vendor needs controlled access to a company application.

**Answer:** ______________________________

---

# Part 9 — Office Building Review

Match the office-building example to the identity concept.

| Office Example | Identity Concept |
|---|---|
| Show your badge at the entrance | __________________ |
| Badge determines which rooms you can enter | __________________ |
| Employee directory stores your identity | __________________ |
| Contractor receives controlled guest access | __________________ |

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

Microsoft Entra ID provides cloud identity and access management.

## Part 2

Centralized user management helps organizations manage identities consistently instead of maintaining separate accounts independently for every service.

## Part 3

Groups can simplify access management by allowing appropriate permissions or assignments to be managed for a collection of users.

## Part 4

Microsoft Entra ID can help control access to enterprise applications and support Single Sign-On. SSO reduces the need for users to repeatedly authenticate separately to multiple applications.

## Part 5

External Identities allow organizations to provide controlled access to people outside the organization. External users should receive only the access they require.

## Part 6

Authentication answers **Who are you?** Multiple factors can make it more difficult for an attacker to gain access using only one compromised credential.

## Part 7

| Scenario | Answer |
|---|---|
| 1 | Authentication |
| 2 | Authorization |
| 3 | Authentication |
| 4 | Authorization |
| 5 | Authentication |
| 6 | Authorization |

## Part 8

| Scenario | Answer |
|---|---|
| 1 | Directory Services |
| 2 | Authentication |
| 3 | Authorization |
| 4 | Microsoft Entra ID |
| 5 | External Identities |

## Part 9

| Office Example | Answer |
|---|---|
| Show your badge | Authentication |
| Badge determines rooms | Authorization |
| Employee directory | Directory Services |
| Contractor guest access | External Identities |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Authentication.
- Authorization.
- Authentication vs. Authorization.
- Directory Services.
- Microsoft Entra ID.
- External Identities.
- Users and Groups.
- Enterprise Applications.
- Authentication Methods.
- Which identity concept best fits a basic AZ-900 scenario.
