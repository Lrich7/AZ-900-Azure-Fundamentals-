
# Lab 04 — Azure Architecture I

## Objective

This lab reinforces **Lesson 4 — Azure Architecture I**.

By the end, you should be able to:
- Locate Azure regions.
- Explain the purpose of Region Pairs.
- Identify Availability Zone support.
- Compare an Azure Region with an Availability Zone.
- Distinguish Region Pairs, Availability Zones, and Availability Sets.

---

## Prerequisites

- Completed **Lesson 4 — Azure Architecture I**
- Web browser
- Azure account is optional

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Azure Architecture Fundamentals:** https://learn.microsoft.com/en-us/training/modules/azure-architecture-fundamentals/
- **Azure Global Infrastructure:** https://azure.microsoft.com/explore/global-infrastructure/
- **Azure Geographies:** https://azure.microsoft.com/explore/global-infrastructure/geographies/

> [!NOTE]
> No Azure resources need to be deployed.

---

# Part 1 — Explore Azure Regions

### Links
- **Azure Geographies:** https://azure.microsoft.com/explore/global-infrastructure/geographies/
- **Azure Global Infrastructure:** https://azure.microsoft.com/explore/global-infrastructure/
- **Azure Portal:** https://portal.azure.com/

## Steps
1. Open **Azure Geographies**.
2. Review Azure's geographic distribution.
3. Identify two Azure regions in the United States.
4. Find one region outside the United States.
5. Optionally open the Azure Portal and review the location choices for a regional resource without deploying it.

## Record What You Find

**U.S. Region 1:** ______________________________________

**U.S. Region 2:** ______________________________________

**Region outside the U.S.:** _____________________________

## Think About It

Why might an organization choose a region close to its users?

**Answer:** _______________________________________________

Why might an organization need a particular geography?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure Region = geographic area containing Azure datacenters connected by a low-latency network.**

---

# Part 2 — Explore Region Pairs

### Links
- **Cross-region replication in Azure:** https://learn.microsoft.com/en-us/azure/reliability/cross-region-replication-azure
- **Azure Reliability Documentation:** https://learn.microsoft.com/en-us/azure/reliability/

## Steps
1. Open the cross-region replication documentation.
2. Review Microsoft's information about paired regions and cross-region resiliency.
3. Look for regional relationship examples.
4. Consider why geographic separation is useful during a large-scale outage.

## Think About It

What type of failure is cross-region architecture designed to help address?

**Answer:** _______________________________________________

Is a Region Pair the same thing as two Availability Zones?

**Answer:** _______________________________________________

Why?

**Answer:** _______________________________________________

### Exam Thinking
> **Region Pair = Region ↔ Region**

Think **regional disaster recovery**.

---

# Part 3 — Explore Availability Zones

### Links
- **Availability Zones Overview:** https://learn.microsoft.com/en-us/azure/reliability/availability-zones-overview
- **Azure Global Infrastructure:** https://azure.microsoft.com/explore/global-infrastructure/

## Steps
1. Open the Availability Zones overview.
2. Review how Microsoft defines Availability Zones.
3. Identify the independent infrastructure associated with a zone.
4. Review region and service Availability Zone support.
5. Compare an Availability Zone with an Azure Region.

## Record What You Find

Availability Zones have independent:

1. ______________________________________
2. ______________________________________
3. ______________________________________

## Think About It

Are Availability Zones located in different Azure regions?

**Answer:** _______________________________________________

What type of failure do Availability Zones help isolate?

**Answer:** _______________________________________________

### Exam Thinking
> **Availability Zone = physically separate location inside an Azure Region.**

---

# Part 4 — Explore Availability Sets

### Links
- **VM Availability Options:** https://learn.microsoft.com/en-us/azure/virtual-machines/availability
- **Availability Sets Overview:** https://learn.microsoft.com/en-us/azure/virtual-machines/availability-set-overview

## Steps
1. Open the Availability Sets overview.
2. Find the definitions of **Fault Domain** and **Update Domain**.
3. Review how Availability Sets distribute VMs.
4. Compare this logical separation with Availability Zones.

## Record What You Find

**Fault Domain:** _________________________________________

**Update Domain:** ________________________________________

## Think About It

Which protects VMs from shared underlying hardware failures?

**Answer:** _______________________________________________

Which prevents planned maintenance from affecting every VM simultaneously?

**Answer:** _______________________________________________

### Exam Thinking
> **Availability Set = Fault Domains + Update Domains**

---

# Part 5 — Compare the Concepts

Complete the table before checking the answer key.

| Scenario | Architecture Concept |
|---|---|
| Geographic location where Azure resources are deployed | __________________ |
| Two geographically separated Azure regions | __________________ |
| Separate locations within one Azure region | __________________ |
| Logical VM protection using fault and update domains | __________________ |
| Protect against a regional disaster | __________________ |
| Protect against a location failure within a region | __________________ |

---

# Part 6 — Real-World Scenarios

Choose **Azure Region, Region Pair, Availability Zone, or Availability Set**.

### Scenario 1
Resources need to be distributed across physically separate locations inside the same Azure region.

**Answer:** ______________________________

### Scenario 2
A company is designing disaster recovery in case an entire Azure region becomes unavailable.

**Answer:** ______________________________

### Scenario 3
Two VMs should be separated so one hardware failure or maintenance event is less likely to affect both.

**Answer:** ______________________________

### Scenario 4
A company wants its application geographically close to most of its customers.

**Answer:** ______________________________

---

# Part 7 — Exam Thinking

1. **Azure Region** = ______________________________________
2. **Region Pair** = _______________________________________
3. **Availability Zone** = _________________________________
4. **Availability Set** = __________________________________
5. **Fault Domain** = ______________________________________
6. **Update Domain** = _____________________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Availability Zones
Independent infrastructure includes:
- Power
- Cooling
- Networking

Availability Zones are **inside an Azure region** and help isolate location/datacenter-level failures.

## Availability Sets
- **Fault Domain:** Helps isolate VMs from shared hardware failures.
- **Update Domain:** Helps prevent planned maintenance from affecting all VMs simultaneously.

## Compare the Concepts

| Scenario | Answer |
|---|---|
| Geographic location where Azure resources are deployed | Azure Region |
| Two geographically separated Azure regions | Region Pair |
| Separate locations within one Azure region | Availability Zone |
| Logical VM protection using fault and update domains | Availability Set |
| Protect against a regional disaster | Region Pair |
| Protect against a location failure within a region | Availability Zone |

## Real-World Scenarios

| Scenario | Answer |
|---|---|
| 1 | Availability Zone |
| 2 | Region Pair |
| 3 | Availability Set |
| 4 | Azure Region |

## Exam Thinking
- **Azure Region:** Geographic area containing Azure datacenters.
- **Region Pair:** Region-to-region resiliency.
- **Availability Zone:** Physically separate location within an Azure region.
- **Availability Set:** Logical VM grouping using fault and update domains.
- **Fault Domain:** Protects against shared hardware failures.
- **Update Domain:** Protects during planned maintenance.

</details>

---

# Lab Complete

Before moving on, make sure you can explain:
- Region vs. Availability Zone.
- Region Pair vs. Availability Zone.
- Availability Zone vs. Availability Set.
- Fault Domain vs. Update Domain.
- Which concept fits a basic availability or disaster-recovery scenario.
