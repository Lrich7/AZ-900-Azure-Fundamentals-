[glossary.md](https://github.com/user-attachments/files/31230322/glossary.md)

# AZ-900 Glossary

A quick-reference glossary for the major terms, services, and concepts
covered throughout this AZ-900 training course.

> \[!TIP\] Use this page when you recognize a term but cannot quite
> remember what it means. For side-by-side differences, use
> `comparison-table.md`. For rapid review, use `cram-sheet.md`.

------------------------------------------------------------------------

# A

## Authentication

The process of verifying **who a user or identity is**.

**Remember:**\
\> **Authentication = Who are you?**

------------------------------------------------------------------------

## Authorization

The process of determining **what an authenticated identity is allowed
to do**.

**Remember:**\
\> **Authorization = What can you do?**

------------------------------------------------------------------------

## Availability

The ability of a service or resource to remain accessible and
operational when needed.

------------------------------------------------------------------------

## Availability Set

A logical grouping of virtual machines designed to help protect against
hardware failures and planned maintenance using **fault domains** and
**update domains**.

**Remember:**\
\> **Availability Set = logical VM protection.**

------------------------------------------------------------------------

## Availability Zone

A physically separate location within an Azure region with independent
infrastructure such as power, cooling, and networking.

**Remember:**\
\> **Availability Zone = separate location inside one region.**

------------------------------------------------------------------------

## Azure Advisor

An Azure service that provides personalized recommendations to help
improve areas such as cost, reliability, security, performance, and
operational excellence.

**Remember:**\
\> **Advisor = What should I improve?**

------------------------------------------------------------------------

## Azure App Service

A managed platform for hosting web applications, APIs, and related
application workloads without managing the underlying servers.

**Remember:**\
\> **App Service = managed web app hosting.**

------------------------------------------------------------------------

## Azure Arc

A service that extends Azure management and governance capabilities to
supported resources outside Azure, including on-premises, edge, and
multicloud environments.

**Remember:**\
\> **Azure Arc = extend Azure management beyond Azure.**

------------------------------------------------------------------------

## Azure Blob Storage

Object storage designed for large amounts of unstructured data such as
images, video, documents, and backups.

**Remember:**\
\> **Blob = objects/unstructured data.**

------------------------------------------------------------------------

## Azure CLI

A command-line tool used to create and manage Azure resources.

------------------------------------------------------------------------

## Azure Container Instances (ACI)

A service for running containers in Azure without managing virtual
machines or a Kubernetes environment.

**Remember:**\
\> **ACI = run containers.**

------------------------------------------------------------------------

## Azure Cosmos DB

A globally distributed NoSQL database service.

**Remember:**\
\> **Cosmos DB = global NoSQL.**

------------------------------------------------------------------------

## Azure Cost Management

Tools for monitoring, analyzing, controlling, and optimizing cloud
spending.

**Remember:**\
\> **Cost Management = What are we spending?**

------------------------------------------------------------------------

## Azure DDoS Protection

An Azure networking security service designed to help protect resources
from Distributed Denial-of-Service attacks.

**Remember:**\
\> **DDoS Protection = traffic-flood protection.**

------------------------------------------------------------------------

## Azure Dedicated Host

A physical Azure server dedicated to a single customer for hosting
supported Azure virtual machines.

**Remember:**\
\> **Dedicated Host = dedicated physical server.**

------------------------------------------------------------------------

## Azure Files

Managed file shares that can be accessed using supported file-sharing
protocols such as SMB and NFS.

**Remember:**\
\> **Azure Files = managed file share.**

------------------------------------------------------------------------

## Azure Firewall

A managed, centralized network security service for controlling network
traffic.

**Remember:**\
\> **Azure Firewall = managed centralized firewall.**

------------------------------------------------------------------------

## Azure Functions

A serverless compute service designed to run code in response to events
or triggers.

**Remember:**\
\> **Functions = event-driven code.**

------------------------------------------------------------------------

## Azure Kubernetes Service (AKS)

A managed Kubernetes service used to deploy, manage, and orchestrate
containerized applications.

**Remember:**\
\> **AKS = orchestrate containers.**

------------------------------------------------------------------------

## Azure Marketplace

A catalog where customers can find Microsoft and third-party solutions
that run on or integrate with Azure.

**Remember:**\
\> **Marketplace = shop for Azure solutions.**

------------------------------------------------------------------------

## Azure Monitor

Azure's monitoring service for collecting and analyzing metrics, logs,
telemetry, and other monitoring data.

**Remember:**\
\> **Monitor = What is happening?**

------------------------------------------------------------------------

## Azure Policy

A governance service used to enforce organizational standards and
evaluate resource compliance.

**Remember:**\
\> **Policy = What is allowed or required?**

------------------------------------------------------------------------

## Azure Portal

The web-based graphical interface used to create, configure, monitor,
and manage Azure resources.

------------------------------------------------------------------------

## Azure Pricing Calculator

A tool used to estimate the expected cost of Azure services before
deployment.

**Remember:**\
\> **Pricing Calculator = What will Azure cost?**

------------------------------------------------------------------------

## Azure Queue Storage

A storage service used to store messages that application components can
process asynchronously.

**Remember:**\
\> **Queue = messages.**

------------------------------------------------------------------------

## Azure Region

A geographic area containing one or more Azure datacenters connected
through a low-latency network.

**Remember:**\
\> **Region = geographic Azure location.**

------------------------------------------------------------------------

## Azure Reservation

A purchasing option that can provide savings for eligible predictable
workloads in exchange for a commitment.

**Remember:**\
\> **Reservation = commit and save.**

------------------------------------------------------------------------

## Azure Resource Manager (ARM)

Azure's management and deployment layer for creating, updating,
organizing, and deleting Azure resources.

**Remember:**\
\> **ARM = manage Azure resources.**

------------------------------------------------------------------------

## Azure Service Health

A service that provides information about Azure service incidents,
planned maintenance, and health advisories relevant to your environment.

**Remember:**\
\> **Service Health = Is Azure having a problem?**

------------------------------------------------------------------------

## Azure SQL Database

A managed relational database service based on Microsoft SQL
technologies.

**Remember:**\
\> **Azure SQL Database = relational.**

------------------------------------------------------------------------

## Azure Spot Virtual Machines

Azure virtual machines that use available unused compute capacity at a
discount but can be evicted when Azure needs the capacity back.

**Remember:**\
\> **Spot = discounted + interruptible.**

------------------------------------------------------------------------

## Azure Storage

Azure services used to store data such as objects, files, messages, and
other data types.

------------------------------------------------------------------------

## Azure Table Storage

A NoSQL key/attribute data store for structured non-relational data.

**Remember:**\
\> **Table Storage = NoSQL key/attribute data.**

------------------------------------------------------------------------

## Azure Virtual Machine (VM)

An Infrastructure as a Service compute resource that provides a virtual
computer with control over the operating system and installed software.

**Remember:**\
\> **VM = virtual computer.**

------------------------------------------------------------------------

## Azure Virtual Machine Scale Sets (VMSS)

A service used to deploy and manage a group of load-balanced virtual
machines that can scale.

**Remember:**\
\> **VMSS = scale groups of VMs.**

------------------------------------------------------------------------

# B

## Bicep

A declarative language used to define and deploy Azure resources. It
provides a more concise authoring experience than traditional ARM
template JSON while deploying through Azure Resource Manager.

------------------------------------------------------------------------

# C

## Capital Expenditure (CapEx)

Money spent upfront to purchase or improve long-term assets such as
physical servers.

**Remember:**\
\> **CapEx = buy it.**

------------------------------------------------------------------------

## Cloud Computing

The delivery of computing services such as compute, storage, networking,
and applications over the internet.

------------------------------------------------------------------------

## Cloud Service Model

A model describing how management responsibilities are divided between
the cloud provider and customer.

Common models include:

-   IaaS
-   PaaS
-   SaaS

------------------------------------------------------------------------

## Composite SLA

The calculated availability of a solution that depends on multiple
services.

For dependent components, availability percentages may be multiplied.

``` text
99.9% × 99.9% = 99.8001%
```

------------------------------------------------------------------------

## Conditional Access

A Microsoft Entra capability that uses signals and configured policies
to make access decisions.

**Remember:**\
\> **Conditional Access = IF / THEN access policy.**

------------------------------------------------------------------------

# D

## Defense in Depth

A security strategy that uses multiple layers of protection so that if
one layer fails, additional layers remain.

**Remember:**\
\> **Defense in Depth = layers.**

------------------------------------------------------------------------

## Declarative

An approach where you describe the desired end state rather than
specifying every individual step required to reach it.

ARM templates are declarative.

**Remember:**\
\> **Declarative = describe what you want.**

------------------------------------------------------------------------

## Distributed Denial-of-Service (DDoS)

An attack that attempts to overwhelm a service or network with large
amounts of traffic.

------------------------------------------------------------------------

# E

## Elasticity

The ability to rapidly or automatically increase and decrease resources
as demand changes.

------------------------------------------------------------------------

## Encryption

The process of transforming data so that it cannot be easily read
without the appropriate key or authorization.

------------------------------------------------------------------------

# F

## Fault Domain

A grouping used by Availability Sets to help separate virtual machines
across underlying hardware dependencies.

**Remember:**\
\> **Fault Domain = hardware failure protection.**

------------------------------------------------------------------------

# G

## Generally Available (GA)

A service or feature that has reached general release.

**Remember:**\
\> **GA = generally released.**

------------------------------------------------------------------------

## Geo-Redundant Storage (GRS)

A storage redundancy option that replicates data to a secondary
geographic region in addition to maintaining copies in the primary
region.

**Remember:**\
\> **GRS = geographic redundancy.**

------------------------------------------------------------------------

## Geo-Zone-Redundant Storage (GZRS)

A storage redundancy option combining zone redundancy in the primary
region with geographic replication to a secondary region.

**Remember:**\
\> **GZRS = zones + geography.**

------------------------------------------------------------------------

## Governance

The policies, processes, and controls used to manage resources according
to organizational requirements.

------------------------------------------------------------------------

# H

## High Availability

Designing systems and services to remain available despite failures or
disruptions.

------------------------------------------------------------------------

## Hybrid Cloud

A cloud model combining public cloud services with private cloud or
on-premises infrastructure.

**Remember:**\
\> **Hybrid = mix.**

------------------------------------------------------------------------

# I

## Identity

A representation of a user, application, device, or other entity that
can be authenticated and authorized.

------------------------------------------------------------------------

## Infrastructure as a Service (IaaS)

A cloud service model where the provider manages the physical
infrastructure while the customer manages items such as the operating
system, applications, and data.

**Remember:**\
\> **IaaS = manage more.**

------------------------------------------------------------------------

## Infrastructure as Code (IaC)

The practice of defining and managing infrastructure through code or
configuration files rather than only through manual configuration.

**Remember:**\
\> **IaC = infrastructure defined as code.**

------------------------------------------------------------------------

# L

## Least Privilege

The security principle of granting only the minimum permissions required
to perform a task.

------------------------------------------------------------------------

## Locally Redundant Storage (LRS)

A storage redundancy option that keeps multiple copies of data within a
single physical location in the primary region.

**Remember:**\
\> **LRS = local.**

------------------------------------------------------------------------

# M

## Management Group

A level of the Azure resource hierarchy used to organize and apply
governance across multiple subscriptions.

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

## Microsoft Defender for Cloud

A cloud security service that provides security posture management and
workload protection capabilities.

**Remember:**\
\> **Defender for Cloud = security posture + workload protection.**

------------------------------------------------------------------------

## Microsoft Entra ID

Microsoft's cloud-based identity and access management service.

**Remember:**\
\> **Entra ID = identity.**

------------------------------------------------------------------------

## Microsoft Sentinel

A cloud-native security information and event management (SIEM) platform
used for security monitoring, detection, investigation, and response.

**Remember:**\
\> **Sentinel = SIEM.**

------------------------------------------------------------------------

## Multi-Cloud

The use of cloud services from more than one cloud provider.

**Remember:**\
\> **Multi-Cloud = multiple providers.**

------------------------------------------------------------------------

## Multi-Factor Authentication (MFA)

An authentication method that requires more than one factor to verify
identity.

**Remember:**\
\> **MFA = verify with multiple factors.**

------------------------------------------------------------------------

# N

## Network Security Group (NSG)

A networking feature containing security rules that allow or deny
inbound and outbound network traffic.

**Remember:**\
\> **NSG = allow/deny traffic rules.**

------------------------------------------------------------------------

## NoSQL

A broad category of non-relational database technologies designed for
data models that do not require a traditional relational table
structure.

------------------------------------------------------------------------

# O

## Operational Expenditure (OpEx)

Ongoing spending for services or resources as they are consumed.

**Remember:**\
\> **OpEx = use it / pay as you go.**

------------------------------------------------------------------------

# P

## Platform as a Service (PaaS)

A cloud service model where the cloud provider manages the underlying
infrastructure and platform so customers can focus primarily on
applications and data.

**Remember:**\
\> **PaaS = build without managing the underlying servers.**

------------------------------------------------------------------------

## PowerShell

A command-line shell and scripting language that can be used to automate
and manage Azure resources.

------------------------------------------------------------------------

## Private Cloud

A cloud environment dedicated to a single organization.

**Remember:**\
\> **Private Cloud = organization-dedicated environment.**

------------------------------------------------------------------------

## Private Endpoint

A network interface that uses a private IP address from a virtual
network to connect privately to a supported Azure service.

**Remember:**\
\> **Private Endpoint = private entrance to a service.**

------------------------------------------------------------------------

## Private Preview

An early service or feature preview available to a limited set of
participants.

------------------------------------------------------------------------

## Public Cloud

Cloud infrastructure operated by a cloud provider and offered to
customers over shared provider infrastructure.

**Remember:**\
\> **Public Cloud = provider cloud.**

------------------------------------------------------------------------

## Public Endpoint

An endpoint that can be reached using a public network address, subject
to the service's configuration and security controls.

------------------------------------------------------------------------

## Public Preview

A preview stage made available more broadly for customers to evaluate
before general availability.

------------------------------------------------------------------------

# R

## Region Pair

A relationship between Azure regions used in some resiliency and
disaster-recovery scenarios.

**Remember:**\
\> **Region Pair = Region ↔ Region.**

------------------------------------------------------------------------

## Relational Database

A database that organizes data using structured tables and
relationships.

**AZ-900 example:** Azure SQL Database.

------------------------------------------------------------------------

## Reliability

The ability of a system to recover from failures and continue operating.

------------------------------------------------------------------------

## Resource

An individual manageable Azure item such as a virtual machine, storage
account, or virtual network.

------------------------------------------------------------------------

## Resource Group

A logical container used to organize related Azure resources.

**Remember:**\
\> **Resource Group = container.**

------------------------------------------------------------------------

## Resource Lock

A protection mechanism that helps prevent accidental deletion or
modification of Azure resources.

### Common Locks

-   **CanNotDelete** --- resource can be modified but not deleted.
-   **ReadOnly** --- resource cannot be modified or deleted.

------------------------------------------------------------------------

## Role-Based Access Control (Azure RBAC)

An authorization system used to control who can perform actions on Azure
resources.

**Remember:**\
\> **RBAC = WHO can do it?**

------------------------------------------------------------------------

# S

## Scalability

The ability to increase or decrease resources or capacity to meet
changing demand.

------------------------------------------------------------------------

## Secure Score

A numerical measurement used to help assess and improve an
organization's security posture.

**Remember:**\
\> **Secure Score = security measurement.**

------------------------------------------------------------------------

## Serverless Computing

A cloud computing model where customers run applications or code without
managing the underlying servers.

**AZ-900 example:** Azure Functions.

------------------------------------------------------------------------

## Service Credit

A billing credit that may apply when an eligible service fails to meet
the terms of its Service Level Agreement.

------------------------------------------------------------------------

## Service Level Agreement (SLA)

An agreement describing Microsoft's availability commitment and
associated terms for an Azure service.

**Remember:**\
\> **SLA = availability commitment.**

------------------------------------------------------------------------

## Shared Responsibility Model

A cloud security model in which security and management responsibilities
are divided between the cloud provider and the customer. The exact
division changes depending on the cloud service model.

------------------------------------------------------------------------

## Single Sign-On (SSO)

An authentication experience that allows a user to sign in once and
access multiple applications without repeatedly entering credentials.

**Remember:**\
\> **SSO = sign in once.**

------------------------------------------------------------------------

## Software as a Service (SaaS)

A cloud service model where customers use a finished application while
the provider manages most of the underlying technology.

**Remember:**\
\> **SaaS = use the application.**

------------------------------------------------------------------------

## Subnet

A logical subdivision of an Azure Virtual Network.

**Remember:**\
\> **Subnet = part of a VNet.**

------------------------------------------------------------------------

## Subscription

An Azure resource hierarchy level that acts as a management and billing
boundary for Azure resources.

------------------------------------------------------------------------

# T

## Tag

Key-value metadata attached to Azure resources to help organize,
categorize, report on, or identify them.

**Remember:**\
\> **Tags = organize.**

------------------------------------------------------------------------

## Total Cost of Ownership (TCO) Calculator

A tool used to compare the estimated cost of running workloads
on-premises with running them in Azure.

**Remember:**\
\> **TCO = on-premises vs. Azure.**

------------------------------------------------------------------------

# U

## Update Domain

A grouping used by Availability Sets to help prevent all virtual
machines from being affected by planned maintenance at the same time.

**Remember:**\
\> **Update Domain = planned maintenance protection.**

------------------------------------------------------------------------

# V

## Virtual Network (VNet)

A logically isolated private network in Azure that allows supported
Azure resources to communicate.

**Remember:**\
\> **VNet = private Azure network.**

------------------------------------------------------------------------

# Z

## Zero Trust

A security model based on continually verifying access rather than
automatically trusting users or systems.

### Core Principles

``` text
VERIFY EXPLICITLY
USE LEAST PRIVILEGE
ASSUME BREACH
```

**Remember:**\
\> **Zero Trust = never trust, always verify.**

------------------------------------------------------------------------

## Zone-Redundant Storage (ZRS)

A storage redundancy option that replicates data across multiple
Availability Zones in the primary region.

**Remember:**\
\> **ZRS = zone redundancy.**

------------------------------------------------------------------------

# 🔤 Common AZ-900 Acronyms

  Acronym     Meaning
  ----------- -------------------------------------------
  **ACI**     Azure Container Instances
  **AKS**     Azure Kubernetes Service
  **ARM**     Azure Resource Manager
  **CapEx**   Capital Expenditure
  **DDoS**    Distributed Denial-of-Service
  **GA**      Generally Available
  **GRS**     Geo-Redundant Storage
  **GZRS**    Geo-Zone-Redundant Storage
  **IaaS**    Infrastructure as a Service
  **IaC**     Infrastructure as Code
  **LRS**     Locally Redundant Storage
  **MFA**     Multi-Factor Authentication
  **NSG**     Network Security Group
  **OpEx**    Operational Expenditure
  **PaaS**    Platform as a Service
  **RBAC**    Role-Based Access Control
  **SaaS**    Software as a Service
  **SIEM**    Security Information and Event Management
  **SLA**     Service Level Agreement
  **SSO**     Single Sign-On
  **TCO**     Total Cost of Ownership
  **VM**      Virtual Machine
  **VMSS**    Virtual Machine Scale Sets
  **VNet**    Virtual Network
  **ZRS**     Zone-Redundant Storage

------------------------------------------------------------------------

# 🎯 Ultra-Quick Definitions

  Term                     Remember
  ------------------------ ------------------------------
  **Authentication**       Who are you?
  **Authorization**        What can you do?
  **Entra ID**             Identity
  **RBAC**                 Permissions
  **Policy**               Rules
  **Locks**                Protection
  **Tags**                 Organization
  **Monitor**              Observe
  **Advisor**              Recommend
  **Service Health**       Azure problems
  **Defender for Cloud**   Security posture/protection
  **Secure Score**         Security measurement
  **Key Vault**            Secrets, keys, certificates
  **Sentinel**             SIEM
  **ARM**                  Manage Azure
  **ARM Template**         Define/deploy infrastructure
  **Azure Arc**            Extend Azure management
  **VM**                   Virtual computer
  **Functions**            Event-driven code
  **ACI**                  Run containers
  **AKS**                  Orchestrate containers
  **Blob**                 Objects
  **Azure Files**          File shares
  **Queue**                Messages
  **SQL Database**         Relational
  **Cosmos DB**            Global NoSQL
  **Pricing Calculator**   Estimate Azure
  **TCO Calculator**       On-premises vs. Azure
  **Cost Management**      Track spending
  **Reservation**          Commit and save
  **Spot VM**              Cheap but interruptible
  **SLA**                  Availability commitment
  **Marketplace**          Find Azure solutions
  **GA**                   General release

------------------------------------------------------------------------

# 📚 Related Cheat Sheets

Use the other files in this folder depending on what you need:

``` text
glossary.md
→ "What does this term mean?"

comparison-table.md
→ "What is the difference between these?"

cram-sheet.md
→ "Give me a fast review of everything."

exam-tips.md
→ "How do I remember the important concepts?"
```

> \[!TIP\] A good study method is to find a term in this glossary,
> explain it without looking, and then identify the Azure service or
> concept it is most easily confused with.
