# Lab 19 — Security II

## Objective

This lab reinforces **Lesson 19 — Security II**.

By the end, you should be able to:

- Create and explore a Network Security Group.
- Review default inbound and outbound NSG rules.
- Create and remove a temporary security rule.
- Browse Azure Firewall.
- Review Azure DDoS Protection.
- Explore Azure Key Vault.
- Explore Microsoft Sentinel.
- Review Azure Dedicated Hosts.
- Match common security requirements to the correct Azure service.

---

# Prerequisites

- Completed **Lesson 19 — Security II**
- Web browser
- Azure account with permission to create and delete a test NSG

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Network Security Groups:** https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview
- **Azure Firewall:** https://learn.microsoft.com/en-us/azure/firewall/overview
- **Azure DDoS Protection:** https://learn.microsoft.com/en-us/azure/ddos-protection/ddos-protection-overview
- **Azure Key Vault:** https://learn.microsoft.com/en-us/azure/key-vault/general/overview
- **Microsoft Sentinel:** https://learn.microsoft.com/en-us/azure/sentinel/overview
- **Azure Dedicated Hosts:** https://learn.microsoft.com/en-us/azure/virtual-machines/dedicated-hosts

> [!IMPORTANT]
> Some Azure security services can create significant charges. **Do not deploy Azure Firewall, enable paid DDoS protection, enable Microsoft Sentinel, purchase Dedicated Host capacity, or create paid security services simply to complete this lab.** Those sections are exploration and documentation exercises.

---

# Part 1 — Create a Test Network Security Group

### Links

- **Azure Portal:** https://portal.azure.com/
- **Create or Manage an NSG:** https://learn.microsoft.com/en-us/azure/virtual-network/manage-network-security-group

## Steps

1. Open the Azure Portal.
2. Search for **Network security groups**.
3. Select **Create**.
4. Choose an appropriate lab subscription.
5. Select or create a temporary lab Resource Group.
6. Enter a name such as:

```text
az900-lab19-nsg
```

7. Select an Azure region.
8. Review the configuration.
9. Select **Review + create**.
10. Create the NSG.

> [!TIP]
> An NSG by itself does not need a virtual machine for this exercise. The goal is to learn how its security rules are organized.

---

# Part 2 — Review Default Inbound Rules

## Steps

1. Open the NSG you created.
2. Select **Inbound security rules**.
3. Review the default inbound rules.
4. Notice the:
   - Priority
   - Name
   - Port
   - Protocol
   - Source
   - Destination
   - Action
5. Do not delete or modify the default rules.

## Questions

What direction do inbound rules control?

**Answer:** _______________________________________________

Are lower or higher NSG priority numbers evaluated first?

**Answer:** _______________________________________________

What happens when Azure finds a matching NSG rule?

**Answer:** _______________________________________________

---

# Part 3 — Review Default Outbound Rules

## Steps

1. Select **Outbound security rules**.
2. Review the default outbound rules.
3. Compare them with the inbound rules.

## Questions

What direction do outbound rules control?

**Answer:** _______________________________________________

Why might an organization restrict outbound traffic?

**Answer:** _______________________________________________

### Memory Trick

```text
Inbound  = IN
Outbound = OUT
```

---

# Part 4 — Create a Temporary Inbound Rule

> [!IMPORTANT]
> This rule is only for learning how NSG rules are configured. Do not attach this NSG to a production resource.

## Steps

1. Return to **Inbound security rules**.
2. Select **Add**.
3. Review the available fields.
4. Create a harmless temporary rule using values appropriate for your lab environment.

For example, you can create a rule that **denies** inbound TCP traffic on a test port:

```text
Source:              Any
Source port ranges:  *
Destination:         Any
Service:             Custom
Destination port:    65000
Protocol:            TCP
Action:              Deny
Priority:            300
Name:                AZ900-Lab-Test-Deny
```

5. Save the rule.
6. Verify that the new custom rule appears above the default rules based on priority.

## Questions

What does the **Priority** value control?

**Answer:** _______________________________________________

What does **Deny** mean?

**Answer:** _______________________________________________

Why is using an unused test port safer than opening a common administrative port for a learning exercise?

**Answer:** _______________________________________________

---

# Part 5 — Delete the Temporary Rule

## Steps

1. Select the temporary rule.
2. Delete it.
3. Confirm that it no longer appears in the NSG.

> [!IMPORTANT]
> Remove the temporary rule before continuing.

---

# Part 6 — Browse Azure Firewall

### Links

- **Azure Firewall Overview:** https://learn.microsoft.com/en-us/azure/firewall/overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Search the Azure Portal for **Firewalls** or **Azure Firewall**.
2. Browse the service page.
3. Review the creation options without deploying a firewall.
4. Read the Azure Firewall overview.
5. Close the creation screen without saving.

## Questions

What is Azure Firewall's primary purpose?

**Answer:** _______________________________________________

How is Azure Firewall different from an NSG?

**Answer:** _______________________________________________

> [!WARNING]
> Do not deploy Azure Firewall for this AZ-900 exercise. Azure Firewall is a billable service and is unnecessary for this introductory lab.

---

# Part 7 — Review Azure DDoS Protection

### Links

- **Azure DDoS Protection Overview:** https://learn.microsoft.com/en-us/azure/ddos-protection/ddos-protection-overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Review the Microsoft documentation for Azure DDoS Protection.
2. Search for DDoS-related options in the Azure Portal if available.
3. Review the service without enabling a paid plan.

## Questions

What type of attack does Azure DDoS Protection address?

**Answer:** _______________________________________________

How is DDoS Protection different from Azure Firewall?

**Answer:** _______________________________________________

### Exam Thinking

```text
Firewall = FILTER TRAFFIC
DDoS     = HANDLE TRAFFIC-FLOOD ATTACKS
```

---

# Part 8 — Browse Azure Key Vault

### Links

- **Azure Key Vault Overview:** https://learn.microsoft.com/en-us/azure/key-vault/general/overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Search for **Key vaults**.
2. Review any safe existing lab vault if available, or review the creation screen without creating one.
3. Look for areas involving:
   - Keys
   - Secrets
   - Certificates
4. Do not view, copy, modify, or expose real company secrets.

## Questions

Which three major types of sensitive items can Key Vault manage?

1. _______________________________________________
2. _______________________________________________
3. _______________________________________________

Where should an application store a database password instead of hardcoding it into source code?

**Answer:** _______________________________________________

### Exam Thinking

> **Key Vault = secrets + keys + certificates.**

---

# Part 9 — Encryption, Secrets, and Certificates

Choose:

- **Encryption**
- **Secret**
- **Certificate**

### Scenario 1

A database password must be stored securely.

**Answer:** ______________________________

### Scenario 2

Data should be unreadable if accessed without the correct key.

**Answer:** ______________________________

### Scenario 3

A website needs to establish trust and use HTTPS.

**Answer:** ______________________________

### Scenario 4

An application requires an API key.

**Answer:** ______________________________

### Scenario 5

Stored data is protected from unauthorized reading.

**Answer:** ______________________________

### Memory Trick

```text
Encryption   = PROTECT DATA
Secrets      = SENSITIVE VALUES
Certificates = ESTABLISH TRUST
```

---

# Part 10 — Browse Microsoft Sentinel

### Links

- **Microsoft Sentinel Overview:** https://learn.microsoft.com/en-us/azure/sentinel/overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Search for **Microsoft Sentinel**.
2. Open the service.
3. Review the available interface or onboarding information.
4. Read the Microsoft Sentinel overview.
5. Do not enable Sentinel or connect production data sources just for this lab.

## Look For

Concepts involving:

- Data connectors
- Analytics
- Incidents
- Hunting
- Automation

## Questions

What does **SIEM** stand for?

**Answer:** _______________________________________________

Why would an organization send security logs from many systems into Microsoft Sentinel?

**Answer:** _______________________________________________

### Exam Thinking

> **Sentinel = collect, detect, investigate, and respond.**

---

# Part 11 — Review Azure Dedicated Hosts

### Links

- **Azure Dedicated Hosts:** https://learn.microsoft.com/en-us/azure/virtual-machines/dedicated-hosts
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Read the Azure Dedicated Hosts overview.
2. Search the Azure Portal for **Dedicated hosts** if available.
3. Review the creation experience without deploying anything.
4. Close the creation screen without saving.

## Questions

What makes a Dedicated Host different from a standard Azure VM deployment?

**Answer:** _______________________________________________

Name one reason an organization might require a Dedicated Host.

**Answer:** _______________________________________________

> [!WARNING]
> Do not deploy a Dedicated Host simply for AZ-900 practice. Dedicated physical capacity can be expensive.

---

# Part 12 — Identity Protection Review

### Links

- **Microsoft Entra ID Protection:** https://learn.microsoft.com/en-us/entra/id-protection/overview-identity-protection
- **Microsoft Entra Admin Center:** https://entra.microsoft.com/

## Steps

1. Review the Microsoft Entra ID Protection documentation.
2. If your tenant and licensing allow it, browse the Identity Protection area in the Entra admin center.
3. Do not modify production risk policies.

## Questions

What type of risk does Identity Protection focus on?

**Answer:** _______________________________________________

Give one example of an identity-related risk it may help identify.

**Answer:** _______________________________________________

### Exam Thinking

> **Identity Protection = risky users and risky sign-ins.**

---

# Part 13 — Security Service Scenarios

Choose from:

- **Network Security Group**
- **Azure Firewall**
- **Azure DDoS Protection**
- **Azure Key Vault**
- **Microsoft Sentinel**
- **Azure Dedicated Host**
- **Microsoft Entra ID Protection**

### Scenario 1

An administrator needs allow and deny rules for inbound traffic to a subnet.

**Answer:** ______________________________

### Scenario 2

An organization needs centralized managed firewall protection for Azure networks.

**Answer:** ______________________________

### Scenario 3

A public application needs protection against large-scale traffic-flood attacks.

**Answer:** ______________________________

### Scenario 4

An application needs a secure location for an API key and database password.

**Answer:** ______________________________

### Scenario 5

A security operations team needs to collect and analyze security events from many systems.

**Answer:** ______________________________

### Scenario 6

A regulated workload requires Azure VMs to run on a physical server dedicated to one customer.

**Answer:** ______________________________

### Scenario 7

A security team needs to detect risky users and suspicious sign-ins.

**Answer:** ______________________________

---

# Part 14 — Clean Up

If you created the test NSG for this lab:

1. Verify the temporary custom rule has been deleted.
2. Return to the NSG overview.
3. Delete the test NSG if it is no longer needed.
4. If you created a temporary Resource Group only for this lab, delete it after confirming it contains nothing else you need.

> [!IMPORTANT]
> Never delete a Resource Group unless you have confirmed that every resource inside it is safe to remove.

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Parts 2–4

- Inbound rules control traffic coming into the protected resource.
- Outbound rules control traffic leaving it.
- Lower priority numbers are evaluated first.
- When a matching NSG rule is found, its allow or deny action is applied.
- Deny blocks matching traffic.

## Part 6

Azure Firewall is a centralized managed network firewall. NSGs provide allow/deny security rules for traffic associated with subnets and network interfaces.

## Part 7

Azure DDoS Protection addresses Distributed Denial-of-Service attacks. Firewall rules filter traffic; DDoS protection is focused on mitigating traffic-flood attacks.

## Part 8

Key Vault manages:

1. Secrets
2. Keys
3. Certificates

A database password should be stored as a protected secret rather than hardcoded into application source code.

## Part 9

| Scenario | Answer |
|---|---|
| 1 | Secret |
| 2 | Encryption |
| 3 | Certificate |
| 4 | Secret |
| 5 | Encryption |

## Part 10

SIEM stands for **Security Information and Event Management**. Centralizing security data allows a security team to correlate events and detect, investigate, and respond to threats.

## Part 11

A Dedicated Host provides physical server capacity dedicated to one Azure customer. Reasons can include physical isolation, compliance, licensing, or VM-placement requirements.

## Part 12

Identity Protection focuses on identity-based risks such as risky users and suspicious or risky sign-ins.

## Part 13

| Scenario | Answer |
|---|---|
| 1 | Network Security Group |
| 2 | Azure Firewall |
| 3 | Azure DDoS Protection |
| 4 | Azure Key Vault |
| 5 | Microsoft Sentinel |
| 6 | Azure Dedicated Host |
| 7 | Microsoft Entra ID Protection |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- NSGs and inbound/outbound rules.
- Azure Firewall.
- Azure DDoS Protection.
- Azure Key Vault.
- Encryption, secrets, and certificates.
- Microsoft Sentinel and SIEM.
- Azure Dedicated Hosts.
- Microsoft Entra ID Protection.
- Which Azure security service best fits a basic AZ-900 scenario.
