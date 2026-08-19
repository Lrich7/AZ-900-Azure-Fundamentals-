[azure-free-account.md](https://github.com/user-attachments/files/31231197/azure-free-account.md)

# Azure Free Account --- Setup Guide

This guide explains how to get access to Microsoft Azure for the
hands-on portions of this AZ-900 training course and how to explore
Azure while reducing the risk of unexpected charges.

> \[!IMPORTANT\] Azure offers, free-service limits, credits, and
> eligibility can change. Always review Microsoft's current Azure Free
> Account page before signing up or creating resources.

------------------------------------------------------------------------

# ☁️ Do You Need an Azure Account?

You do **not** need to deploy Azure resources for every lesson in this
course.

Many AZ-900 topics can be learned through:

-   Microsoft Learn
-   Azure documentation
-   Videos
-   Diagrams
-   Scenario questions
-   Portal exploration

However, an Azure account is useful for hands-on labs that ask you to
explore the **Azure Portal**, create resources, review configuration
options, or practice basic Azure administration.

------------------------------------------------------------------------

# 🆓 Azure Free Account

Microsoft currently offers an **Azure Free Account** for eligible new
Azure customers.

At the time this guide was written, Microsoft lists:

-   **\$200 USD in Azure credit for 30 days**
-   Free monthly amounts of selected popular services for the first 12
    months
-   Free monthly amounts of additional services that remain available
    beyond the first 12 months
-   Spending protection on the free-account credit
-   The option to move to pay-as-you-go if you choose to continue beyond
    the free-account limits

> \[!NOTE\] Do not rely on this guide for the current dollar amounts,
> service limits, or eligibility requirements. Microsoft can change the
> Azure Free Account offer.

### Official Links

-   **Create or Review an Azure Free Account:**\
    https://azure.microsoft.com/en-us/pricing/purchase-options/azure-account

-   **Explore Azure Free Services:**\
    https://azure.microsoft.com/en-us/pricing/free-services/

-   **Avoid Charges with an Azure Free Account:**\
    https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/avoid-charges-free-account

------------------------------------------------------------------------

# ⚠️ Before You Sign Up

Read Microsoft's current offer before creating your account.

You may need:

-   A Microsoft account
-   A phone number for identity verification
-   A credit or debit card for account verification

Microsoft may place a temporary authorization on the card during
verification.

> \[!CAUTION\] Providing a payment method for verification is not the
> same as choosing to use paid Azure services. However, if you later
> move the subscription to pay-as-you-go, usage beyond applicable free
> amounts can result in charges.

------------------------------------------------------------------------

# 🚀 Step 1 --- Create Your Azure Account

Go to:

https://azure.microsoft.com/en-us/pricing/purchase-options/azure-account

Select the option to try Azure for free and follow Microsoft's signup
process.

During signup:

1.  Sign in with your Microsoft account.
2.  Complete identity verification.
3.  Complete payment-method verification if required.
4.  Review the subscription terms.
5.  Finish creating the account.

> \[!TIP\] Read each screen rather than clicking through quickly. Pay
> particular attention to anything mentioning **pay-as-you-go**,
> **upgrade**, **billing**, or **spending limits**.

------------------------------------------------------------------------

# 🌐 Step 2 --- Open the Azure Portal

After your account is ready, open:

https://portal.azure.com/

The **Azure Portal** is the web interface used to manage Azure.

You will use it throughout several labs in this course.

### Things You May See

``` text
Azure Portal
    |
    +-- Resource Groups
    +-- Virtual Machines
    +-- Storage Accounts
    +-- Virtual Networks
    +-- Microsoft Entra ID
    +-- Cost Management
    +-- Azure Monitor
    +-- Azure Advisor
    +-- Service Health
    +-- Azure Arc
    +-- More Azure Services
```

Do not worry about learning everything at once.

The purpose of the labs is to gradually introduce these areas.

------------------------------------------------------------------------

# 🔎 Step 3 --- Check Your Subscription

In the Azure Portal:

1.  Use the search bar at the top.
2.  Search for **Subscriptions**.
3.  Open **Subscriptions**.
4.  Select your Azure subscription.
5.  Review the subscription information.

Your subscription is an important part of the Azure hierarchy:

``` text
Management Group
       ↓
Subscription
       ↓
Resource Group
       ↓
Resource
```

### AZ-900 Connection

Remember:

> **Subscription = management and billing boundary.**

Resources you create are associated with an Azure subscription.

------------------------------------------------------------------------

# 💳 Step 4 --- Understand the Spending Limit

Azure free accounts normally begin with a spending limit associated with
the included credit.

Microsoft documents the spending limit here:

https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/spending-limit

The spending limit is designed to help prevent spending beyond the
available credit for eligible subscription types.

> \[!WARNING\] Do **not** remove the spending limit just to complete
> these AZ-900 labs.

Removing a spending limit can allow usage to generate charges when the
subscription is otherwise eligible to bill for that usage.

If your goal is simply to learn Azure Fundamentals, keep the protections
provided by your account unless you have a specific reason to change
them and understand the billing consequences.

------------------------------------------------------------------------

# 💰 Step 5 --- Learn Where Costs Are Shown

In the Azure Portal, search for:

``` text
Cost Management + Billing
```

Depending on your subscription and permissions, this area can help you
review:

-   Current costs
-   Usage
-   Remaining credit
-   Budgets
-   Cost analysis
-   Billing information

### Official Cost Management Documentation

https://learn.microsoft.com/en-us/azure/cost-management-billing/

### AZ-900 Connection

Remember:

``` text
Pricing Calculator
= Estimate costs BEFORE deployment

Cost Management
= Monitor costs AFTER resources are running
```

------------------------------------------------------------------------

# 📊 Step 6 --- Consider Creating a Budget

A budget can help you track spending against an amount you define.

Microsoft's budget tutorial:

https://learn.microsoft.com/en-us/azure/cost-management-billing/costs/tutorial-acm-create-budgets

A typical path is:

``` text
Azure Portal
     ↓
Subscriptions
     ↓
Your Subscription
     ↓
Budgets
```

You can then create a budget and configure notifications where
supported.

> \[!IMPORTANT\] A **budget is not automatically a hard spending cap**.
> It is primarily a cost-tracking and alerting tool. Do not assume that
> creating a budget prevents Azure resources from generating charges.

------------------------------------------------------------------------

# 📁 Step 7 --- Create a Lab Resource Group

For labs that actually require resources, keeping your training
resources together makes cleanup easier.

A useful name is:

``` text
AZ900-Labs
```

To create one:

1.  Open the Azure Portal.
2.  Search for **Resource groups**.
3.  Select **Create**.
4.  Choose your subscription.
5.  Enter:

``` text
Resource group:
AZ900-Labs
```

6.  Select an appropriate Azure region.
7.  Review the configuration.
8.  Select **Create**.

> \[!TIP\] When a lab gives you a specific resource-group name, use the
> name provided by that lab instead.

### Why Use a Lab Resource Group?

Instead of scattering temporary resources throughout the subscription:

``` text
Subscription
   |
   +-- Random VM
   +-- Random Storage
   +-- Random Network
   +-- Random Resources
```

keep disposable training resources organized:

``` text
Subscription
   |
   +-- AZ900-Labs
          |
          +-- Lab VM
          +-- Lab Storage
          +-- Lab Network
```

This can make it much easier to identify what was created for training.

------------------------------------------------------------------------

# 🚨 Free Does Not Mean Everything Is Free

An Azure Free Account provides access to Azure, but that does **not**
mean every Azure resource can be used without cost.

Microsoft provides specific free amounts for specific services.

Always check:

-   Whether the service is included in the free offer
-   Which service tier is free
-   The monthly free limit
-   The selected region
-   The resource size/SKU
-   How long the resource will run

### Check Current Free Services

https://azure.microsoft.com/en-us/pricing/free-services/

> \[!CAUTION\] A resource appearing in the Azure Portal does **not**
> mean that resource is free.

------------------------------------------------------------------------

# 🧪 Rules for This Course's Labs

Use these rules when completing hands-on activities:

### 1. Explore Before You Deploy

If the lab only asks you to **view**, **find**, **compare**, or
**identify** something, do not create a resource unless the lab
specifically tells you to.

### 2. Use the Smallest Appropriate Resource

When a lab requires a resource, follow the lab's instructions and choose
free or low-cost options when available.

### 3. Never Use Production Resources

Do not use:

-   Employer production subscriptions
-   Company production Resource Groups
-   Production servers
-   Production networks
-   Production storage accounts

for personal AZ-900 practice.

### 4. Delete Temporary Resources

If a resource was created only for a lab and is no longer needed, remove
it when the lab is finished.

### 5. Check Cost Management

Make a habit of reviewing Azure costs and usage.

------------------------------------------------------------------------

# 🧹 Step 8 --- Clean Up After Labs

Resource cleanup is one of the most important habits to learn.

If all resources inside a Resource Group were created only for training,
deleting the Resource Group can remove the resources it contains.

### Azure Portal

``` text
Azure Portal
     ↓
Resource Groups
     ↓
Select Lab Resource Group
     ↓
Delete Resource Group
```

Microsoft's official instructions:

https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/delete-resource-group

> \[!CAUTION\] Deleting a Resource Group is destructive and cannot
> simply be undone. Verify that the Resource Group contains **only
> disposable lab resources** before deleting it.

Never delete a Resource Group just because its name looks like a lab
group. Inspect its contents first.

------------------------------------------------------------------------

# 🛑 Stop vs. Delete

Stopping a resource and deleting a resource are not always the same
thing.

For example, some Azure resources may continue to have associated
storage, networking, or other billable components even when the main
workload is stopped.

For temporary training environments:

> **If the lab is finished and you no longer need the resources,
> deletion is usually safer than assuming "stopped" means "free."**

Always verify what resources remain.

------------------------------------------------------------------------

# 🔍 Before Creating Any Resource

Use this quick checklist:

``` text
□ Does the lab actually require me to create this?

□ Is this the correct subscription?

□ Is this a lab Resource Group?

□ Is there a free or lower-cost option?

□ Does Azure show an estimated cost?

□ Do I know how to delete it afterward?

□ Am I sure this is NOT a production resource?
```

If you cannot answer these questions confidently, review the lab
instructions before continuing.

------------------------------------------------------------------------

# 🎓 Azure for Students

If you are an eligible student, Microsoft also offers **Azure for
Students**.

Review the current offer here:

https://azure.microsoft.com/en-us/free/students/

Eligibility, credits, included services, and terms can change, so check
Microsoft's current page for details.

------------------------------------------------------------------------

# 🔗 Useful Azure Links

  ---------------------------------------------------------------------------------------------------------------------------------------
  Resource                            Link
  ----------------------------------- ---------------------------------------------------------------------------------------------------
  **Azure Portal**                    https://portal.azure.com/

  **Azure Free Account**              https://azure.microsoft.com/en-us/pricing/purchase-options/azure-account

  **Azure Free Services**             https://azure.microsoft.com/en-us/pricing/free-services/

  **Microsoft Learn**                 https://learn.microsoft.com/training/

  **AZ-900 Study Guide**              https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900

  **AZ-900 Certification**            https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/

  **Azure Pricing Calculator**        https://azure.microsoft.com/en-us/pricing/calculator/

  **Azure Cost Management**           https://learn.microsoft.com/en-us/azure/cost-management-billing/

  **Avoid Free Account Charges**      https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/avoid-charges-free-account

  **Azure Spending Limit**            https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/spending-limit

  **Azure Budgets**                   https://learn.microsoft.com/en-us/azure/cost-management-billing/costs/tutorial-acm-create-budgets

  **Delete Resource Groups**          https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/delete-resource-group
  ---------------------------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

# ✅ Ready for the Labs?

Before starting a hands-on Azure lab, make sure you can:

-   Sign in to the Azure Portal.
-   Identify your Azure subscription.
-   Find Resource Groups.
-   Understand that Azure resources can generate costs.
-   Find Cost Management.
-   Check the current Azure Free Services offer.
-   Understand that a budget is not necessarily a hard spending limit.
-   Keep training resources separate from production resources.
-   Delete disposable lab resources when finished.

------------------------------------------------------------------------

# 🧠 AZ-900 Connections

Setting up your lab environment also reinforces several concepts that
appear on the exam:

  What You Just Used   AZ-900 Concept
  -------------------- -------------------------------------
  Azure subscription   Management + billing boundary
  Resource Group       Logical container
  Azure Portal         Azure management tool
  Cost Management      Monitor and optimize Azure spending
  Budget               Cost tracking and alerts
  Free services        Azure pricing and consumption
  Resource cleanup     Resource lifecycle management

> \[!TIP\] Treat the Azure Free Account as a **learning environment**,
> not a challenge to use all of the available credit. For AZ-900,
> understanding the services is more important than deploying expensive
> resources.
