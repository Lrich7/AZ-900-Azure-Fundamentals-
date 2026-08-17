# Lesson 20 — Pricing & Support

## 📖 Microsoft Learn

**Module:** Describe Azure Cost Management and Service Level Agreements (SLAs)  
https://learn.microsoft.com/en-us/training/modules/describe-azure-cost-management-service-level-agreements/

### Focus
- Factors That Affect Azure Costs
- Cost Optimization
- Azure Pricing Calculator
- Total Cost of Ownership (TCO) Calculator
- Azure Cost Management
- Service Level Agreements (SLAs)
- Azure Marketplace
- Azure Support Plans
- Azure Service Lifecycle
- Reservations
- Azure Spot Virtual Machines

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Factors That Affect Costs | 6:32 | https://youtu.be/fMShW_RGcxY |
| Factors to Reduce Cost | 15:29 | https://youtu.be/B5yiKE2DLH8 |
| Functionality and Usage of Pricing and TCO Calculators | 7:26 | https://youtu.be/pE-bf8i5blU |

---

# Understanding Azure Costs

Azure generally uses a consumption-based model.

The amount an organization pays depends on what services it uses, how those services are configured, and how long or how heavily they are used.

```text
Azure Cost
   |
   +-- Resource Type
   +-- Usage
   +-- Region
   +-- Performance / Tier
   +-- Storage
   +-- Data Transfer
   +-- Purchasing Option
```

### Exam Thinking

> **Azure cost is affected by resource configuration, location, usage, and purchasing choices.**

---

# Factors That Affect Azure Costs

## Resource Type

Different Azure services have different pricing models.

Examples include:

- Virtual Machines
- Storage Accounts
- Databases
- Networking services
- App hosting services

A small Storage Account and a powerful Virtual Machine do not have the same cost structure.

---

## Resource Usage

Many Azure resources are billed according to how much they are used.

Examples can include:

- Compute time
- Storage capacity
- Transactions
- Network usage

### Exam Thinking

> **More consumption can result in higher cost.**

---

## Azure Region

The same Azure service may have different prices in different Azure regions.

Region selection can therefore affect:

- Cost
- Latency
- Service availability
- Compliance and data residency

### Exam Thinking

> **Region can affect Azure pricing.**

---

## Performance Tier and Resource Size

Higher-performance resources generally cost more.

For example, a larger VM with more:

- vCPUs
- Memory
- Storage
- Performance

will generally cost more than a smaller VM.

---

## Usage Duration

A resource that runs continuously will generally cost more than one that only runs when needed.

This is especially important for compute resources.

### Real-World Thinking

A development VM does not necessarily need to run 24 hours per day.

Shutting it down when it is not needed can reduce cost.

---

## Data Transfer

Network data transfer can affect cost.

In particular, **outbound data transfer** from Azure can create charges depending on the service and destination.

### Exam Thinking

> **Outbound data transfer is a common Azure cost factor.**

---

# Cost Optimization

Cost optimization means getting the required business value while avoiding unnecessary cloud spending.

Common approaches include:

- Right-sizing resources.
- Removing unused resources.
- Shutting down resources when they are not needed.
- Using appropriate service tiers.
- Using Reservations for predictable long-term workloads.
- Using Spot VMs for interruptible workloads.
- Monitoring spending with Azure Cost Management.
- Using budgets and alerts.

### Memory Trick

```text
USE LESS
SIZE RIGHT
COMMIT WHEN PREDICTABLE
MONITOR COSTS
```

---

# Azure Pricing Calculator

The **Azure Pricing Calculator** is a Microsoft tool used to estimate the cost of Azure services before deployment.

**Calculator:**  
https://azure.microsoft.com/en-us/pricing/calculator/

It can help estimate resources such as:

- Virtual Machines
- Storage
- Databases
- Networking
- Many other Azure services

## Typical Process

```text
Choose Azure Service
        |
        v
Configure Options
        |
        v
Select Region / Tier / Usage
        |
        v
Review Estimated Cost
```

### What Can Affect the Estimate?

Depending on the service, options can include:

- Region
- Operating system
- VM size
- Hours of use
- Storage type
- Capacity
- Pricing model
- Reservation or savings options

### Exam Thinking

> **Pricing Calculator = estimate the cost of Azure resources before deployment.**

---

# Total Cost of Ownership (TCO) Calculator

The **Total Cost of Ownership (TCO) Calculator** is used to compare the cost of an existing on-premises environment with the estimated cost of running comparable workloads in Azure.

**Calculator:**  
https://azure.microsoft.com/en-us/pricing/tco/calculator/

The comparison can consider items such as:

- Servers
- Databases
- Storage
- Networking
- Electricity
- IT labor
- Hardware costs

### Real-World Thinking

A company wants to know whether moving its existing datacenter workloads to Azure could reduce overall infrastructure costs.

The TCO Calculator is designed for that type of comparison.

### Exam Thinking

> **TCO Calculator = compare on-premises costs with Azure.**

---

# Pricing Calculator vs. TCO Calculator

This distinction is important.

| Tool | Main Question |
|---|---|
| **Pricing Calculator** | What might these Azure resources cost? |
| **TCO Calculator** | How might Azure compare with our existing on-premises environment? |

### Memory Trick

```text
Pricing Calculator = AZURE PRICE
TCO Calculator     = ON-PREM vs. AZURE
```

---

# Azure Cost Management

**Azure Cost Management** helps organizations monitor, analyze, manage, and optimize Azure spending.

Capabilities can include:

- Cost analysis
- Budgets
- Alerts
- Cost allocation
- Recommendations and optimization workflows

### Real-World Thinking

The Pricing Calculator is useful **before** deployment.

Azure Cost Management becomes especially useful when resources are already running and an organization needs to understand actual spending.

### Exam Thinking

> **Azure Cost Management = monitor and optimize cloud spending.**

---

# Azure Budgets

Budgets help organizations track spending against a defined amount.

Alerts can notify appropriate users when configured thresholds are reached.

### Important

A budget is primarily a **monitoring and notification tool**.

Reaching a budget threshold does not automatically mean Azure will shut down all resources.

### Exam Thinking

> **Budget = track spending and alert when thresholds are reached.**

---

# Azure Reservations

**Azure Reservations** can reduce costs for supported services when an organization commits to eligible resource usage for a longer period.

Common commitment periods include:

- 1 year
- 3 years

Reservations are useful when workloads are:

- Predictable
- Long-running
- Expected to remain in use

### Important

A reservation primarily changes **billing**, not the way the workload itself operates.

### Exam Thinking

> **Reservation = commit to eligible long-term usage for a discount.**

---

# Pay-As-You-Go vs. Reservations

| Option | Best Fit |
|---|---|
| **Pay-As-You-Go** | Flexible or unpredictable workloads |
| **Reservation** | Predictable long-term workloads |

### Memory Trick

```text
Pay-As-You-Go = FLEXIBILITY
Reservation   = COMMITMENT + SAVINGS
```

---

# Azure Spot Virtual Machines

**Azure Spot Virtual Machines** use unused Azure compute capacity at a discounted price.

The tradeoff is that Azure can **evict** the VM when Azure needs the capacity back or when other configured conditions are met.

Because of this, Spot VMs are best suited for workloads that can tolerate interruption.

## Good Use Cases

Examples include:

- Batch processing
- Dev/test workloads
- Large compute jobs
- Rendering
- Some analytics workloads

## Poor Use Cases

Spot VMs are generally not appropriate for critical workloads that require guaranteed continuous availability.

### Exam Thinking

> **Spot VM = lower-cost compute that can be interrupted or evicted.**

---

# Reservations vs. Spot VMs

| Option | Main Benefit | Tradeoff |
|---|---|---|
| **Reservation** | Discount for predictable long-term usage | Commitment |
| **Spot VM** | Deeply discounted unused capacity | Can be evicted |

### Easy Way to Remember

```text
Reservation = COMMIT
Spot VM     = INTERRUPTIBLE
```

---

# Service Level Agreements (SLAs)

A **Service Level Agreement (SLA)** describes Microsoft's commitments for the availability and connectivity of Azure services.

SLAs can define:

- Availability targets
- Conditions
- Exclusions
- Service-credit eligibility

### Exam Thinking

> **SLA = Microsoft's service availability commitment.**

---

# SLA Availability Percentages

Higher availability percentages allow less downtime.

For example:

```text
99%
99.9%
99.95%
99.99%
99.999%
```

As the number of 9s increases, expected availability increases and allowable downtime decreases.

> [!NOTE]
> Exact SLA percentages and terms vary by Azure service and configuration. For AZ-900, understand the concept rather than memorizing every product's current SLA.

---

# Composite SLAs

Applications often depend on multiple services.

When multiple dependent services are required for the application to function, the application's combined or **composite SLA** can be lower than the SLA of an individual component.

For two serial dependencies:

```text
Composite SLA = SLA A × SLA B
```

Example:

```text
99.9% × 99.9%
= 0.999 × 0.999
= 0.998001
= 99.8001%
```

### Exam Thinking

> **Adding dependent components can reduce the overall composite SLA.**

---

# Service Credits

If Microsoft does not meet an applicable SLA, customers may be eligible for a **service credit** according to the service's SLA terms.

Service credits are governed by the specific agreement and generally require the applicable process to be followed.

### Exam Thinking

> **Service credit = potential billing credit when an applicable SLA commitment is not met.**

---

# Azure Marketplace

**Azure Marketplace** is an online catalog for finding, trying, purchasing, and deploying solutions that run on or integrate with Azure.

Solutions can come from:

- Microsoft
- Third-party vendors

Examples include:

- Virtual machine images
- Security products
- Databases
- Developer tools
- Business applications

### Memory Trick

> **Marketplace = SHOP for Azure solutions.**

---

# Azure Support

Microsoft provides Azure support options for different customer needs.

Support offerings can differ in:

- Technical support access
- Response times
- Scope of support
- Advisory services
- Cost

> [!NOTE]
> Support plan names, prices, and benefits can change. For AZ-900, focus on the concept that organizations can select different levels of Azure technical support.

### Exam Thinking

> **Azure Support = choose a support level based on business and technical needs.**

---

# Azure Service Lifecycle

Azure services and features can move through lifecycle stages.

Common terms include:

```text
Private Preview
      |
      v
Public Preview
      |
      v
Generally Available (GA)
      |
      v
Future updates / possible retirement
```

---

# Private Preview

A service or feature is available to a limited set of customers for testing and feedback.

### Think

> **Private Preview = limited access.**

---

# Public Preview

A service or feature is made available more broadly for evaluation and feedback.

Preview features may have different support terms and are subject to change.

### Think

> **Public Preview = broader testing/evaluation.**

---

# Generally Available (GA)

A service or feature has reached general production release.

### Think

> **GA = generally released for production use.**

---

# Retirement

Microsoft can eventually retire services or features.

Customers are typically given guidance and timelines to migrate when retirement is announced.

### Memory Trick

```text
Preview = TEST
GA      = RELEASED
Retired = MOVE AWAY
```

---

# Choosing the Right Pricing or Support Concept

### Think Pricing Calculator when:
- You need to estimate Azure resource costs before deployment.
- You want to compare configurations or regions.

### Think TCO Calculator when:
- You are comparing on-premises infrastructure with Azure.

### Think Azure Cost Management when:
- You need to monitor and optimize actual cloud spending.

### Think Reservation when:
- The workload is predictable and long-running.

### Think Spot VM when:
- The workload can tolerate interruption in exchange for lower compute cost.

### Think SLA when:
- The question asks about Microsoft's availability commitment.

### Think Azure Marketplace when:
- You need to find or deploy Microsoft or third-party Azure solutions.

### Think Service Lifecycle when:
- The question asks whether a service is Preview, GA, or being retired.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 20 Lab — Pricing & Support](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-20-Lab-20-Pricing-and-Support.md)**

### Lab Focus

- Build an estimate with the Azure Pricing Calculator.
- Estimate a Windows Virtual Machine.
- Add Azure Storage to the estimate.
- Compare pricing between two Azure regions.
- Explore the TCO Calculator.
- Compare Pricing Calculator vs. TCO Calculator.
- Browse Azure Cost Management.
- Review Azure SLA information.
- Practice Reservations, Spot VMs, Marketplace, and lifecycle scenarios.

> [!TIP]
> This lab uses estimation and exploration tools. You do not need to deploy the resources you price.

---

# Quick Check

| Need | Tool / Concept |
|---|---|
| Estimate Azure resources before deployment | Pricing Calculator |
| Compare on-premises costs with Azure | TCO Calculator |
| Monitor and optimize Azure spending | Azure Cost Management |
| Discount for predictable long-term usage | Reservation |
| Discounted interruptible compute | Spot VM |
| Availability commitment | SLA |
| Find third-party Azure solutions | Azure Marketplace |
| Production release stage | Generally Available (GA) |

---

# Before Moving On

You should be able to:

- Explain the Azure Pricing Calculator.
- Explain the TCO Calculator.
- Compare the Pricing Calculator and TCO Calculator.
- Identify major factors that affect Azure costs.
- Explain common ways to optimize Azure costs.
- Explain Azure Cost Management.
- Explain Reservations and Spot VMs.
- Explain the purpose of an SLA.
- Explain composite SLAs at a basic level.
- Explain Azure Marketplace.
- Explain Azure support at a high level.
- Distinguish Preview, GA, and retirement lifecycle stages.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Pricing Calculator** | Estimate Azure cost |
| **TCO Calculator** | On-prem vs. Azure |
| **Cost Management** | Monitor and optimize spending |
| **Reservation** | Commitment discount |
| **Spot VM** | Discounted but interruptible |
| **SLA** | Availability commitment |
| **Composite SLA** | Combined dependent-service availability |
| **Marketplace** | Find and deploy solutions |
| **Support** | Technical assistance options |
| **Preview** | Testing/evaluation |
| **GA** | General production release |
