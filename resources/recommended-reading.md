[recommended-reading.md](https://github.com/user-attachments/files/31231273/recommended-reading.md)
# Recommended Reading --- AZ-900 and Beyond

This page contains **optional resources** that complement the lessons,
labs, Microsoft Learn material, videos, and cheat sheets in this
repository.

> \[!IMPORTANT\] You do **not** need to read everything on this page to
> prepare for AZ-900. Start with the course lessons and the current
> Microsoft AZ-900 Study Guide. Use these resources when you want
> additional explanation or want to continue learning after Azure
> Fundamentals.

------------------------------------------------------------------------

# 🎯 Start Here --- Current AZ-900 Exam Information

## AZ-900 Study Guide

This should be your first reference when deciding what to study.

https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900

Use it to check:

-   Current skills measured
-   Exam topic areas
-   Changes to the exam
-   Official learning resources

> \[!TIP\] If an older video, article, or study guide conflicts with the
> current Microsoft study guide, follow Microsoft's current exam
> objectives.

------------------------------------------------------------------------

## Microsoft Azure Fundamentals Certification

Official certification page:

https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/

This page provides access to certification information, preparation
resources, the Practice Assessment, and Microsoft's Exam Sandbox.

### Exam Sandbox

The Exam Sandbox lets you become familiar with the Microsoft
certification exam interface and question experience before exam day.

Use the **Launch the sandbox** option on the certification page.

------------------------------------------------------------------------

# 🏗️ Azure Architecture Center

https://learn.microsoft.com/en-us/azure/architecture/

The Azure Architecture Center is a collection of:

-   Reference architectures
-   Example workloads
-   Architecture guides
-   Cloud design patterns
-   Technology decision guides
-   Best practices

This is **beyond what you need to memorize for AZ-900**, but it is a
great next step when you want to understand how Azure services work
together in real environments.

### Good Topics to Explore

-   Choosing an Azure compute service
-   Choosing a container service
-   Choosing a data store
-   Networking architectures
-   Storage architectures
-   Security architectures
-   Highly available applications

> \[!TIP\] AZ-900 teaches you **what the services are**. The
> Architecture Center starts showing you **how they fit together**.

------------------------------------------------------------------------

# 🧱 Azure Well-Architected Framework

https://learn.microsoft.com/en-us/azure/well-architected/

The Azure Well-Architected Framework provides guidance for designing and
improving Azure workloads.

It is organized around five pillars:

``` text
Reliability
Security
Cost Optimization
Operational Excellence
Performance Efficiency
```

### Easy Way to Think About It

``` text
Reliability
→ Will it keep working?

Security
→ Is it protected?

Cost Optimization
→ Are we spending wisely?

Operational Excellence
→ Can we operate it effectively?

Performance Efficiency
→ Can it perform and scale appropriately?
```

This material goes deeper than AZ-900, but many of the ideas connect
directly to Azure Fundamentals topics such as:

-   High availability
-   Scalability
-   Reliability
-   Security
-   Monitoring
-   Cost optimization

### Beginner Microsoft Learn Module

https://learn.microsoft.com/en-us/training/modules/azure-well-architected-introduction/

------------------------------------------------------------------------

# ☁️ Microsoft Cloud Adoption Framework

https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/

The Cloud Adoption Framework provides guidance for organizations
adopting cloud technologies.

It covers areas such as:

``` text
Strategy
   ↓
Plan
   ↓
Ready
   ↓
Migrate / Modernize / Cloud-native
   ↓
Govern
   ↓
Secure
   ↓
Manage
```

This is useful after AZ-900 because it helps connect individual Azure
services to larger business and IT decisions.

### Why Read It?

AZ-900 may teach you:

``` text
Azure Policy
RBAC
Management Groups
Cost Management
Security
Networking
```

The Cloud Adoption Framework helps answer:

> **How would an organization actually put these concepts together when
> adopting Azure?**

------------------------------------------------------------------------

# 🧪 Azure Sandbox Guidance

Microsoft also documents how organizations can create isolated Azure
sandbox environments for learning, testing, and experimentation.

https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ready/considerations/sandbox-environments

A sandbox is designed to separate experimentation from production
environments.

This is useful reading if you eventually manage Azure for an
organization and want employees or administrators to have a safer place
to learn.

> \[!NOTE\] This is different from the old Microsoft Learn training
> sandbox experience. It describes how organizations can design their
> own Azure sandbox environments.

------------------------------------------------------------------------

# 📖 Azure Documentation

https://learn.microsoft.com/en-us/azure/

The Azure documentation library is useful when you want to go deeper
into a specific service.

A good habit is:

``` text
Learn the service in AZ-900
        ↓
Use it in a lab
        ↓
Read its documentation
        ↓
Understand its real-world capabilities
```

Do not try to read the entire Azure documentation library.

Use it as a reference.

------------------------------------------------------------------------

# 🧭 Azure Service Documentation Worth Bookmarking

As you continue learning Azure, these areas are especially useful:

### Azure Virtual Machines

https://learn.microsoft.com/en-us/azure/virtual-machines/

### Azure Virtual Network

https://learn.microsoft.com/en-us/azure/virtual-network/

### Azure Storage

https://learn.microsoft.com/en-us/azure/storage/

### Microsoft Entra

https://learn.microsoft.com/en-us/entra/

### Azure Monitor

https://learn.microsoft.com/en-us/azure/azure-monitor/

### Azure Policy

https://learn.microsoft.com/en-us/azure/governance/policy/

### Azure Cost Management

https://learn.microsoft.com/en-us/azure/cost-management-billing/

> \[!TIP\] Bookmark documentation for services you actually use. There
> is no benefit to trying to memorize every Azure product page.

------------------------------------------------------------------------

# 💻 Azure Command-Line and Automation

AZ-900 does not require you to become a scripting expert, but learning
basic Azure automation is useful after you understand the fundamentals.

## Azure PowerShell

https://learn.microsoft.com/en-us/powershell/azure/

Azure PowerShell allows administrators to manage Azure resources through
PowerShell commands and scripts.

## Azure CLI

https://learn.microsoft.com/en-us/cli/azure/

Azure CLI is a cross-platform command-line tool for managing Azure.

## Bicep

https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/

Bicep is a declarative language for deploying Azure resources through
Azure Resource Manager.

### Suggested Progression

``` text
Azure Portal
     ↓
PowerShell / Azure CLI
     ↓
Bicep / Infrastructure as Code
     ↓
Automation
```

------------------------------------------------------------------------

# 🔐 Microsoft Security Learning

If the identity and security sections of AZ-900 interest you, Microsoft
has additional learning resources for:

-   Microsoft Entra
-   Zero Trust
-   Microsoft Defender
-   Microsoft Sentinel
-   Security and governance

### Microsoft Security Documentation

https://learn.microsoft.com/en-us/security/

### Microsoft Entra Documentation

https://learn.microsoft.com/en-us/entra/

These are useful areas to explore after you are comfortable with Azure
Fundamentals.

------------------------------------------------------------------------

# 📰 Azure Updates

Azure changes frequently.

Microsoft provides an Azure Updates page for new services, features,
previews, and changes:

https://azure.microsoft.com/en-us/updates/

You do not need to follow every update for AZ-900.

It becomes more useful once you actively administer Azure or continue
into more advanced certifications.

------------------------------------------------------------------------

# 🗺️ What Should I Read Next?

Use this based on your goal:

  -----------------------------------------------------------------------
  Goal                                Recommended Resource
  ----------------------------------- -----------------------------------
  **Pass AZ-900**                     Current AZ-900 Study Guide

  **Practice exam interface**         Microsoft Exam Sandbox

  **Understand real Azure designs**   Azure Architecture Center

  **Learn design best practices**     Well-Architected Framework

  **Understand organizational Azure   Cloud Adoption Framework
  adoption**                          

  **Look up a specific Azure          Azure Documentation
  service**                           

  **Learn command-line                Azure PowerShell / Azure CLI
  administration**                    

  **Learn Infrastructure as Code**    Bicep

  **Go deeper into                    Microsoft Security + Entra
  identity/security**                 documentation

  **Follow Azure changes**            Azure Updates
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 🚦 Recommended Learning Order

Do not jump into advanced architecture before learning the fundamentals.

A better progression is:

``` text
AZ-900 LESSONS
      ↓
AZ-900 LABS
      ↓
CHEAT SHEETS
      ↓
MICROSOFT PRACTICE ASSESSMENT
      ↓
PASS AZ-900
      ↓
REAL AZURE PRACTICE
      ↓
ARCHITECTURE CENTER
      ↓
WELL-ARCHITECTED FRAMEWORK
      ↓
CLOUD ADOPTION FRAMEWORK
      ↓
ROLE-BASED AZURE TRAINING
```

------------------------------------------------------------------------

# 🎓 After AZ-900

AZ-900 is a **fundamentals certification**.

After completing it, your next learning goal should depend on the type
of Azure work you want to perform.

Instead of choosing another certification only because it is the "next
number," ask:

``` text
What do I actually want to do in Azure?
```

Examples:

``` text
Administration
→ Learn more about Azure administration, identity,
  networking, compute, storage, and governance.

Security
→ Go deeper into identity, security operations,
  Defender, Sentinel, and Zero Trust.

Architecture
→ Study workload design, reliability, networking,
  governance, and the Architecture Center.

Automation
→ Learn PowerShell, Azure CLI, Bicep,
  GitHub, and Infrastructure as Code.
```

> \[!TIP\] Build practical Azure skills alongside certification study.
> Being able to explain a service is useful; being able to recognize,
> configure, troubleshoot, and automate it is even better.

------------------------------------------------------------------------

# 🔗 Recommended Reading Links

  -----------------------------------------------------------------------
  Resource                            Purpose
  ----------------------------------- -----------------------------------
  **AZ-900 Study Guide**              Current exam objectives

  **Azure Fundamentals                Exam and preparation resources
  Certification**                     

  **Azure Architecture Center**       Real-world Azure designs

  **Well-Architected Framework**      Workload design principles

  **Cloud Adoption Framework**        Organizational cloud adoption

  **Azure Documentation**             Technical service reference

  **Azure PowerShell**                PowerShell administration

  **Azure CLI**                       Command-line administration

  **Bicep**                           Infrastructure as Code

  **Microsoft Security**              Security guidance

  **Microsoft Entra**                 Identity and access

  **Azure Updates**                   New and changed Azure capabilities
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 🏁 Final Recommendation

For AZ-900 itself, keep your study scope focused:

``` text
Microsoft AZ-900 Study Guide
        +
Microsoft Learn
        +
Course Lessons
        +
John Savill Videos
        +
Labs
        +
Cheat Sheets
        +
Practice Assessment
```

Use the resources on this page when you want to understand **why Azure
is designed the way it is** and how the fundamentals you learned are
applied in real environments.

> \[!IMPORTANT\] More reading is not always better exam preparation.
> Master the current AZ-900 objectives first, then use these resources
> to continue building practical Azure knowledge.
