[answer-key-1.md](https://github.com/user-attachments/files/31232257/answer-key-1.md)

# AZ-900 Practice Exam 1 --- Answer Key

Answer key for **Practice Exam 1 --- Lessons 1--6**.

> \[!TIP\] Do not just count correct answers. Review the explanation for
> every question you missed **or guessed on**.

------------------------------------------------------------------------

# 📊 Score Guide

  Score          Percentage Recommendation
  ------------ ------------ ----------------------------
  **36--40**       90--100% Excellent --- move forward
  **32--35**      80--87.5% Ready to move forward
  **28--31**      70--77.5% Review weak areas
  **0--27**       Below 70% Revisit Lessons 1--6

> \[!NOTE\] This score guide is for this training repository. It is not
> Microsoft's official AZ-900 exam scoring system.

------------------------------------------------------------------------

# ✅ Answer Key

    \#    Answer     Topic
  ---- ------------- ------------------------------
     1     **B**     CapEx
     2     **C**     Consumption-based pricing
     3     **B**     OpEx
     4     **B**     Scalability
     5     **A**     High Availability
     6     **A**     Reliability
     7     **B**     Predictability
     8     **C**     Public Cloud
     9     **B**     Private Cloud
    10     **A**     Hybrid Cloud
    11     **C**     Multi-Cloud
    12     **C**     IaaS
    13     **B**     Azure Virtual Machines
    14     **B**     PaaS
    15     **A**     Azure App Service
    16     **C**     Microsoft 365 / SaaS
    17     **A**     Azure Functions / Serverless
    18     **B**     Azure SQL Database / PaaS
    19     **B**     Azure Region
    20     **B**     Availability Zone
    21     **A**     Availability Zones
    22     **C**     Region Pair
    23     **A**     Availability Set
    24     **A**     Fault Domain
    25     **A**     Update Domain
    26     **B**     Resource Hierarchy
    27     **C**     Resource Group
    28     **B**     Subscription
    29     **D**     Management Group
    30     **A**     Resource
    31     **C**     Resource Group deletion
    32     **B**     Resource Group
    33     **A**     Azure Resource Manager
    34     **B**     ARM Template
    35     **B**     Infrastructure as Code
    36     **C**     ARM Template resources
    37     **A**     ARM Template parameters
    38     **A**     ARM Template benefits
    39     **B**     Azure Arc
    40  **A and B**  Azure Arc

------------------------------------------------------------------------

# 🧠 Explanations

## Questions 1--7 --- Cloud Economics and Benefits

### 1. B --- CapEx

**CapEx** is upfront spending used to purchase long-term assets such as
physical servers and networking equipment.

``` text
CapEx = BUY IT
```

------------------------------------------------------------------------

### 2. C --- Consumption-Based Pricing

Consumption-based pricing means paying for resources or services based
on usage.

``` text
Consumption = PAY FOR WHAT YOU USE
```

------------------------------------------------------------------------

### 3. B --- OpEx

**OpEx** is ongoing operational spending for services as they are
consumed.

``` text
CapEx = Upfront
OpEx  = Ongoing
```

------------------------------------------------------------------------

### 4. B --- Scalability

Scalability is the ability to adjust resources or capacity to meet
changing demand.

------------------------------------------------------------------------

### 5. A --- High Availability

High Availability focuses on keeping services accessible despite
disruptions.

``` text
High Availability = KEEP IT AVAILABLE
```

------------------------------------------------------------------------

### 6. A --- Reliability

Reliability focuses on recovering from failures and continuing to
operate.

``` text
Reliability = RECOVER AND CONTINUE
```

------------------------------------------------------------------------

### 7. B --- Predictability

Predictability helps organizations anticipate cloud performance and
costs.

------------------------------------------------------------------------

# Questions 8--11 --- Cloud Models

### 8. C --- Public Cloud

Public Cloud resources are provided by a third-party cloud provider.

------------------------------------------------------------------------

### 9. B --- Private Cloud

A Private Cloud environment is dedicated to one organization.

------------------------------------------------------------------------

### 10. A --- Hybrid Cloud

Hybrid Cloud combines public cloud and private/on-premises environments.

``` text
Hybrid = PUBLIC + PRIVATE
```

------------------------------------------------------------------------

### 11. C --- Multi-Cloud

Multi-Cloud means using services from multiple cloud providers.

``` text
Hybrid = MIX OF PUBLIC + PRIVATE
Multi  = MULTIPLE CLOUD PROVIDERS
```

------------------------------------------------------------------------

# Questions 12--18 --- Cloud Service Models

### 12. C --- IaaS

Of IaaS, PaaS, and SaaS, **IaaS** gives the customer the most management
responsibility.

``` text
MORE CUSTOMER MANAGEMENT

IaaS
 ↓
PaaS
 ↓
SaaS

LESS CUSTOMER MANAGEMENT
```

------------------------------------------------------------------------

### 13. B --- Azure Virtual Machines

Azure Virtual Machines are used in the lessons as the primary example of
**IaaS**.

------------------------------------------------------------------------

### 14. B --- PaaS

PaaS provides a managed platform so developers can focus more on
applications and data instead of the underlying infrastructure.

------------------------------------------------------------------------

### 15. A --- Azure App Service

Azure App Service is used as an example of **PaaS**.

------------------------------------------------------------------------

### 16. C --- Microsoft 365

Microsoft 365 is used as the example of **SaaS**: finished software
consumed by the customer.

------------------------------------------------------------------------

### 17. A --- Serverless / Function as a Service

Azure Functions is a serverless compute service commonly described as
**Function as a Service (FaaS)**.

------------------------------------------------------------------------

### 18. B --- PaaS

The Week 1 material classifies Azure SQL Database as **PaaS**.

### Quick Memory Table

  Service                  Model
  ------------------------ -----------------------
  Azure Virtual Machines   **IaaS**
  Azure App Service        **PaaS**
  Azure SQL Database       **PaaS**
  Azure Functions          **Serverless / FaaS**
  Microsoft 365            **SaaS**

------------------------------------------------------------------------

# Questions 19--25 --- Azure Architecture

### 19. B --- Azure Region

An Azure Region is a geographic area containing Azure datacenters.

------------------------------------------------------------------------

### 20. B --- Availability Zone

An Availability Zone is a physically separate location **inside an Azure
Region**.

``` text
Azure Region
    |
    +-- Zone 1
    +-- Zone 2
    +-- Zone 3
```

------------------------------------------------------------------------

### 21. A --- Availability Zones

Availability Zones provide physical separation inside a region and are
used for protection from location/datacenter-level failures within that
region.

------------------------------------------------------------------------

### 22. C --- Region Pair

Region Pairs are associated with region-to-region resiliency and
disaster-recovery planning.

``` text
Region Pair = REGION ↔ REGION
```

------------------------------------------------------------------------

### 23. A --- Availability Set

Availability Sets use:

-   Fault Domains
-   Update Domains

------------------------------------------------------------------------

### 24. A --- Fault Domain

Fault Domains separate VMs based on underlying hardware dependencies
such as power and networking.

``` text
Fault = HARDWARE FAILURE
```

------------------------------------------------------------------------

### 25. A --- Update Domain

Update Domains separate VMs into groups so planned maintenance does not
affect all VMs simultaneously.

``` text
Update = PLANNED MAINTENANCE
```

------------------------------------------------------------------------

# Questions 26--32 --- Azure Resource Hierarchy

### 26. B

The hierarchy is:

``` text
Management Group
       ↓
Subscription
       ↓
Resource Group
       ↓
Resource
```

------------------------------------------------------------------------

### 27. C --- Resource Group

A Resource Group is a logical container for related Azure resources.

------------------------------------------------------------------------

### 28. B --- Subscription

A Subscription acts as a billing and management boundary.

------------------------------------------------------------------------

### 29. D --- Management Group

Management Groups organize and help govern multiple Azure subscriptions.

------------------------------------------------------------------------

### 30. A --- Resource

An individual Azure service or asset, such as a Virtual Machine, is a
**Resource**.

------------------------------------------------------------------------

### 31. C --- The Resources Are Deleted

Deleting a Resource Group deletes the resources contained inside it.

> \[!CAUTION\] This is also important in real Azure administration.
> Always inspect a Resource Group before deleting it.

------------------------------------------------------------------------

### 32. B --- Logical Container

A Resource Group is a logical container. Resources within the same
Resource Group do not all have to exist in the same Azure Region.

### Hierarchy Memory Trick

``` text
Management Group = GOVERN SUBSCRIPTIONS
Subscription     = BILLING / MANAGEMENT
Resource Group   = CONTAINER
Resource         = ACTUAL SERVICE
```

------------------------------------------------------------------------

# Questions 33--40 --- ARM, IaC, and Azure Arc

### 33. A --- Azure's Management and Deployment Layer

Azure Resource Manager is Azure's management and deployment layer for
Azure resources.

``` text
ARM = MANAGE AZURE
```

------------------------------------------------------------------------

### 34. B --- JSON File

An ARM Template is a JSON file that defines Azure resources and their
configurations.

------------------------------------------------------------------------

### 35. B --- Manage Infrastructure Using Code

Infrastructure as Code means provisioning and managing infrastructure
using code rather than relying only on manual graphical configuration.

``` text
IaC = INFRASTRUCTURE DEFINED AS CODE
```

------------------------------------------------------------------------

### 36. C --- resources

The `resources` section defines the Azure resources that the template
should deploy.

------------------------------------------------------------------------

### 37. A --- parameters

The `parameters` section provides customizable inputs that can be
supplied during deployment.

### ARM Template Quick Reference

``` text
parameters = INPUT
variables  = REUSABLE VALUES
resources  = CREATE
outputs    = RETURN
```

------------------------------------------------------------------------

### 38. A --- Repeatable and Consistent Deployments

ARM Templates allow infrastructure to be deployed consistently,
repeatedly, and automatically.

------------------------------------------------------------------------

### 39. B --- Extend Azure Management Beyond Azure

Azure Arc extends Azure management and governance capabilities to
supported resources outside Azure.

``` text
ARM = MANAGE AZURE
ARC = EXTEND AZURE
```

------------------------------------------------------------------------

### 40. A and B --- On-Premises Datacenters and Other Cloud Providers

Lesson 6 describes Azure Arc as managing supported resources in
locations including:

-   On-premises datacenters
-   Other cloud providers
-   Edge locations

------------------------------------------------------------------------

# 📊 Review Your Results

Count the questions you missed by category:

  Area                         Questions     Missed
  ---------------------------- ----------- ----------
  Cloud Economics & Benefits   1--7         \_\_\_\_
  Cloud Models                 8--11        \_\_\_\_
  Service Models               12--18       \_\_\_\_
  Azure Architecture           19--25       \_\_\_\_
  Resource Hierarchy           26--32       \_\_\_\_
  ARM, IaC & Azure Arc         33--40       \_\_\_\_

Your weakest category should be the **first area you review**.

------------------------------------------------------------------------

# 🎯 What to Review

``` text
Missed 1–7
→ Review Lesson 1

Missed 8–11
→ Review Lesson 2

Missed 12–18
→ Review Lesson 3

Missed 19–25
→ Review Lesson 4

Missed 26–32
→ Review Lesson 5

Missed 33–40
→ Review Lesson 6
```

------------------------------------------------------------------------

# 🏁 Final Check

Before moving on, make sure you can explain these without looking at
your notes:

``` text
CapEx vs. OpEx
Public vs. Private vs. Hybrid vs. Multi-Cloud
High Availability vs. Scalability
Reliability vs. Predictability
IaaS vs. PaaS vs. SaaS
Region vs. Availability Zone vs. Region Pair
Fault Domain vs. Update Domain
Management Group → Subscription → Resource Group → Resource
ARM vs. ARM Template
Infrastructure as Code
ARM vs. Azure Arc
```

If you can explain **why** each correct answer is right---not just
memorize the letter---you are ready to continue.
