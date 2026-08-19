[practice-exam-2.md](https://github.com/user-attachments/files/31232326/practice-exam-2.md)
 
# AZ-900 Practice Exam 2 --- Lessons 8--14

This practice exam covers the concepts introduced in **Lessons 8--14**.

### Topics Covered

-   Azure compute services
-   Azure networking
-   Azure Storage and storage redundancy
-   Azure SQL Database and Azure Cosmos DB
-   Azure Database Migration Service
-   Core Azure solutions: IoT, analytics, and AI
-   Azure management tools
-   Microsoft Entra ID and identity foundations
-   Azure RBAC, Conditional Access, MFA, SSO, and Least Privilege

> \[!IMPORTANT\] Try to complete the exam without using your lesson
> notes, glossary, cram sheet, comparison tables, or answer key.

------------------------------------------------------------------------

# 📋 Instructions

-   **40 questions**
-   Choose the **best answer** unless the question says **Choose two**.
-   Suggested time: **45--60 minutes**
-   Suggested passing target: **80%**
-   Each question is worth **1 point**.
-   Maximum score: **40 points**

``` text
36–40 = Excellent
32–35 = Ready to move forward
28–31 = Review weak areas
 0–27 = Revisit Lessons 8–14
```

------------------------------------------------------------------------

# Questions

## 1.

A company needs a cloud-based Windows computer and wants control over
the operating system.

Which Azure service is the best fit?

A. Azure App Service\
B. Azure Virtual Machine\
C. Azure Functions\
D. Azure Container Instances

------------------------------------------------------------------------

## 2.

A website runs on multiple similar virtual machines. The company wants
the number of VM instances to automatically increase when demand rises.

Which service should it use?

A. Azure Virtual Machine Scale Sets\
B. Azure Logic Apps\
C. Azure Files\
D. Azure Cosmos DB

------------------------------------------------------------------------

## 3.

A development team wants to host a web application without managing the
underlying web servers.

Which service is the best fit?

A. Azure Virtual Machines\
B. Azure App Service\
C. Azure Kubernetes Service\
D. Azure Virtual Network

------------------------------------------------------------------------

## 4.

Code should run automatically whenever a file is uploaded to storage.

Which service best fits this requirement?

A. Azure Functions\
B. Azure Virtual Machines\
C. Azure Files\
D. Azure Advisor

------------------------------------------------------------------------

## 5.

A company wants to run a container quickly without managing a Kubernetes
cluster.

Which Azure service should it choose?

A. Azure Kubernetes Service\
B. Azure Container Instances\
C. Virtual Machine Scale Sets\
D. Azure App Service

------------------------------------------------------------------------

## 6.

A company has a large containerized application that requires Kubernetes
orchestration.

Which Azure service is designed for this requirement?

A. Azure Container Instances\
B. Azure Kubernetes Service\
C. Azure Functions\
D. Azure Files

------------------------------------------------------------------------

## 7.

Which pairing is correct?

A. Azure Virtual Machines --- PaaS\
B. Azure App Service --- IaaS\
C. Azure Functions --- Serverless\
D. Azure Kubernetes Service --- SaaS

------------------------------------------------------------------------

## 8.

What is an Azure **Virtual Network (VNet)**?

A. A managed relational database\
B. A private network in Azure\
C. A storage redundancy option\
D. A cloud identity directory

------------------------------------------------------------------------

## 9.

What is a **subnet**?

A. A smaller network inside a VNet\
B. A second Azure Region\
C. A public internet address\
D. A storage container

------------------------------------------------------------------------

## 10.

Which Azure networking feature filters inbound and outbound network
traffic using security rules?

A. Azure DNS\
B. Network Security Group\
C. Azure Advisor\
D. Azure Files

------------------------------------------------------------------------

## 11.

An Azure resource must be reachable over the public internet.

Which concept best matches this requirement?

A. Private Endpoint\
B. Public Endpoint\
C. Table Storage\
D. Azure RBAC

------------------------------------------------------------------------

## 12.

A company wants private connectivity to a supported Azure service using
a private IP address in its VNet.

Which concept should it use?

A. Public IP Address\
B. Public Endpoint\
C. Private Endpoint\
D. Azure DNS

------------------------------------------------------------------------

## 13.

Which Azure service translates domain names into IP addresses?

A. Azure DNS\
B. Azure Monitor\
C. Azure Arc\
D. Azure DevOps

------------------------------------------------------------------------

## 14.

A company needs to store images, videos, backups, and other unstructured
objects.

Which storage service is the best fit?

A. Queue Storage\
B. Azure Files\
C. Blob Storage\
D. Table Storage

------------------------------------------------------------------------

## 15.

A company needs managed shared file shares that can support protocols
such as SMB or NFS.

Which service should it use?

A. Azure Files\
B. Blob Storage\
C. Queue Storage\
D. Azure Cosmos DB

------------------------------------------------------------------------

## 16.

An application needs to place messages into a backlog so another
application component can process them later.

Which storage service should it use?

A. Azure Files\
B. Queue Storage\
C. Blob Storage\
D. Azure SQL Database

------------------------------------------------------------------------

## 17.

Which Azure Storage service is designed for structured, non-relational
key/attribute data?

A. Table Storage\
B. Azure Files\
C. Blob Storage\
D. Queue Storage

------------------------------------------------------------------------

## 18.

Which Azure database service is a managed **relational** database?

A. Azure Cosmos DB\
B. Azure SQL Database\
C. Table Storage\
D. Blob Storage

------------------------------------------------------------------------

## 19.

A globally distributed application requires a managed NoSQL database
with low-latency access.

Which service best fits this requirement?

A. Azure SQL Database\
B. Azure Cosmos DB\
C. Azure Files\
D. Azure Database Migration Service

------------------------------------------------------------------------

## 20.

Which storage redundancy option replicates data across Availability
Zones within the primary Azure Region?

A. LRS\
B. ZRS\
C. GRS\
D. GZRS only

------------------------------------------------------------------------

## 21.

Which storage redundancy option adds replication to a secondary
geographic region?

A. LRS\
B. ZRS\
C. GRS\
D. Table Storage

------------------------------------------------------------------------

## 22.

Which redundancy option combines Availability Zone redundancy in the
primary region with replication to another region?

A. LRS\
B. ZRS\
C. GRS\
D. GZRS

------------------------------------------------------------------------

## 23.

A company wants help moving an existing database into Azure.

Which service from Lesson 10 is designed for this purpose?

A. Azure Database Migration Service\
B. Azure Monitor\
C. Azure Advisor\
D. Azure IoT Hub

------------------------------------------------------------------------

## 24.

A company needs secure two-way communication between large numbers of
IoT devices and Azure.

Which service should it use?

A. Azure IoT Hub\
B. Azure Synapse Analytics\
C. Azure Machine Learning\
D. Azure Repos

------------------------------------------------------------------------

## 25.

Which service combines data integration, data warehousing, and big-data
analytics?

A. Azure Synapse Analytics\
B. Azure Functions\
C. Azure DNS\
D. Microsoft Entra ID

------------------------------------------------------------------------

## 26.

A company needs to move, transform, and automate data between different
data sources using pipelines.

Which service best fits this requirement?

A. Azure Data Factory\
B. Azure IoT Hub\
C. Azure Advisor\
D. Azure Files

------------------------------------------------------------------------

## 27.

A developer wants to add capabilities such as vision, speech, language,
translation, or document processing without building the AI capabilities
from scratch.

Which offering best matches the Lesson 11 material?

A. Azure AI Services\
B. Azure Virtual Network\
C. Azure Resource Manager\
D. Azure Files

------------------------------------------------------------------------

## 28.

A data science team wants a platform for building, training, deploying,
and managing machine learning models.

Which service should it use?

A. Azure Machine Learning\
B. Azure Monitor\
C. Azure App Service\
D. Azure DNS

------------------------------------------------------------------------

## 29.

An administrator wants to collect and analyze metrics, logs, and
telemetry from Azure resources.

Which service should be used?

A. Azure Advisor\
B. Azure Monitor\
C. Azure Service Health\
D. Azure Boards

------------------------------------------------------------------------

## 30.

An administrator wants personalized recommendations for improving cost,
reliability, security, performance, and operational excellence.

Which service should be used?

A. Azure Monitor\
B. Azure Service Health\
C. Azure Advisor\
D. Azure Functions

------------------------------------------------------------------------

## 31.

An administrator wants to know whether an Azure service incident or
planned maintenance is affecting the organization's environment.

Which service should be used?

A. Azure Advisor\
B. Azure Service Health\
C. Azure Monitor\
D. Azure Repos

------------------------------------------------------------------------

## 32.

Which Azure DevOps service provides Git repositories for source-code
management?

A. Azure Boards\
B. Azure Repos\
C. Azure Pipelines\
D. Azure Test Plans

------------------------------------------------------------------------

## 33.

Which Azure DevOps service provides CI/CD automation for building,
testing, and deploying applications?

A. Azure Boards\
B. Azure Repos\
C. Azure Pipelines\
D. Azure Artifacts

------------------------------------------------------------------------

## 34.

What is the primary purpose of **Microsoft Entra ID**?

A. Cloud identity and access management\
B. Object storage\
C. Network traffic filtering\
D. VM autoscaling

------------------------------------------------------------------------

## 35.

A user enters credentials to prove who they are.

Which identity concept is being demonstrated?

A. Authorization\
B. Authentication\
C. Azure RBAC\
D. Least Privilege

------------------------------------------------------------------------

## 36.

Azure determines what an authenticated user is allowed to do with a
resource.

Which concept is being demonstrated?

A. Authentication\
B. Authorization\
C. Single Sign-On\
D. Azure DNS

------------------------------------------------------------------------

## 37.

A user should be able to view Azure resources but should not be able to
modify them.

Which built-in Azure RBAC role best fits this requirement?

A. Owner\
B. Contributor\
C. Reader\
D. Administrator

------------------------------------------------------------------------

## 38.

A policy says: **If an administrator signs in under configured risky
conditions, require an additional authentication control.**

Which feature is designed to apply this type of if-then access decision?

A. Single Sign-On\
B. Conditional Access\
C. Azure Monitor\
D. Azure Advisor

------------------------------------------------------------------------

## 39.

A user signs in with a password and then approves a notification on a
phone.

Which security feature is being used?

A. Single Sign-On\
B. Multi-Factor Authentication\
C. Azure RBAC\
D. Azure Arc

------------------------------------------------------------------------

## 40. Choose two.

Which **TWO** statements are correct?

A. Single Sign-On allows a user to sign in once and access multiple
authorized applications.\
B. Least Privilege means users should receive only the permissions
required for their tasks.\
C. Single Sign-On means every user receives Owner permissions.\
D. Least Privilege means all authenticated users should receive the same
permissions.

------------------------------------------------------------------------

# 🛑 Stop Here

Do not open `answer-key-2.md` until you have completed all 40 questions.

Record your answers:

``` text
 1. ____    11. ____    21. ____    31. ____
 2. ____    12. ____    22. ____    32. ____
 3. ____    13. ____    23. ____    33. ____
 4. ____    14. ____    24. ____    34. ____
 5. ____    15. ____    25. ____    35. ____
 6. ____    16. ____    26. ____    36. ____
 7. ____    17. ____    27. ____    37. ____
 8. ____    18. ____    28. ____    38. ____
 9. ____    19. ____    29. ____    39. ____
10. ____    20. ____    30. ____    40. ____
```

When finished, compare your answers with **`answer-key-2.md`**.
