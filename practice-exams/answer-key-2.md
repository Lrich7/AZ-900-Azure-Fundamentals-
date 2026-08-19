[answer-key-2.md](https://github.com/user-attachments/files/31232336/answer-key-2.md)

# AZ-900 Practice Exam 2 --- Answer Key

Answer key for **Practice Exam 2 --- Lessons 8--14**.

> \[!TIP\] Review the explanation for every question you missed **or
> guessed on**. A correct guess can still reveal a topic that needs
> review.

------------------------------------------------------------------------

# 📊 Score Guide

  Score          Percentage Recommendation
  ------------ ------------ ----------------------------
  **36--40**       90--100% Excellent --- move forward
  **32--35**      80--87.5% Ready to move forward
  **28--31**      70--77.5% Review weak areas
  **0--27**       Below 70% Revisit Lessons 8--14

> \[!NOTE\] This score guide is for this training repository. It is not
> Microsoft's official AZ-900 exam scoring system.

------------------------------------------------------------------------

# ✅ Answer Key

    \#    Answer     Topic
  ---- ------------- ----------------------------
     1     **B**     Virtual Machines
     2     **A**     VM Scale Sets
     3     **B**     App Service
     4     **A**     Azure Functions
     5     **B**     ACI
     6     **B**     AKS
     7     **C**     Compute models
     8     **B**     Virtual Network
     9     **A**     Subnet
    10     **B**     NSG
    11     **B**     Public Endpoint
    12     **C**     Private Endpoint
    13     **A**     Azure DNS
    14     **C**     Blob Storage
    15     **A**     Azure Files
    16     **B**     Queue Storage
    17     **A**     Table Storage
    18     **B**     Azure SQL Database
    19     **B**     Azure Cosmos DB
    20     **B**     ZRS
    21     **C**     GRS
    22     **D**     GZRS
    23     **A**     Database Migration Service
    24     **A**     Azure IoT Hub
    25     **A**     Azure Synapse Analytics
    26     **A**     Azure Data Factory
    27     **A**     Azure AI Services
    28     **A**     Azure Machine Learning
    29     **B**     Azure Monitor
    30     **C**     Azure Advisor
    31     **B**     Azure Service Health
    32     **B**     Azure Repos
    33     **C**     Azure Pipelines
    34     **A**     Microsoft Entra ID
    35     **B**     Authentication
    36     **B**     Authorization
    37     **C**     Reader
    38     **B**     Conditional Access
    39     **B**     MFA
    40  **A and B**  SSO / Least Privilege

------------------------------------------------------------------------

# 🧠 Explanations

## Questions 1--7 --- Lesson 8: Compute

### 1. B --- Azure Virtual Machine

A Virtual Machine provides a software-based computer in Azure and gives
the customer control over the guest operating system.

``` text
VM = VIRTUAL COMPUTER
```

------------------------------------------------------------------------

### 2. A --- Virtual Machine Scale Sets

VM Scale Sets manage groups of virtual machines and can automatically
scale the number of instances based on demand or schedules.

``` text
VM   = INDIVIDUAL VIRTUAL COMPUTER
VMSS = GROUP + SCALE
```

------------------------------------------------------------------------

### 3. B --- Azure App Service

Azure App Service is a managed platform for hosting web applications.

``` text
App Service = MANAGED WEB APP
```

------------------------------------------------------------------------

### 4. A --- Azure Functions

Azure Functions runs event-driven serverless code. Lesson 8 describes
triggers such as HTTP requests, timers, queues, and storage updates.

``` text
Functions = EVENT-DRIVEN CODE
```

------------------------------------------------------------------------

### 5. B --- Azure Container Instances

ACI is the better fit when you need to run a container without managing
Kubernetes.

``` text
ACI = RUN CONTAINER
```

------------------------------------------------------------------------

### 6. B --- Azure Kubernetes Service

AKS provides managed Kubernetes for container orchestration.

``` text
AKS = ORCHESTRATE CONTAINERS
```

------------------------------------------------------------------------

### 7. C --- Azure Functions --- Serverless

The Lesson 8 quick reference identifies:

  Service                  Model
  ------------------------ --------------------
  Azure Virtual Machines   IaaS
  VM Scale Sets            IaaS
  Azure App Service        PaaS
  Azure Functions          Serverless / FaaS
  ACI                      Container Service
  AKS                      Managed Kubernetes

------------------------------------------------------------------------

# Questions 8--13 --- Lesson 9: Networking

### 8. B --- Virtual Network

A VNet is Azure's private network for Azure resources.

------------------------------------------------------------------------

### 9. A --- Subnet

A subnet is a smaller network segment inside a VNet.

``` text
VNet   = PRIVATE NETWORK
Subnet = PART OF A VNET
```

------------------------------------------------------------------------

### 10. B --- Network Security Group

NSGs use security rules to filter inbound and outbound network traffic.

``` text
NSG = ALLOW / DENY TRAFFIC RULES
```

------------------------------------------------------------------------

### 11. B --- Public Endpoint

A Public Endpoint allows a resource to be accessed over a public network
path.

------------------------------------------------------------------------

### 12. C --- Private Endpoint

A Private Endpoint provides private connectivity using a private IP
address within a VNet.

``` text
Public Endpoint  = PUBLIC PATH
Private Endpoint = PRIVATE VNET PATH
```

------------------------------------------------------------------------

### 13. A --- Azure DNS

Azure DNS hosts DNS records and translates domain names into IP
addresses.

``` text
DNS = NAME → IP ADDRESS
```

------------------------------------------------------------------------

# Questions 14--23 --- Lesson 10: Storage

### 14. C --- Blob Storage

Blob Storage is designed for object/unstructured data such as images,
video, documents, and backups.

------------------------------------------------------------------------

### 15. A --- Azure Files

Azure Files provides managed file shares and supports file-sharing
protocols such as SMB and NFS.

------------------------------------------------------------------------

### 16. B --- Queue Storage

Queue Storage stores messages that application components can process
asynchronously.

------------------------------------------------------------------------

### 17. A --- Table Storage

Table Storage provides structured, non-relational key/attribute storage.

### Storage Memory Trick

``` text
BLOB  = OBJECTS
FILES = FILE SHARES
QUEUE = MESSAGES
TABLE = NoSQL KEY/ATTRIBUTE DATA
```

------------------------------------------------------------------------

### 18. B --- Azure SQL Database

Azure SQL Database is the managed relational database option covered in
Lesson 10.

``` text
SQL = RELATIONAL
```

------------------------------------------------------------------------

### 19. B --- Azure Cosmos DB

Azure Cosmos DB is the globally distributed NoSQL database covered in
the lesson.

``` text
Cosmos DB = GLOBAL NoSQL
```

------------------------------------------------------------------------

### 20. B --- ZRS

ZRS stores copies across Availability Zones in the primary Azure Region.

------------------------------------------------------------------------

### 21. C --- GRS

GRS adds replication to a secondary geographic region.

------------------------------------------------------------------------

### 22. D --- GZRS

GZRS combines zone redundancy in the primary region with replication to
another region.

``` text
LRS  = LOCAL
ZRS  = ZONES
GRS  = GEOGRAPHIC
GZRS = ZONES + GEOGRAPHIC
```

------------------------------------------------------------------------

### 23. A --- Azure Database Migration Service

Azure Database Migration Service helps move supported database workloads
into Azure.

------------------------------------------------------------------------

# Questions 24--28 --- Lesson 11: Core Azure Solutions

### 24. A --- Azure IoT Hub

Azure IoT Hub securely connects, monitors, and manages IoT devices and
supports two-way communication between devices and Azure.

------------------------------------------------------------------------

### 25. A --- Azure Synapse Analytics

The Lesson 11 material describes Azure Synapse Analytics as combining
data integration, data warehousing, and big-data analytics.

------------------------------------------------------------------------

### 26. A --- Azure Data Factory

Azure Data Factory is used to move, transform, and automate data between
sources using data pipelines.

``` text
Data Factory = MOVE / TRANSFORM DATA
```

------------------------------------------------------------------------

### 27. A --- Azure AI Services

The lesson describes Azure AI Services as prebuilt AI capabilities for
areas such as vision, speech, language, translation, and document
processing.

------------------------------------------------------------------------

### 28. A --- Azure Machine Learning

Azure Machine Learning provides tools for building, training, deploying,
and managing machine learning models.

``` text
AI Services      = PREBUILT AI CAPABILITIES
Machine Learning = BUILD / TRAIN / DEPLOY MODELS
```

------------------------------------------------------------------------

# Questions 29--33 --- Lesson 12: Management Tools

### 29. B --- Azure Monitor

Azure Monitor collects and analyzes monitoring data such as metrics,
logs, telemetry, and application traces.

``` text
Monitor = WHAT IS HAPPENING?
```

------------------------------------------------------------------------

### 30. C --- Azure Advisor

Azure Advisor analyzes configurations and usage and provides
personalized recommendations.

``` text
Advisor = WHAT SHOULD I IMPROVE?
```

------------------------------------------------------------------------

### 31. B --- Azure Service Health

Azure Service Health provides information about Azure service issues,
planned maintenance, and advisories relevant to your environment.

``` text
Service Health = IS AZURE HAVING A PROBLEM?
```

### High-Value Comparison

``` text
Monitor        = OBSERVE
Advisor        = RECOMMEND
Service Health = AZURE PLATFORM HEALTH
```

------------------------------------------------------------------------

### 32. B --- Azure Repos

Azure Repos provides Git repositories for source-code management.

------------------------------------------------------------------------

### 33. C --- Azure Pipelines

Azure Pipelines provides build and release automation / CI/CD.

### Azure DevOps Quick Reference

``` text
Boards    = TRACK WORK
Repos     = SOURCE CODE
Pipelines = BUILD / TEST / DEPLOY
```

------------------------------------------------------------------------

# Questions 34--40 --- Lessons 13--14: Identity and Access

### 34. A --- Microsoft Entra ID

Microsoft Entra ID provides cloud identity and access management.

``` text
Entra ID = IDENTITY
```

------------------------------------------------------------------------

### 35. B --- Authentication

Authentication verifies identity.

``` text
Authentication = WHO ARE YOU?
```

------------------------------------------------------------------------

### 36. B --- Authorization

Authorization determines what an authenticated identity is allowed to
do.

``` text
Authorization = WHAT CAN YOU DO?
```

------------------------------------------------------------------------

### 37. C --- Reader

The Week 2 material identifies **Reader** as the built-in role for
viewing resources without modifying them.

``` text
Reader      = VIEW
Contributor = MANAGE RESOURCES
Owner       = MANAGE + ROLE ASSIGNMENTS
```

------------------------------------------------------------------------

### 38. B --- Conditional Access

Conditional Access applies access rules based on configured conditions.

``` text
Conditional Access = IF / THEN
```

------------------------------------------------------------------------

### 39. B --- Multi-Factor Authentication

MFA requires multiple factors to verify identity. The lesson uses a
password plus phone approval as an example.

``` text
MFA = VERIFY MORE
```

------------------------------------------------------------------------

### 40. A and B --- SSO and Least Privilege

**Single Sign-On** allows a user to authenticate once and access
multiple authorized applications.

**Least Privilege** means granting only the minimum permissions required
to perform a task.

``` text
SSO             = SIGN IN ONCE
Least Privilege = ONLY WHAT YOU NEED
```

------------------------------------------------------------------------

# 📊 Review Your Results

Count the questions you missed by lesson:

  Lesson       Area                   Questions     Missed
  ------------ ---------------------- ----------- ----------
  **8**        Compute                1--7         \_\_\_\_
  **9**        Networking             8--13        \_\_\_\_
  **10**       Storage & Databases    14--23       \_\_\_\_
  **11**       Core Azure Solutions   24--28       \_\_\_\_
  **12**       Management Tools       29--33       \_\_\_\_
  **13--14**   Identity & Access      34--40       \_\_\_\_

Your weakest category should be the **first area you review**.

------------------------------------------------------------------------

# 🎯 What to Review

``` text
Missed 1–7
→ Review Lesson 8

Missed 8–13
→ Review Lesson 9

Missed 14–23
→ Review Lesson 10

Missed 24–28
→ Review Lesson 11

Missed 29–33
→ Review Lesson 12

Missed 34–40
→ Review Lessons 13–14
```

------------------------------------------------------------------------

# 🏁 Final Check

Before moving on, make sure you can explain these without looking at
your notes:

``` text
VM vs. VM Scale Set
App Service vs. Functions
ACI vs. AKS

VNet vs. Subnet
Public Endpoint vs. Private Endpoint
Purpose of an NSG

Blob vs. Files vs. Queue vs. Table
Azure SQL Database vs. Cosmos DB
LRS vs. ZRS vs. GRS vs. GZRS

IoT Hub
Synapse Analytics
Data Factory
Azure AI Services vs. Azure Machine Learning

Monitor vs. Advisor vs. Service Health
Boards vs. Repos vs. Pipelines

Authentication vs. Authorization
Entra ID vs. RBAC
Reader vs. Contributor vs. Owner
Conditional Access vs. MFA
SSO
Least Privilege
```

If you can explain **why** each correct answer is right and why the
competing services do not fit, you are ready to continue.
