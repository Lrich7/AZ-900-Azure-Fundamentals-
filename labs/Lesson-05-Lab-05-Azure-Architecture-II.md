[Lesson-05-Lab-05-Azure-Architecture-II.md](https://github.com/user-attachments/files/31083391/Lesson-05-Lab-05-Azure-Architecture-II.md)

# Lab 05 — Azure Architecture II

## Objective

This lab reinforces **Lesson 5 — Azure Architecture II**.

By the end, you should be able to:
- Create and inspect a Resource Group.
- Locate your Azure Subscription.
- Explore Management Groups.
- Understand how resources can be moved between Resource Groups.
- Identify the Azure resource hierarchy.

---

## Prerequisites
- Completed **Lesson 5 — Azure Architecture II**
- Azure account
- Web browser

### Start Here
- **Azure Portal:** https://portal.azure.com/
- **Manage Azure Resource Groups:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups

> [!NOTE]
> Management Group options may vary depending on your tenant and permissions.

---

# Part 1 — Create a Resource Group

### Links
- **Azure Portal:** https://portal.azure.com/
- **Manage Azure Resource Groups:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups

## Steps
1. Open the Azure Portal.
2. Search for **Resource groups**.
3. Open **Resource groups**.
4. Select **Create**.
5. Select your Azure Subscription.
6. Enter a name such as `AZ900-Lab-RG`.
7. Select an available region.
8. Review the settings and create the Resource Group.
9. Open it after creation.

## Record What You Find
**Resource Group Name:** __________________________________

**Resource Group Region:** _________________________________

## Think About It
Does every resource inside the Resource Group have to be in the same Azure region?

**Answer:** _______________________________________________

What happens to contained resources if the Resource Group is deleted?

**Answer:** _______________________________________________

### Exam Thinking
> **Resource Group = logical container for related Azure resources.**

---

# Part 2 — View Your Azure Subscription

### Links
- **Azure Portal:** https://portal.azure.com/
- **Azure Subscriptions:** https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/create-subscription

## Steps
1. Open the Azure Portal.
2. Search for **Subscriptions**.
3. Open **Subscriptions**.
4. Select your subscription.
5. Review the Overview page.
6. Locate the subscription name, Subscription ID, and status.

> [!IMPORTANT]
> Do not publish your Subscription ID or other tenant/account identifiers in your public GitHub repository.

## Think About It
Why might a company use separate subscriptions for Production and Development?

**Answer:** _______________________________________________

### Exam Thinking
> **Subscription = billing and management boundary.**

---

# Part 3 — Explore Management Groups

### Links
- **Azure Portal:** https://portal.azure.com/
- **Management Groups Overview:** https://learn.microsoft.com/en-us/azure/governance/management-groups/overview

## Steps
1. Open the Azure Portal.
2. Search for **Management groups**.
3. Open **Management groups**.
4. Review the hierarchy if your account has permission.
5. Look for the relationship between Management Groups and Subscriptions.

If the page is unavailable in your tenant, use the Microsoft documentation link instead.

## Think About It
What is located below a Management Group?

**Answer:** _______________________________________________

Why would a large organization use Management Groups?

**Answer:** _______________________________________________

### Exam Thinking
> **Management Group = organize and govern multiple Azure subscriptions.**

---

# Part 4 — Moving Resources Between Resource Groups

### Links
- **Move Azure Resources:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/move-resource-group-and-subscription
- **Azure Portal:** https://portal.azure.com/

> [!NOTE]
> You do not need to move a real resource to complete this section.

## Steps
1. Open the **Move Azure Resources** documentation.
2. Review the requirements and limitations.
3. Note that move support depends on the resource type.
4. If you have safe test resources, review the **Move** options in the Azure Portal.
5. Do not move production or business resources for this AZ-900 exercise.

## Think About It
Can some Azure resources be moved between Resource Groups?

**Answer:** _______________________________________________

Should you assume every resource supports every type of move?

**Answer:** _______________________________________________

---

# Part 5 — Build the Azure Hierarchy

Fill in the levels:

```text
____________________
        |
        v
____________________
        |
        v
____________________
        |
        v
____________________
```

Choose from:
- Resource
- Resource Group
- Subscription
- Management Group

---

# Part 6 — Real-World Scenarios

Choose **Resource, Resource Group, Subscription, or Management Group**.

### Scenario 1
A company wants one logical container for the VM, storage, and networking resources used by one application.

**Answer:** ______________________________

### Scenario 2
A company wants separate billing and administrative boundaries for Production and Development.

**Answer:** ______________________________

### Scenario 3
A large company wants to apply governance across many Azure subscriptions.

**Answer:** ______________________________

### Scenario 4
An Azure Virtual Machine is being created. What level is the VM itself?

**Answer:** ______________________________

---

# Part 7 — Exam Thinking

1. **Resource** = __________________________________________
2. **Resource Group** = ___________________________________
3. **Subscription** = ______________________________________
4. **Management Group** = _________________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1
A Resource Group is a logical container. Resources inside it can exist in different Azure regions.

Deleting a Resource Group deletes the resources contained within it.

## Part 2
Separate subscriptions can help separate billing, access, administration, departments, projects, and environments.

## Part 3
Subscriptions exist below Management Groups. Management Groups help apply governance and access controls across multiple subscriptions.

## Part 4
Some Azure resources can be moved between Resource Groups or subscriptions, but support and requirements vary by resource type.

## Part 5

```text
Management Group
        |
        v
Subscription
        |
        v
Resource Group
        |
        v
Resource
```

## Part 6

| Scenario | Answer |
|---|---|
| 1 | Resource Group |
| 2 | Subscription |
| 3 | Management Group |
| 4 | Resource |

## Part 7
- **Resource:** Individual Azure service or asset.
- **Resource Group:** Logical container for related Azure resources.
- **Subscription:** Billing and management boundary.
- **Management Group:** Organizes and governs multiple subscriptions.

</details>

---

# Lab Cleanup

If you created `AZ900-Lab-RG` and it contains nothing you need, you can delete it after completing the exercise.

- **Resource Group Management:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups

> [!CAUTION]
> Always verify the contents before deleting a Resource Group. Deleting it also deletes its contained resources.

---

# Lab Complete

Before moving on, make sure you can explain:
- Resource vs. Resource Group.
- Resource Group vs. Subscription.
- Subscription vs. Management Group.
- The Azure management hierarchy.
- Why organizations may use multiple subscriptions.
