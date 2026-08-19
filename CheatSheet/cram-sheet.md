[cram-sheet.md](https://github.com/user-attachments/files/31230307/cram-sheet.md)

# AZ-900 Cram Sheet

A fast final-review sheet for **Microsoft Azure Fundamentals (AZ-900)**.

> \[!TIP\] Use this after completing the lessons and labs. The goal is
> quick recall: **see the requirement → recognize the Azure concept →
> eliminate the wrong answers.**

------------------------------------------------------------------------

# ☁️ Cloud Concepts

## Cloud Benefits

  -----------------------------------------------------------------------
  Concept                             Remember
  ----------------------------------- -----------------------------------
  **High Availability**               Keep services available despite
                                      failures

  **Scalability**                     Add/remove capacity to meet demand

  **Elasticity**                      Automatically or rapidly adjust
                                      resources as demand changes

  **Reliability**                     Recover from failures and continue
                                      operating

  **Predictability**                  Better predict performance and cost

  **Governance**                      Apply standards and controls

  **Manageability**                   Easier management through cloud
                                      tools and automation
  -----------------------------------------------------------------------

## Cloud Models

``` text
Public Cloud  = Provider-owned cloud infrastructure
Private Cloud = Dedicated to one organization
Hybrid Cloud  = Public cloud + private/on-premises
Multi-Cloud   = Multiple cloud providers
```

## CapEx vs. OpEx

``` text
CapEx = BUY IT
OpEx  = USE IT / PAY AS YOU GO
```

------------------------------------------------------------------------

# 🏗️ IaaS vs. PaaS vs. SaaS

``` text
MORE CONTROL                               LESS CONTROL
     |                                          |
     v                                          v
   IaaS  ------------>  PaaS  ------------>  SaaS

MORE MANAGEMENT                         LESS MANAGEMENT
```

  -----------------------------------------------------------------------
  Model                   Think                   Example
  ----------------------- ----------------------- -----------------------
  **IaaS**                Manage the OS and       Azure Virtual Machines
                          applications            

  **PaaS**                Build apps without      Azure App Service
                          managing underlying     
                          servers                 

  **SaaS**                Use a finished          Microsoft 365
                          application             
  -----------------------------------------------------------------------

### Serverless

**Azure Functions** = event-driven code without managing servers.

------------------------------------------------------------------------

# 🌎 Azure Architecture

## Region

Geographic area containing one or more Azure datacenters.

## Availability Zone

Physically separate location **inside an Azure Region**.

## Region Pair

Region-to-region relationship used in resiliency and disaster-recovery
planning.

``` text
REGIONAL FAILURE   → Region Pair
ZONE FAILURE       → Availability Zones
```

------------------------------------------------------------------------

# 🏢 Azure Resource Hierarchy

``` text
Management Group
       ↓
Subscription
       ↓
Resource Group
       ↓
Resource
```

  Level                  Think
  ---------------------- -----------------------------
  **Management Group**   Organize subscriptions
  **Subscription**       Billing/management boundary
  **Resource Group**     Logical resource container
  **Resource**           Actual Azure service

------------------------------------------------------------------------

# 🛠️ ARM, Templates, and Arc

``` text
Azure Resource Manager = MANAGE AZURE
ARM Template           = DEFINE/DEPLOY INFRASTRUCTURE
Azure Arc              = EXTEND AZURE MANAGEMENT
```

## ARM Template

-   Infrastructure as Code
-   Declarative
-   Traditional ARM templates use JSON
-   Repeatable deployments

``` text
Parameters = INPUT
Variables  = REUSE
Resources  = CREATE
Outputs    = RETURN
```

## Azure Arc

Think:

> **On-premises + other clouds + edge resources managed with Azure
> capabilities**

------------------------------------------------------------------------

# 💻 Compute

  -----------------------------------------------------------------------
  Requirement                         Choose
  ----------------------------------- -----------------------------------
  Full OS control                     **Azure Virtual Machine**

  Automatically scale a group of VMs  **VM Scale Sets**

  Managed web app/API hosting         **Azure App Service**

  Event-driven serverless code        **Azure Functions**

  Quickly run a container             **Azure Container Instances (ACI)**

  Kubernetes/container orchestration  **Azure Kubernetes Service (AKS)**
  -----------------------------------------------------------------------

### Quick Recall

``` text
VM        = VIRTUAL COMPUTER
VMSS      = SCALE VMs
AppSvc    = HOST WEB APP
Functions = EVENT-DRIVEN CODE
ACI       = RUN CONTAINER
AKS       = ORCHESTRATE CONTAINERS
```

------------------------------------------------------------------------

# 🌐 Networking

## Virtual Network

Private network for Azure resources.

## Subnet

Smaller network segment inside a Virtual Network.

## Network Security Group

Allow/deny inbound and outbound network traffic.

## Azure Firewall

Managed centralized network firewall.

## Azure DDoS Protection

Protection against Distributed Denial-of-Service traffic-flood attacks.

### Quick Recall

``` text
VNet     = PRIVATE NETWORK
Subnet   = DIVIDE VNET
NSG      = ALLOW / DENY TRAFFIC
Firewall = CENTRAL FIREWALL
DDoS     = TRAFFIC-FLOOD PROTECTION
```

------------------------------------------------------------------------

# 💾 Storage

  Service             Think
  ------------------- -----------------------------
  **Blob Storage**    Objects / unstructured data
  **Azure Files**     Managed file shares
  **Queue Storage**   Application messages
  **Table Storage**   NoSQL key/attribute data

## Storage Redundancy

``` text
LRS  = LOCAL
ZRS  = ZONES
GRS  = GEOGRAPHIC
GZRS = GEOGRAPHIC + ZONES
```

  Option     Main Protection
  ---------- ----------------------------
  **LRS**    Local hardware failure
  **ZRS**    Availability Zone failure
  **GRS**    Regional disaster
  **GZRS**   Zone + regional protection

------------------------------------------------------------------------

# 🗄️ Databases

``` text
Azure SQL Database = RELATIONAL
Azure Cosmos DB    = NoSQL / GLOBALLY DISTRIBUTED
```

------------------------------------------------------------------------

# 👤 Identity

## Microsoft Entra ID

Microsoft cloud identity and access management service.

## Authentication vs. Authorization

``` text
Authentication = WHO ARE YOU?
Authorization  = WHAT CAN YOU DO?
```

## MFA

Multiple authentication factors.

## SSO

Sign in once and access multiple applications.

## Conditional Access

Access decisions based on configured signals and conditions.

``` text
MFA                = VERIFY MORE
SSO                = SIGN IN LESS
Conditional Access = IF / THEN ACCESS POLICY
```

------------------------------------------------------------------------

# 🏛️ Governance

``` text
WHO?       → Azure RBAC
WHAT?      → Azure Policy
PROTECT?   → Resource Locks
ORGANIZE?  → Tags
```

## Azure RBAC

Controls **who can perform actions** on Azure resources.

## Azure Policy

Controls **what configurations are allowed or required**.

## Resource Locks

  Lock                Modify?   Delete?
  ------------------ --------- ---------
  **CanNotDelete**      ✅        ❌
  **ReadOnly**          ❌        ❌

## Tags

Key-value metadata used to organize resources.

------------------------------------------------------------------------

# 🛡️ Security

## Microsoft Defender for Cloud

Security posture management and workload protection.

## Secure Score

Numerical indicator used to help measure security posture.

## Defense in Depth

Multiple security layers.

## Zero Trust

``` text
NEVER TRUST, ALWAYS VERIFY

Verify Explicitly
       +
Use Least Privilege
       +
Assume Breach
```

## Azure Key Vault

``` text
SECRETS
KEYS
CERTIFICATES
```

## Microsoft Sentinel

Cloud-native **SIEM** and security operations platform.

``` text
SIEM = Security Information and Event Management
```

## Azure Dedicated Host

Physical Azure server dedicated to one customer for supported Azure VMs.

------------------------------------------------------------------------

# 📊 Monitoring

This comparison is worth knowing cold:

``` text
Azure Monitor
→ WHAT IS HAPPENING?

Azure Advisor
→ WHAT SHOULD I IMPROVE?

Azure Service Health
→ IS AZURE HAVING A PROBLEM?
```

## Azure Monitor

Metrics, logs, telemetry, alerts.

## Azure Advisor

Recommendations involving areas such as cost, reliability, security,
performance, and operational excellence.

## Azure Service Health

Azure incidents, planned maintenance, and health advisories relevant to
your environment.

------------------------------------------------------------------------

# 💵 Pricing

## Pricing Calculator

> **What might these Azure resources cost?**

Estimate Azure resource costs before deployment.

## TCO Calculator

> **How does Azure compare with our on-premises environment?**

Compare on-premises infrastructure costs with Azure.

## Azure Cost Management

> **What are we actually spending?**

Monitor, analyze, and optimize cloud spending.

``` text
Pricing Calculator = ESTIMATE AZURE
TCO Calculator     = ON-PREM vs. AZURE
Cost Management    = MONITOR SPENDING
```

------------------------------------------------------------------------

# 💰 Cost Optimization

``` text
Pay-As-You-Go = FLEXIBILITY
Reservation   = COMMITMENT + SAVINGS
Spot VM       = DISCOUNTED + INTERRUPTIBLE
```

## Reservation

Best for eligible, predictable long-running usage when an organization
can make a commitment.

## Spot VM

Discounted unused compute capacity that can be **evicted**.

------------------------------------------------------------------------

# 📈 SLA

**Service Level Agreement** = Microsoft's availability commitment and
associated terms for an Azure service.

``` text
HIGHER SLA %
     =
LESS ALLOWABLE DOWNTIME
```

## Composite SLA

Dependent services can reduce overall availability.

Example:

``` text
99.9% × 99.9%
= 99.8001%
```

## Service Credit

Potential billing credit when an applicable SLA commitment is not met
according to its terms.

------------------------------------------------------------------------

# 🛒 Azure Marketplace

Find Microsoft and third-party solutions that can run on or integrate
with Azure.

``` text
Marketplace = SHOP FOR AZURE SOLUTIONS
```

------------------------------------------------------------------------

# 🚀 Service Lifecycle

``` text
Private Preview
      ↓
Public Preview
      ↓
Generally Available (GA)
      ↓
Possible Retirement
```

``` text
Private Preview = LIMITED TESTING
Public Preview  = BROADER EVALUATION
GA              = GENERAL RELEASE
Retirement      = MIGRATE AWAY
```

------------------------------------------------------------------------

# 🎯 Know These Cold

  If the question says...           Think...
  --------------------------------- ---------------------------------------
  Who are you?                      **Authentication**
  What can you do?                  **Authorization / RBAC**
  Resource configuration rules      **Azure Policy**
  Prevent resource deletion         **Resource Lock**
  Organize resources                **Tags**
  Metrics and logs                  **Azure Monitor**
  Recommendations                   **Azure Advisor**
  Azure outage or maintenance       **Azure Service Health**
  Secrets, keys, certificates       **Azure Key Vault**
  Multiple security layers          **Defense in Depth**
  Never trust, always verify        **Zero Trust**
  Security posture                  **Defender for Cloud / Secure Score**
  SIEM                              **Microsoft Sentinel**
  Event-driven code                 **Azure Functions**
  Managed web application           **Azure App Service**
  Full OS control                   **Virtual Machine**
  Scale a group of VMs              **VM Scale Sets**
  Simple container                  **ACI**
  Kubernetes                        **AKS**
  Private Azure network             **Virtual Network**
  Allow/deny network traffic        **NSG**
  Central managed firewall          **Azure Firewall**
  Traffic-flood attack              **DDoS Protection**
  Object/unstructured storage       **Blob Storage**
  Managed file share                **Azure Files**
  Relational database               **Azure SQL Database**
  Globally distributed NoSQL        **Azure Cosmos DB**
  Extend management outside Azure   **Azure Arc**
  Infrastructure as Code            **ARM Template**
  Estimate Azure cost               **Pricing Calculator**
  Compare on-premises with Azure    **TCO Calculator**
  Monitor actual spending           **Cost Management**
  Long-term predictable workload    **Reservation**
  Interruptible cheap compute       **Spot VM**
  Availability commitment           **SLA**
  Production release                **GA**

------------------------------------------------------------------------

# ⚠️ Common Exam Traps

### RBAC vs. Policy

``` text
RBAC   = WHO can do it?
Policy = WHAT is allowed?
```

### Monitor vs. Advisor

``` text
Monitor = OBSERVE
Advisor = RECOMMEND
```

### Monitor vs. Service Health

``` text
Monitor        = YOUR RESOURCE TELEMETRY
Service Health = AZURE PLATFORM ISSUES
```

### NSG vs. Firewall

``` text
NSG      = NETWORK TRAFFIC RULES
Firewall = CENTRALIZED MANAGED FIREWALL
```

### Key Vault vs. Sentinel

``` text
Key Vault = STORE SENSITIVE ITEMS
Sentinel  = WATCH / ANALYZE SECURITY EVENTS
```

### Region Pair vs. Availability Zone

``` text
Region Pair       = REGION ↔ REGION
Availability Zone = INSIDE ONE REGION
```

### Pricing vs. TCO

``` text
Pricing = AZURE COST
TCO     = ON-PREM vs. AZURE
```

### Reservation vs. Spot VM

``` text
Reservation = COMMIT
Spot VM     = CAN BE EVICTED
```

------------------------------------------------------------------------

# 🧠 Final Exam Approach

``` text
READ THE REQUIREMENT
        ↓
FIND THE KEYWORD
        ↓
ELIMINATE WRONG SERVICES
        ↓
COMPARE THE FINAL OPTIONS
        ↓
CHOOSE THE BEST MATCH
```

Watch for words such as:

-   **Managed**
-   **Serverless**
-   **Relational**
-   **NoSQL**
-   **Highly available**
-   **Cost-effective**
-   **Private**
-   **Compliant**
-   **Scalable**
-   **Least administrative effort**

> \[!IMPORTANT\] Do not choose an answer just because you recognize the
> Azure service name. Choose the service that **best satisfies the
> requirement**.

------------------------------------------------------------------------

# 📚 Final Review Resources

-   **AZ-900 Study Guide:**
    https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-900
-   **AZ-900 Certification:**
    https://learn.microsoft.com/en-us/credentials/certifications/azure-fundamentals/
-   **Microsoft Learn:** https://learn.microsoft.com/training/

After using this cram sheet, complete the Microsoft **Practice
Assessment** and review every missed or uncertain question.
