# Lab 09 — Networking

## Objective

This lab reinforces **Lesson 9 — Networking**.

By the end, you should be able to:

- Explore the creation of an Azure Virtual Network.
- Identify subnets inside a VNet.
- Explore Network Security Groups.
- Explore Public IP Addresses.
- Explore Azure DNS.
- Compare Public and Private Endpoints.
- Identify the correct Azure networking concept for common scenarios.

---

## Prerequisites

- Completed **Lesson 9 — Networking**
- Web browser
- Azure account if completing resource-creation activities

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Azure Networking Fundamentals:** https://learn.microsoft.com/en-us/training/modules/azure-networking-fundamentals/
- **Create a Virtual Network:** https://learn.microsoft.com/en-us/azure/virtual-network/quick-create-portal

> [!IMPORTANT]
> You do not need to create every resource shown in this lab. Portal exploration and reviewing configuration screens are enough for AZ-900 practice unless you intentionally want to deploy resources.

---

# Part 1 — Explore a Virtual Network

### Links

- **Azure Portal:** https://portal.azure.com/
- **Create a Virtual Network:** https://learn.microsoft.com/en-us/azure/virtual-network/quick-create-portal
- **Virtual Network Documentation:** https://learn.microsoft.com/en-us/azure/virtual-network/

## Steps

1. Open Microsoft's **Create a Virtual Network** quickstart.
2. Open the Azure Portal.
3. Search for **Virtual networks**.
4. Select **Create**.
5. Review the configuration options.
6. Pay attention to:
   - Subscription
   - Resource Group
   - VNet name
   - Region
   - IP address space
   - Subnets
7. Follow Microsoft's current quickstart if you want to create the VNet.
8. Otherwise, stop before deployment.

## Think About It

What is the primary purpose of a VNet?

**Answer:** _______________________________________________

Can one VNet contain multiple subnets?

**Answer:** _______________________________________________

### Exam Thinking

> **VNet = Azure's private network.**

---

# Part 2 — Explore Subnets

### Links

- **Azure Portal:** https://portal.azure.com/
- **Virtual Network Documentation:** https://learn.microsoft.com/en-us/azure/virtual-network/virtual-networks-overview

## Steps

1. Open an existing test VNet, or review the VNet creation screens.
2. Locate **Subnets**.
3. Review the subnet names and address ranges.
4. If using the creation wizard, review how a subnet is defined inside the VNet.
5. Do not change business or production networks.

## Think About It

Why might an organization separate resources into multiple subnets?

**Answer:** _______________________________________________

Is a subnet larger than the VNet containing it?

**Answer:** _______________________________________________

### Exam Thinking

> **Subnet = smaller network inside a VNet.**

---

# Part 3 — Explore Network Security Groups

### Links

- **Azure Portal:** https://portal.azure.com/
- **NSG Overview:** https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview

## Steps

1. Search the Azure Portal for **Network security groups**.
2. Open an existing safe test NSG if available.
3. Otherwise, select **Create** only to review the initial options.
4. Review **Inbound security rules** and **Outbound security rules** if available.
5. Look for:
   - Priority
   - Source
   - Destination
   - Port
   - Protocol
   - Allow or Deny
6. Do not change security rules on production resources.

## Think About It

Which rule is evaluated first: priority 100 or priority 500?

**Answer:** _______________________________________________

What is the purpose of an NSG?

**Answer:** _______________________________________________

Where can an NSG be associated?

**Answer:** _______________________________________________

### Exam Thinking

> **NSG = filters inbound and outbound network traffic.**

---

# Part 4 — Explore Public IP Addresses

### Links

- **Azure Portal:** https://portal.azure.com/
- **Public IP Addresses:** https://learn.microsoft.com/en-us/azure/virtual-network/ip-services/public-ip-addresses

## Steps

1. Search the Azure Portal for **Public IP addresses**.
2. Open the service.
3. Review any existing test resources or select **Create** to review the options.
4. Do not deploy a Public IP unless needed for a safe lab environment.
5. Review Microsoft's Public IP documentation.

## Think About It

What makes a Public IP different from a private IP?

**Answer:** _______________________________________________

Why might an Azure resource need a Public IP?

**Answer:** _______________________________________________

### Exam Thinking

> **Public IP Address = internet-routable address.**

---

# Part 5 — Explore Azure DNS

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure DNS Overview:** https://learn.microsoft.com/en-us/azure/dns/dns-overview

## Steps

1. Search the Azure Portal for **DNS zones**.
2. Open the service.
3. Review the creation screen or an existing safe test DNS zone.
4. Review Microsoft's Azure DNS overview.
5. Look for examples of DNS records.

## Think About It

What problem does DNS solve?

**Answer:** _______________________________________________

What does DNS translate a domain name into?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure DNS = name-to-IP resolution.**

---

# Part 6 — Public vs. Private Endpoints

### Links

- **Private Endpoint Overview:** https://learn.microsoft.com/en-us/azure/private-link/private-endpoint-overview
- **Azure Private Link Overview:** https://learn.microsoft.com/en-us/azure/private-link/private-link-overview

Review the documentation and compare the two access models.

## Public Endpoint

A public endpoint provides a publicly reachable network path to a service.

## Private Endpoint

A private endpoint uses a private IP address from a VNet to provide private connectivity to a supported Azure service.

## Complete the Comparison

| Question | Public Endpoint | Private Endpoint |
|---|---|---|
| Uses a public network path? | __________ | __________ |
| Uses a private IP in a VNet? | __________ | __________ |
| Reduces public network exposure? | __________ | __________ |

### Exam Thinking

```text
Public Endpoint  = Public access path
Private Endpoint = Private VNet access
```

---

# Part 7 — Networking Scenarios

Choose:

- **Virtual Network**
- **Subnet**
- **Network Security Group**
- **Public Endpoint**
- **Private Endpoint**
- **Azure DNS**
- **Public IP Address**

### Scenario 1

A company needs a private Azure network for its cloud resources.

**Answer:** ______________________________

### Scenario 2

An administrator wants to divide a VNet into smaller network segments.

**Answer:** ______________________________

### Scenario 3

Inbound traffic should be allowed or denied based on ports and source addresses.

**Answer:** ______________________________

### Scenario 4

An Azure service should be reachable privately from a VNet instead of through a public network path.

**Answer:** ______________________________

### Scenario 5

A public-facing Azure resource needs an internet-routable address.

**Answer:** ______________________________

### Scenario 6

An organization needs to translate a domain name into an IP address.

**Answer:** ______________________________

### Scenario 7

An Azure service is intentionally reachable through a public network path.

**Answer:** ______________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1
A VNet provides a private network in Azure. One VNet can contain multiple subnets.

## Part 2
Subnets divide a VNet into smaller network segments. A subnet exists inside the VNet.

## Part 3
Priority **100** is evaluated before priority **500** because lower numbers are processed first.

NSGs filter inbound and outbound traffic using security rules and can be associated with supported subnet and network-interface scopes.

## Part 4
A Public IP is internet-routable and can allow Azure resources to communicate over public networks.

## Part 5
DNS translates names into IP addresses.

## Part 6

| Question | Public Endpoint | Private Endpoint |
|---|---|---|
| Uses a public network path? | Yes | No |
| Uses a private IP in a VNet? | No | Yes |
| Reduces public network exposure? | No | Yes |

## Part 7

| Scenario | Answer |
|---|---|
| 1 | Virtual Network |
| 2 | Subnet |
| 3 | Network Security Group |
| 4 | Private Endpoint |
| 5 | Public IP Address |
| 6 | Azure DNS |
| 7 | Public Endpoint |

</details>

---

# Lab Cleanup

If you created a VNet or other test resources during this lab, remove them when finished unless you intentionally want to keep them.

### Links

- **Manage Resource Groups:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal
- **Azure Portal:** https://portal.azure.com/

> [!CAUTION]
> Verify that a Resource Group contains only lab resources before deleting it. Deleting a Resource Group deletes everything inside it.

---

# Lab Complete

Before moving on, make sure you can explain:

- VNet vs. Subnet.
- NSG purpose and rule priority.
- Public Endpoint vs. Private Endpoint.
- Public IP Address vs. Private Endpoint.
- Azure DNS.
- Which networking concept best fits a basic AZ-900 scenario.
