# Lesson 4 — Azure Architecture I

## 📖 Microsoft Learn

**Module:** Azure Architecture Fundamentals  
https://learn.microsoft.com/en-us/training/modules/azure-architecture-fundamentals/

### Focus
- Azure Regions
- Region Pairs
- Availability Zones
- Availability Sets

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Regions and Region Pairs | 13:08 | https://youtu.be/4RjPOAN54AE |
| Benefits and Usage of Availability Zones | 8:41 | https://youtu.be/h0enGb17lnw |

---

# Azure Infrastructure

Azure's global infrastructure is organized into geographic locations designed to support availability, resiliency, performance, disaster recovery, and data residency.

```text
Azure Geography
      │
      ├── Azure Region
      │      ├── Availability Zone 1
      │      ├── Availability Zone 2
      │      └── Availability Zone 3
      │
      └── Other Azure Regions
```

---

# Azure Regions

An **Azure Region** is a set of datacenters deployed within a latency-defined perimeter and connected through a dedicated regional low-latency network.

## Key Characteristics
- Contains one or more datacenters.
- Uses high-speed, low-latency networking.
- Regional Azure resources are deployed to a selected region.
- Service and feature availability can vary by region.
- Region choice can affect latency, availability, compliance, and cost.

### Real-World Thinking
A company may choose a region close to its users to reduce latency or select a particular geography to meet data-residency requirements.

### Exam Thinking
> **Azure Region = geographic area containing one or more Azure datacenters connected by a low-latency network.**

---

# Region Pairs

Azure regions may be associated with another region in the same geography to support resiliency and disaster-recovery planning.

## Key Features
- Regions are geographically separated.
- Pairing supports regional resiliency and geo-redundancy scenarios.
- Planned platform updates can be sequenced between paired regions.
- Recovery prioritization can take regional relationships into account.
- Regional relationships generally support geographic data-residency considerations.

### Real-World Thinking
If a major regional event affects one location, an organization can design workloads and replicated data to use another region as part of its disaster-recovery strategy.

### Exam Thinking
> **Region Pair = region-to-region resiliency and disaster-recovery planning.**

Think **Region ↔ Region**.

---

# Availability Zones

**Availability Zones** are physically separate locations within an Azure region with independent infrastructure such as:

- Power
- Cooling
- Networking

```text
              Azure Region
                   │
       ┌───────────┼───────────┐
       │           │           │
     Zone 1      Zone 2      Zone 3
       │           │           │
 Independent   Independent   Independent
 Power/Net     Power/Net     Power/Net
```

## Service Categories

### Zonal Services
Resources can be deployed into a specific Availability Zone.

Examples include virtual machines and managed disks.

### Zone-Redundant Services
Azure can distribute or replicate supported services across multiple Availability Zones.

### Non-Regional Services
Some Azure services operate globally rather than depending on a single region or zone.

### Real-World Thinking
An application can use multiple Availability Zones so a failure affecting one location inside the region does not necessarily take down the entire workload.

### Exam Thinking
> **Availability Zone = physically separate location inside an Azure Region.**

**Region = geographic area**  
**Availability Zone = isolated location inside the region**

---

# Availability Sets

**Availability Sets** are logical groupings that help protect virtual machines from hardware failures and planned maintenance.

They use:

- **Fault Domains**
- **Update Domains**

## Fault Domains
Separate VMs based on underlying hardware dependencies such as power and networking.

## Update Domains
Separate VMs into groups so planned maintenance and reboots do not affect every VM simultaneously.

### Real-World Thinking
If two VMs provide the same application, separating them across fault and update domains reduces the chance that the same hardware failure or maintenance event affects both.

### Exam Thinking
> **Availability Set = logical VM protection using fault domains and update domains.**

---

# Region Pairs vs. Availability Zones vs. Availability Sets

| Concept | Scope | Primary Purpose |
|---|---|---|
| **Region Pair** | Two Azure regions | Regional resiliency / disaster recovery |
| **Availability Zone** | Separate location inside one region | Datacenter-level fault isolation |
| **Availability Set** | Logical grouping of VMs | Hardware failure and planned-maintenance protection |

### Easy Way to Remember

```text
REGION PAIR
Region ↔ Region

AVAILABILITY ZONES
Zone 1 | Zone 2 | Zone 3
       inside
    ONE REGION

AVAILABILITY SET
VMs separated across
Fault + Update Domains
```

---

# Choosing the Right Architecture Concept

### Think Region Pair when:
- Planning for a regional outage.
- Designing cross-region disaster recovery.

### Think Availability Zone when:
- Protecting against a location/datacenter failure inside a region.
- Distributing supported resources across physically separate locations.

### Think Availability Set when:
- Protecting multiple VMs from shared hardware failures.
- Separating VMs during planned maintenance.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 04 Lab — Azure Architecture I](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-04-Lab-04-Azure-Architecture-I.md)**

### Lab Focus
- Explore Azure's global infrastructure.
- Locate Azure regions.
- Review Region Pair information.
- Identify Availability Zone support.
- Compare Regions, Region Pairs, Availability Zones, and Availability Sets.
- Practice AZ-900 architecture scenarios.

> [!TIP]
> No Azure resources need to be deployed for this lab.

---

# Quick Check

| Question | Answer |
|---|---|
| Geographic area containing Azure datacenters | Azure Region |
| Two associated Azure regions | Region Pair |
| Physically separate location inside a region | Availability Zone |
| Logical VM grouping using fault and update domains | Availability Set |
| Protect against a datacenter-level failure within a region | Availability Zones |
| Protect VMs from shared hardware/maintenance events | Availability Set |

---

# Before Moving On

You should be able to:
- Explain what an Azure Region is.
- Explain the purpose of Region Pairs.
- Explain Availability Zones.
- Explain Availability Sets.
- Compare Region Pairs vs. Availability Zones.
- Compare Availability Zones vs. Availability Sets.
- Identify the appropriate concept from a basic scenario.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Azure Region** | Geographic area containing Azure datacenters |
| **Region Pair** | Region-to-region resiliency |
| **Availability Zone** | Physically separate location within a region |
| **Availability Set** | Logical VM protection |
| **Fault Domain** | Protects against shared hardware failure |
| **Update Domain** | Protects during planned maintenance |
