# Lab 20 — Pricing & Support

## Objective

This lab reinforces **Lesson 20 — Pricing & Support**.

By the end, you should be able to:

- Use the Azure Pricing Calculator.
- Estimate the cost of a Windows Virtual Machine.
- Add Azure Storage to an estimate.
- Compare Azure pricing across two regions.
- Explore the Total Cost of Ownership Calculator.
- Distinguish the Pricing Calculator from the TCO Calculator.
- Browse Azure Cost Management.
- Review Azure SLA information.
- Apply Reservations, Spot VMs, Marketplace, and lifecycle concepts to AZ-900 scenarios.

---

# Prerequisites

- Completed **Lesson 20 — Pricing & Support**
- Web browser

An Azure subscription is not required for the calculator portions of this lab.

### Start Here

- **Azure Pricing Calculator:** https://azure.microsoft.com/en-us/pricing/calculator/
- **Azure TCO Calculator:** https://azure.microsoft.com/en-us/pricing/tco/calculator/
- **Azure Cost Management:** https://learn.microsoft.com/en-us/azure/cost-management-billing/cost-management-billing-overview
- **Azure SLAs:** https://azure.microsoft.com/en-us/support/legal/sla/
- **Azure Marketplace:** https://azuremarketplace.microsoft.com/
- **Azure Support:** https://azure.microsoft.com/en-us/support/
- **Azure Reservations:** https://learn.microsoft.com/en-us/azure/cost-management-billing/reservations/save-compute-costs-reservations
- **Azure Spot Virtual Machines:** https://learn.microsoft.com/en-us/azure/virtual-machines/spot-vms

> [!IMPORTANT]
> The Pricing Calculator and TCO Calculator produce **estimates**, not guaranteed future bills. Azure prices, services, discounts, and support offerings can change.

---

# Part 1 — Open the Azure Pricing Calculator

### Link

https://azure.microsoft.com/en-us/pricing/calculator/

## Steps

1. Open the Azure Pricing Calculator.
2. Browse the available products.
3. Locate **Virtual Machines**.
4. Add Virtual Machines to your estimate.
5. Do not deploy anything in Azure.

## Question

What is the main purpose of the Pricing Calculator?

**Answer:** _______________________________________________

### Exam Thinking

> **Pricing Calculator = estimate Azure costs before deployment.**

---

# Part 2 — Estimate a Windows Virtual Machine

## Steps

Configure a sample Virtual Machine estimate.

The calculator interface can change, but look for settings such as:

- Region
- Operating system
- VM type or size
- Number of instances
- Hours
- Pricing option

Use a reasonable general-purpose Windows VM configuration.

Record your choices:

| Setting | Selection |
|---|---|
| Region | ______________________________ |
| Operating System | Windows |
| VM Size | ______________________________ |
| Number of VMs | ______________________________ |
| Estimated Monthly Cost | ______________________________ |

## Think About It

Which settings caused the estimate to change?

**Answer:** _______________________________________________

Would a larger VM generally cost more or less?

**Answer:** _______________________________________________

---

# Part 3 — Add Azure Storage

## Steps

1. Add **Storage Accounts** or the relevant Azure Storage product to the same estimate.
2. Choose a sample storage configuration.
3. Review settings such as:
   - Region
   - Storage type
   - Redundancy
   - Capacity
   - Transactions, if shown
4. Record the estimate.

| Setting | Selection |
|---|---|
| Region | ______________________________ |
| Storage / Service Type | ______________________________ |
| Redundancy | ______________________________ |
| Capacity | ______________________________ |
| Estimated Monthly Cost | ______________________________ |

## Question

Name two storage settings that can affect price.

**Answer:** _______________________________________________

---

# Part 4 — Compare Two Azure Regions

## Steps

1. Record the current VM region and estimated cost.
2. Change only the **region**.
3. Select a different Azure region.
4. Keep the other VM settings as similar as possible.
5. Record the new estimate.

| | Region 1 | Region 2 |
|---|---|---|
| Region | __________________ | __________________ |
| VM Configuration | __________________ | __________________ |
| Estimated Cost | __________________ | __________________ |

## Questions

Was the price identical?

**Answer:** _______________________________________________

What does this demonstrate?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure region can affect resource cost.**

---

# Part 5 — Explore Purchasing Options

Depending on the current calculator options, review available purchasing models such as:

- Pay-as-you-go
- Reservation options
- Savings options

Do not purchase anything.

## Questions

Which option provides the greatest flexibility for unpredictable usage?

**Answer:** _______________________________________________

Why might a long-running predictable workload benefit from a commitment-based pricing option?

**Answer:** _______________________________________________

---

# Part 6 — Explore the TCO Calculator

### Link

https://azure.microsoft.com/en-us/pricing/tco/calculator/

## Steps

1. Open the Azure TCO Calculator.
2. Review the categories of on-premises information it asks for.
3. If the current calculator permits, create a simple sample scenario involving one on-premises server.
4. Review assumptions involving areas such as:
   - Servers
   - Storage
   - Networking
   - IT labor
   - Electricity or datacenter costs
5. Review the resulting comparison or report.

> [!NOTE]
> Microsoft's calculator interface can change. The important part of this exercise is understanding **what TCO compares**, not producing a specific dollar amount.

## Questions

What two environments does the TCO Calculator compare?

**Answer:** _______________________________________________

Why would an organization use the TCO Calculator before a cloud migration?

**Answer:** _______________________________________________

### Exam Thinking

> **TCO = on-premises vs. Azure.**

---

# Part 7 — Pricing Calculator vs. TCO Calculator

Choose:

- **Pricing Calculator**
- **TCO Calculator**

### Scenario 1

A company wants to estimate the monthly price of three Azure Virtual Machines.

**Answer:** ______________________________

### Scenario 2

A company wants to compare its existing datacenter costs with Azure.

**Answer:** ______________________________

### Scenario 3

An architect wants to compare the estimated price of an Azure service in two regions.

**Answer:** ______________________________

### Scenario 4

Management wants financial information to help evaluate whether moving existing servers to Azure makes sense.

**Answer:** ______________________________

### Memory Trick

```text
Pricing = AZURE COST
TCO     = ON-PREM vs. AZURE
```

---

# Part 8 — Browse Azure Cost Management

### Links

- **Azure Portal:** https://portal.azure.com/
- **Cost Management + Billing Overview:** https://learn.microsoft.com/en-us/azure/cost-management-billing/cost-management-billing-overview
- **Azure Budgets:** https://learn.microsoft.com/en-us/azure/cost-management-billing/costs/tutorial-acm-create-budgets

## Steps

If you have an Azure subscription with permission to view billing information:

1. Open the Azure Portal.
2. Search for **Cost Management + Billing**.
3. Browse **Cost analysis**.
4. Locate **Budgets**.
5. Review the interface without creating or changing company budgets.

If you do not have billing access, use the Microsoft documentation instead.

## Questions

What is Azure Cost Management used for?

**Answer:** _______________________________________________

What is the purpose of an Azure budget?

**Answer:** _______________________________________________

Does reaching a budget threshold automatically shut down every Azure resource?

**Answer:** _______________________________________________

---

# Part 9 — Review Azure SLAs

### Links

- **Azure SLAs:** https://azure.microsoft.com/en-us/support/legal/sla/
- **Azure SLA Documentation:** https://learn.microsoft.com/en-us/azure/architecture/framework/resiliency/business-metrics

## Steps

1. Open the Azure SLA page.
2. Select or review an Azure service.
3. Look for:
   - Availability commitments
   - Conditions
   - Service credits
4. Do not try to memorize every percentage.

## Questions

What does an SLA describe?

**Answer:** _______________________________________________

What generally happens to allowed downtime as an SLA percentage increases?

**Answer:** _______________________________________________

What is a service credit?

**Answer:** _______________________________________________

---

# Part 10 — Composite SLA Practice

Assume an application requires **two dependent services**, and each has an SLA of **99.9%**.

Convert each percentage to decimal form:

```text
99.9% = 0.999
```

Multiply:

```text
0.999 × 0.999 = 0.998001
```

Convert back to a percentage:

```text
99.8001%
```

## Question

Is the composite SLA higher or lower than 99.9%?

**Answer:** _______________________________________________

### Exam Thinking

> **Dependent services can reduce the application's overall composite SLA.**

---

# Part 11 — Reservations vs. Spot VMs

### Links

- **Azure Reservations:** https://learn.microsoft.com/en-us/azure/cost-management-billing/reservations/save-compute-costs-reservations
- **Azure Spot Virtual Machines:** https://learn.microsoft.com/en-us/azure/virtual-machines/spot-vms

Choose:

- **Reservation**
- **Spot VM**
- **Pay-As-You-Go**

### Scenario 1

A production workload is expected to run continuously for several years with predictable usage.

**Answer:** ______________________________

### Scenario 2

A batch-processing workload can be interrupted and restarted later.

**Answer:** ______________________________

### Scenario 3

A temporary workload has unpredictable usage and the company does not want a long-term commitment.

**Answer:** ______________________________

### Scenario 4

The organization wants discounted compute but can tolerate eviction.

**Answer:** ______________________________

### Memory Trick

```text
Reservation   = COMMIT
Spot VM       = INTERRUPTIBLE
Pay-As-You-Go = FLEXIBLE
```

---

# Part 12 — Browse Azure Marketplace

### Link

https://azuremarketplace.microsoft.com/

## Steps

1. Open Azure Marketplace.
2. Search for a general category such as:
   - Firewall
   - Database
   - Linux
3. Review several results.
4. Do not purchase or deploy anything.

## Questions

Can Azure Marketplace contain solutions from third-party vendors?

**Answer:** _______________________________________________

What is the primary purpose of Azure Marketplace?

**Answer:** _______________________________________________

### Exam Thinking

> **Marketplace = discover and deploy cloud solutions.**

---

# Part 13 — Review the Azure Service Lifecycle

### Links

- **Azure Updates:** https://azure.microsoft.com/en-us/updates/
- **Azure Preview Terms:** https://azure.microsoft.com/en-us/support/legal/preview-supplemental-terms/

Match the lifecycle stage to the description.

### 1.

Available to a limited group for early testing.

**Answer:** ______________________________

### 2.

Available more broadly for evaluation and feedback.

**Answer:** ______________________________

### 3.

Generally released for production use.

**Answer:** ______________________________

### 4.

A service or feature is being discontinued and customers need to migrate.

**Answer:** ______________________________

Choose from:

- Private Preview
- Public Preview
- Generally Available (GA)
- Retirement

### Memory Trick

```text
Private Preview = LIMITED TEST
Public Preview  = BROADER TEST
GA              = RELEASED
Retirement      = MIGRATE AWAY
```

---

# Part 14 — Pricing & Support Scenarios

Choose from:

- **Pricing Calculator**
- **TCO Calculator**
- **Azure Cost Management**
- **Reservation**
- **Spot VM**
- **SLA**
- **Azure Marketplace**
- **Generally Available (GA)**

### Scenario 1

Estimate an Azure workload before deployment.

**Answer:** ______________________________

### Scenario 2

Compare an existing datacenter with Azure.

**Answer:** ______________________________

### Scenario 3

Analyze actual Azure spending after resources are running.

**Answer:** ______________________________

### Scenario 4

Reduce cost for a predictable long-running supported workload.

**Answer:** ______________________________

### Scenario 5

Run an interruptible batch workload at a lower compute price.

**Answer:** ______________________________

### Scenario 6

Determine Microsoft's availability commitment for an Azure service.

**Answer:** ______________________________

### Scenario 7

Find a third-party security application that can be deployed in Azure.

**Answer:** ______________________________

### Scenario 8

Choose the lifecycle stage representing general production release.

**Answer:** ______________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

The Pricing Calculator estimates Azure resource costs before deployment.

## Parts 2–4

Costs can change based on configuration, size, region, storage, usage, and purchasing options. Region is one factor that can affect Azure pricing.

## Part 5

Pay-as-you-go provides flexibility. Commitment-based pricing can reduce cost for predictable long-running usage.

## Part 6

The TCO Calculator compares on-premises infrastructure costs with estimated Azure costs. Organizations can use it to help evaluate the financial case for migration.

## Part 7

| Scenario | Answer |
|---|---|
| 1 | Pricing Calculator |
| 2 | TCO Calculator |
| 3 | Pricing Calculator |
| 4 | TCO Calculator |

## Part 8

Azure Cost Management helps monitor, analyze, and optimize cloud spending. Budgets track spending against defined thresholds and can trigger alerts. A budget threshold does not inherently shut down every Azure resource.

## Part 9

An SLA describes Microsoft's availability commitment and associated terms. Higher availability percentages generally mean less allowable downtime. Service credits may apply when Microsoft does not meet an applicable SLA under its terms.

## Part 10

The composite SLA is **99.8001%**, which is lower than 99.9%.

## Part 11

| Scenario | Answer |
|---|---|
| 1 | Reservation |
| 2 | Spot VM |
| 3 | Pay-As-You-Go |
| 4 | Spot VM |

## Part 12

Yes. Azure Marketplace can contain Microsoft and third-party solutions. Its purpose is to help customers discover and deploy solutions for Azure.

## Part 13

1. Private Preview
2. Public Preview
3. Generally Available (GA)
4. Retirement

## Part 14

| Scenario | Answer |
|---|---|
| 1 | Pricing Calculator |
| 2 | TCO Calculator |
| 3 | Azure Cost Management |
| 4 | Reservation |
| 5 | Spot VM |
| 6 | SLA |
| 7 | Azure Marketplace |
| 8 | Generally Available (GA) |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Factors that affect Azure cost.
- Pricing Calculator vs. TCO Calculator.
- Azure Cost Management.
- Budgets.
- Reservations.
- Spot VMs.
- Azure SLAs and composite SLAs.
- Azure Marketplace.
- Azure support at a high level.
- Private Preview, Public Preview, GA, and retirement.
- Which pricing or support concept best fits a basic AZ-900 scenario.
