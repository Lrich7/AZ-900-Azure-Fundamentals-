# Lab 02 — Cloud Models & Azure Arc

## Objective

This lab reinforces the concepts from **Lesson 2 — Cloud Benefits & Cloud Models**.

By the end of the lab, you should be able to:

- Identify Public, Private, Hybrid, and Multi-Cloud environments.
- Recognize cloud models from real-world scenarios.
- Explain the purpose of Azure Arc.
- Explore Azure Arc in the Azure Portal.
- Explain the difference between Azure Arc and Azure VMware Solution.

---

## Prerequisites

- Completed **Lesson 2 — Cloud Benefits & Cloud Models**
- Access to the Azure Portal for the Azure Arc exploration activity

> [!NOTE]
> You do **not** need to deploy any Azure resources for this lab.

---

# Part 1 — Identify the Cloud Model

For each scenario, determine whether it represents:

- **Public Cloud**
- **Private Cloud**
- **Hybrid Cloud**
- **Multi-Cloud**

Write down your answer before opening the answer section.

### Scenario 1

A company runs all of its servers in its own private datacenter. The company controls the hardware, networking, security, and virtual machines.

**Cloud Model:** ______________________

### Scenario 2

A startup runs its entire application using Microsoft Azure resources and does not maintain its own datacenter.

**Cloud Model:** ______________________

### Scenario 3

A company keeps a sensitive customer database on-premises but hosts its public website in Microsoft Azure.

**Cloud Model:** ______________________

### Scenario 4

A company uses Microsoft Azure for identity-related workloads, AWS for application hosting, and Google Cloud for analytics.

**Cloud Model:** ______________________

### Scenario 5

A company operates a private VMware environment in its own datacenter and connects that environment with services running in Microsoft Azure.

**Cloud Model:** ______________________

---

# Part 2 — Explore Azure Arc

## Step 1 — Open Azure Arc

1. Sign in to the **Azure Portal**.
2. Use the search bar at the top of the portal.
3. Search for **Azure Arc**.
4. Open **Azure Arc**.

---

## Step 2 — Explore the Available Resources

Review the Azure Arc interface and look for the types of resources that can be managed.

Look for examples related to:

- Servers
- Kubernetes
- Data services
- Other resources outside Azure

You do not need to connect or deploy anything.

---

## Step 3 — Think Like an Administrator

Consider the following environment:

```text
                    Azure Portal
                         │
        ┌────────────────┼────────────────┐
        │                │                │
   On-Premises       Other Clouds      Edge
      Servers         / Kubernetes     Devices
        │                │                │
        └──────────── Azure Arc ──────────┘
```

Answer the following:

1. Would Azure Arc require the on-premises servers to be migrated into Azure?

   **Answer:** _______________________________

2. What is the main benefit of connecting these resources to Azure Arc?

   **Answer:** _______________________________

3. Name two Azure management or governance capabilities that could be useful across these environments.

   **Answer:** _______________________________

---

# Part 3 — Azure Arc vs. Azure VMware Solution

Determine which Microsoft service best fits each scenario.

Choose:

- **Azure Arc**
- **Azure VMware Solution (AVS)**

### Scenario 1

An organization wants to keep servers in its local datacenter but manage supported resources using Azure management and governance capabilities.

**Service:** ______________________

### Scenario 2

An organization wants to move its existing VMware environment into Azure while continuing to use familiar VMware technologies.

**Service:** ______________________

### Scenario 3

An administrator wants centralized governance for resources located on-premises and in other cloud environments.

**Service:** ______________________

### Scenario 4

A company wants to lift and shift VMware workloads to infrastructure hosted in Azure.

**Service:** ______________________

---

# Part 4 — Exam Thinking

Complete these statements without looking back at the lesson.

1. **Private Cloud** = ______________________________________

2. **Public Cloud** = ______________________________________

3. **Hybrid Cloud** = ______________________________________

4. **Multi-Cloud** = ______________________________________

5. **Azure Arc** = ______________________________________

6. **Azure VMware Solution** = ______________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

| Scenario | Answer |
|---|---|
| 1 | Private Cloud |
| 2 | Public Cloud |
| 3 | Hybrid Cloud |
| 4 | Multi-Cloud |
| 5 | Hybrid Cloud |

## Part 2

1. **No.** Azure Arc allows supported resources outside Azure to be managed without moving those resources into Azure.
2. Centralized Azure management and governance across environments.
3. Examples from Lesson 2 include **Azure Policy, Azure RBAC, resource tagging, monitoring, and security integration**.

## Part 3

| Scenario | Answer |
|---|---|
| 1 | Azure Arc |
| 2 | Azure VMware Solution |
| 3 | Azure Arc |
| 4 | Azure VMware Solution |

## Part 4

- **Private Cloud:** Dedicated environment for one organization.
- **Public Cloud:** Provider-owned cloud infrastructure delivered over the internet.
- **Hybrid Cloud:** Private/on-premises and public-cloud environments working together.
- **Multi-Cloud:** Two or more cloud providers.
- **Azure Arc:** Manage supported resources across Azure, on-premises, edge, and other clouds.
- **Azure VMware Solution:** VMware environment running on Azure infrastructure.

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Why a scenario is Public, Private, Hybrid, or Multi-Cloud.
- Why Azure Arc is a **management** solution rather than a migration solution.
- When Azure VMware Solution would be used instead of Azure Arc.
