# Lab 14 — Identity & Access

## Objective

This lab reinforces **Lesson 14 — Identity & Access**.

By the end, you should be able to:

- Explore Azure roles and role assignments.
- Identify RBAC Security Principals, Role Definitions, and Scope.
- Explore Conditional Access.
- Review authentication and MFA settings.
- Explore Enterprise Applications and Single Sign-On.
- Apply the Principle of Least Privilege to basic scenarios.
- Choose the correct identity and access feature for common AZ-900 scenarios.

---

## Prerequisites

- Completed **Lesson 14 — Identity & Access**
- Web browser
- Azure / Microsoft Entra account with appropriate read access

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **Microsoft Learn — Secure Azure Resources with RBAC:** https://learn.microsoft.com/en-us/training/modules/secure-your-azure-resources-with-rbac/
- **Assign Azure Roles Using the Azure Portal:** https://learn.microsoft.com/en-us/azure/role-based-access-control/role-assignments-portal

> [!IMPORTANT]
> Identity, RBAC, MFA, and Conditional Access changes can affect real users and administrators. Unless you are using a dedicated lab environment and have permission to make changes, **review the configuration screens without creating or changing assignments or policies**.

---

# Part 1 — Explore Azure Roles and Role Assignments

### Links

- **Azure RBAC Overview:** https://learn.microsoft.com/en-us/azure/role-based-access-control/overview
- **Azure Built-In Roles:** https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open the Azure Portal.
2. Open a safe subscription, Resource Group, or test resource.
3. Locate **Access control (IAM)**.
4. Review the available tabs and options.
5. Locate **Role assignments**.
6. Review existing assignments if your permissions allow it.
7. Do not add, remove, or modify role assignments in a production environment.

## Look For

- Role name
- Assigned identity
- Scope
- Assignment type

## Think About It

What is Azure RBAC used for?

**Answer:** _______________________________________________

Is Azure RBAC primarily authentication or authorization?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure RBAC = authorization for Azure resources.**

---

# Part 2 — Identify WHO, WHAT, and WHERE

Azure RBAC role assignments combine three important concepts:

```text
WHO   = Security Principal
WHAT  = Role Definition
WHERE = Scope
```

### Links

- **Understand Azure Role Definitions:** https://learn.microsoft.com/en-us/azure/role-based-access-control/role-definitions
- **Understand Scope for Azure RBAC:** https://learn.microsoft.com/en-us/azure/role-based-access-control/scope-overview

Complete the table:

| RBAC Component | Meaning |
|---|---|
| Security Principal | ______________________________ |
| Role Definition | ______________________________ |
| Scope | ______________________________ |

## Scenario

A user named Alex is assigned the **Reader** role on a Resource Group.

Identify:

**Security Principal:** ______________________________

**Role Definition:** ______________________________

**Scope:** ______________________________

---

# Part 3 — Compare Owner, Contributor, and Reader

### Links

- **Azure Built-In Roles:** https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles

Complete the table before checking the answer key.

| Role | View Resources | Manage Resources | Assign Azure Roles |
|---|:---:|:---:|:---:|
| **Owner** | ______ | ______ | ______ |
| **Contributor** | ______ | ______ | ______ |
| **Reader** | ______ | ______ | ______ |

## Least-Privilege Scenarios

### Scenario 1

A user only needs to view Azure resources.

**Best role:** ______________________________

### Scenario 2

A user needs to create and manage resources but should not assign Azure roles.

**Best role:** ______________________________

### Scenario 3

An administrator needs full resource management and the ability to assign Azure roles.

**Best role:** ______________________________

### Exam Thinking

```text
Owner       = Manage + assign access
Contributor = Manage
Reader      = View
```

---

# Part 4 — Explore Conditional Access

### Links

- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **Conditional Access Overview:** https://learn.microsoft.com/en-us/entra/identity/conditional-access/overview

## Steps

1. Open the Microsoft Entra admin center.
2. Locate **Conditional Access** if your account and tenant provide access.
3. Review existing policy names and configuration areas without changing anything.
4. Look for concepts involving:
   - Users or groups
   - Target resources
   - Conditions
   - Grant controls
5. Do not create, enable, disable, or modify Conditional Access policies.

> [!NOTE]
> Conditional Access availability and configuration access depend on the tenant, licensing, and your permissions. If you cannot view it, use the linked Microsoft documentation for this exercise.

## Think About It

What kind of logic does Conditional Access use?

**Answer:** _______________________________________________

Name one signal or condition that could influence an access decision.

**Answer:** _______________________________________________

Name one control a Conditional Access policy could require.

**Answer:** _______________________________________________

### Exam Thinking

> **Conditional Access = if-then access policy.**

---

# Part 5 — Review MFA and Authentication Methods

### Links

- **Microsoft Entra Authentication Methods:** https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-methods
- **Microsoft Entra Multifactor Authentication:** https://learn.microsoft.com/en-us/entra/identity/authentication/concept-mfa-howitworks
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. In the Microsoft Entra admin center, locate the authentication-method areas available to your account.
2. Review the supported authentication methods.
3. Do not enable, disable, or modify authentication policies.
4. Identify examples of the three factor categories.

Complete the table:

| Factor | Example |
|---|---|
| Something you know | __________________ |
| Something you have | __________________ |
| Something you are | __________________ |

## Think About It

Why does MFA provide stronger protection than a password alone?

**Answer:** _______________________________________________

### Exam Thinking

> **MFA = two or more authentication factors.**

---

# Part 6 — Explore Enterprise Applications and SSO

### Links

- **Microsoft Entra Admin Center:** https://entra.microsoft.com/
- **Single Sign-On Overview:** https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/what-is-single-sign-on
- **Enterprise Applications:** https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/what-is-enterprise-apps

## Steps

1. Locate **Enterprise applications**.
2. Open the application list if your permissions allow it.
3. Open a safe application only if appropriate.
4. Review the available **Single sign-on** area.
5. Do not change SSO configuration or user assignments.

## Think About It

What is the main benefit of SSO to a user?

**Answer:** _______________________________________________

Does SSO mean that every authenticated user automatically receives access to every application?

**Answer:** _______________________________________________

### Exam Thinking

> **SSO = sign in once and access multiple authorized applications.**

---

# Part 7 — RBAC vs. Conditional Access

Choose:

- **Azure RBAC**
- **Conditional Access**

### Scenario 1

A user needs Reader access to one Resource Group.

**Answer:** ______________________________

### Scenario 2

Administrators must complete MFA before accessing a cloud application.

**Answer:** ______________________________

### Scenario 3

A user needs permission to manage Azure virtual machines.

**Answer:** ______________________________

### Scenario 4

Access should be blocked when configured sign-in conditions are met.

**Answer:** ______________________________

### Memory Trick

```text
RBAC               = RESOURCE PERMISSIONS
Conditional Access = ACCESS CONDITIONS
```

---

# Part 8 — Identity & Access Scenarios

Choose from:

- **Microsoft Entra ID**
- **Azure RBAC**
- **Conditional Access**
- **MFA**
- **SSO**
- **Least Privilege**

### Scenario 1

A company needs Microsoft's cloud identity and access-management service.

**Answer:** ______________________________

### Scenario 2

An administrator needs to control who can manage an Azure Resource Group.

**Answer:** ______________________________

### Scenario 3

An organization requires additional verification when configured sign-in conditions are met.

**Answer:** ______________________________

### Scenario 4

A user enters a password and then completes another authentication factor.

**Answer:** ______________________________

### Scenario 5

Employees should authenticate once and then open multiple authorized business applications.

**Answer:** ______________________________

### Scenario 6

A help-desk employee only needs permission to view a particular Azure resource.

**Answer:** ______________________________

---

# Part 9 — Exam Review

Complete the table:

| Question | Answer |
|---|---|
| Who receives an RBAC assignment? | __________________ |
| What permissions are allowed? | __________________ |
| Where does the assignment apply? | __________________ |
| Which role can view but not modify? | __________________ |
| Which role can manage resources but not assign Azure roles? | __________________ |
| Which role can manage resources and assign Azure roles? | __________________ |
| Which feature uses condition-based access rules? | __________________ |
| Which feature uses multiple authentication factors? | __________________ |
| Which feature reduces repeated application sign-ins? | __________________ |

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

Azure RBAC controls authorization to Azure resources.

## Part 2

| Component | Meaning |
|---|---|
| Security Principal | Who receives access |
| Role Definition | What permissions are allowed |
| Scope | Where the permissions apply |

For Alex:

- **Security Principal:** Alex
- **Role Definition:** Reader
- **Scope:** Resource Group

## Part 3

| Role | View | Manage | Assign Azure Roles |
|---|:---:|:---:|:---:|
| Owner | Yes | Yes | Yes |
| Contributor | Yes | Yes | No |
| Reader | Yes | No | No |

Scenarios:

1. **Reader**
2. **Contributor**
3. **Owner**

## Part 4

Conditional Access uses if-then policy logic. Signals can include user, group, device, location, application, or risk information. A policy can require controls such as MFA or a compliant device, or it can block access.

## Part 5

| Factor | Example |
|---|---|
| Something you know | Password or PIN |
| Something you have | Phone, authenticator, or security key |
| Something you are | Fingerprint or facial recognition |

MFA provides stronger protection because compromising one factor alone may not be enough to authenticate.

## Part 6

SSO reduces repeated sign-ins. It does **not** automatically authorize every user to every application.

## Part 7

| Scenario | Answer |
|---|---|
| 1 | Azure RBAC |
| 2 | Conditional Access |
| 3 | Azure RBAC |
| 4 | Conditional Access |

## Part 8

| Scenario | Answer |
|---|---|
| 1 | Microsoft Entra ID |
| 2 | Azure RBAC |
| 3 | Conditional Access |
| 4 | MFA |
| 5 | SSO |
| 6 | Least Privilege |

## Part 9

| Question | Answer |
|---|---|
| Who receives an RBAC assignment? | Security Principal |
| What permissions are allowed? | Role Definition |
| Where does the assignment apply? | Scope |
| View but not modify | Reader |
| Manage resources but not assign Azure roles | Contributor |
| Manage resources and assign Azure roles | Owner |
| Condition-based access rules | Conditional Access |
| Multiple authentication factors | MFA |
| Reduces repeated sign-ins | SSO |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Microsoft Entra ID.
- Azure RBAC.
- Security Principal, Role Definition, and Scope.
- Owner vs. Contributor vs. Reader.
- Conditional Access.
- MFA.
- SSO.
- Least Privilege.
- RBAC vs. Conditional Access.
- Which identity and access feature best fits a basic AZ-900 scenario.
