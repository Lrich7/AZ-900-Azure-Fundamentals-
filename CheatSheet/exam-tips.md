[exam-tips.md](https://github.com/user-attachments/files/31230317/exam-tips.md)

# AZ-900 Exam Tips & Memory Tricks

Use this page for **quick memory tricks, keywords, and exam shortcuts**
for Microsoft Azure Fundamentals (AZ-900).

> \[!TIP\] Do not try to memorize every Azure feature. Learn the **main
> job of each service** and the words that usually point toward it.

------------------------------------------------------------------------

# 🧠 Start With the Requirement

When you see a scenario question:

``` text
READ THE REQUIREMENT
        ↓
FIND THE KEYWORD
        ↓
ASK "WHAT DOES THIS SERVICE DO?"
        ↓
ELIMINATE SERVICES THAT DO SOMETHING ELSE
        ↓
CHOOSE THE BEST MATCH
```

A question may contain lots of information that does not change the
answer.

Focus on the actual requirement.

------------------------------------------------------------------------

# ☁️ Cloud Models

## Easy Memory Trick

``` text
PUBLIC  = PROVIDER
PRIVATE = ORGANIZATION
HYBRID  = MIX
MULTI   = MULTIPLE PROVIDERS
```

### Think Hybrid when:

> The scenario mentions **on-premises AND cloud**.

### Think Multi-Cloud when:

> The scenario mentions **more than one cloud provider**.

------------------------------------------------------------------------

# 💰 CapEx vs. OpEx

``` text
CapEx = BUY
OpEx  = USE
```

### CapEx

Think:

> **Buy the server. Own the hardware. Pay upfront.**

### OpEx

Think:

> **Use the cloud. Pay as you consume.**

------------------------------------------------------------------------

# 🏗️ IaaS vs. PaaS vs. SaaS

Use the **management ladder**:

``` text
MOST CONTROL
    |
   IaaS
    |
   PaaS
    |
   SaaS
    |
LEAST CONTROL
```

### Memory Trick

``` text
IaaS = MANAGE MORE
PaaS = BUILD
SaaS = USE
```

### Scenario Keywords

  Question Mentions...                            Think...
  ----------------------------------------------- ----------
  Control the operating system                    **IaaS**
  Build an application without managing servers   **PaaS**
  Use a finished application                      **SaaS**

------------------------------------------------------------------------

# 🌎 Regions, Zones, and Region Pairs

This distinction is worth memorizing.

``` text
REGION PAIR
Region  ←→  Region

AVAILABILITY ZONES
     ONE REGION
        |
   Zone 1
   Zone 2
   Zone 3
```

### Memory Trick

``` text
PAIR = TWO REGIONS
ZONE = INSIDE A REGION
```

### If the Question Says...

  Scenario                                      Think
  --------------------------------------------- ---------------------------------------
  Datacenter/location failure inside a region   **Availability Zone**
  Regional disaster                             **Region Pair / cross-region design**
  Geographic Azure location                     **Region**

------------------------------------------------------------------------

# 🏢 Azure Resource Hierarchy

Remember it from **biggest to smallest**:

``` text
Management Group
      ↓
Subscription
      ↓
Resource Group
      ↓
Resource
```

### Memory Phrase

> **Manage → Subscribe → Group → Resource**

### Quick Recall

``` text
Management Group = ORGANIZE SUBSCRIPTIONS
Subscription     = BILLING / MANAGEMENT BOUNDARY
Resource Group   = CONTAINER
Resource         = ACTUAL SERVICE
```

------------------------------------------------------------------------

# 🛠️ ARM vs. ARM Template vs. Azure Arc

These names are easy to mix up.

``` text
ARM          = MANAGE
ARM TEMPLATE = DEFINE / DEPLOY
AZURE ARC    = EXTEND
```

### ARM

> Azure's management and deployment layer.

### ARM Template

> Infrastructure as Code used for repeatable Azure deployments.

### Azure Arc

> Extend Azure management to supported resources **outside Azure**.

### Keyword Trick

``` text
Management layer → ARM
JSON / IaC       → ARM Template
On-prem / other cloud → Azure Arc
```

------------------------------------------------------------------------

# 💻 Compute Memory Tricks

``` text
VM        = COMPUTER
VMSS      = MANY SCALING VMs
APP SVC   = WEB APP
FUNCTIONS = EVENT CODE
ACI       = RUN CONTAINER
AKS       = MANAGE CONTAINERS
```

## VM vs. VM Scale Sets

``` text
VM   = ONE / INDIVIDUAL COMPUTE
VMSS = GROUP + SCALE
```

## App Service vs. Functions

``` text
App Service = HOST THE APP
Functions   = RUN CODE WHEN SOMETHING HAPPENS
```

## ACI vs. AKS

``` text
ACI = RUN IT
AKS = ORCHESTRATE IT
```

### Exam Keywords

  Keyword                   Think
  ------------------------- ---------------------
  Full OS control           **Virtual Machine**
  Automatically scale VMs   **VM Scale Sets**
  Managed web application   **App Service**
  Event-driven              **Azure Functions**
  Simple container          **ACI**
  Kubernetes                **AKS**

------------------------------------------------------------------------

# 🌐 Networking Memory Tricks

``` text
VNet     = PRIVATE NETWORK
SUBNET   = PIECE OF A VNET
NSG      = TRAFFIC RULES
FIREWALL = CENTRAL FIREWALL
DDoS     = TRAFFIC FLOOD
```

## NSG vs. Azure Firewall

Ask:

> Do I need **allow/deny network rules**, or a **central managed
> firewall**?

``` text
NSG      = ALLOW / DENY
Firewall = CENTRAL FILTERING
```

## DDoS

Remember:

> **DDoS = TOO MUCH TRAFFIC**

If the scenario describes attackers overwhelming a public service with
traffic:

**Think Azure DDoS Protection.**

------------------------------------------------------------------------

# 💾 Storage Memory Tricks

``` text
BLOB  = OBJECTS
FILES = FILE SHARES
QUEUE = MESSAGES
TABLE = NoSQL DATA
```

### Blob

Think:

> Pictures, video, backups, documents, unstructured objects.

### Azure Files

Think:

> Network/shared drive.

### Queue

Think:

> Applications sending messages to each other.

### Table

Think:

> Simple NoSQL key/attribute data.

------------------------------------------------------------------------

# 🛡️ Storage Redundancy

The letters tell you most of the answer.

``` text
L = LOCAL
Z = ZONE
G = GEO
```

So:

``` text
LRS  = LOCAL
ZRS  = ZONES
GRS  = GEO
GZRS = GEO + ZONES
```

### Failure Memory Trick

``` text
Hardware failure → LRS
Zone failure     → ZRS
Regional failure → GRS
Zone + Region    → GZRS
```

------------------------------------------------------------------------

# 🗄️ SQL vs. Cosmos DB

Keep this one simple:

``` text
SQL Database = RELATIONAL
Cosmos DB    = NoSQL + GLOBAL
```

### Keyword Trick

``` text
Tables / relational → Azure SQL Database
Globally distributed NoSQL → Cosmos DB
```

------------------------------------------------------------------------

# 👤 Authentication vs. Authorization

One of the most important memory tricks:

``` text
AUTHENTICATION = WHO ARE YOU?
AUTHORIZATION  = WHAT CAN YOU DO?
```

Remember the order:

``` text
WHO ARE YOU?
     ↓
WHAT CAN YOU DO?
```

> **Authenticate first. Authorize second.**

------------------------------------------------------------------------

# 🔑 MFA vs. SSO vs. Conditional Access

``` text
MFA = VERIFY MORE
SSO = SIGN IN LESS
CA  = IF / THEN
```

## MFA

More than one authentication factor.

## SSO

One sign-in used across multiple applications.

## Conditional Access

Makes an access decision based on configured conditions/signals.

### Example

``` text
IF
User signs in from a risky situation

THEN
Require MFA
```

------------------------------------------------------------------------

# 🏛️ RBAC vs. Policy vs. Locks vs. Tags

Memorize these four questions:

``` text
WHO?      = RBAC
WHAT?     = POLICY
PROTECT?  = LOCK
ORGANIZE? = TAG
```

## RBAC

> **WHO can do something?**

## Azure Policy

> **WHAT is allowed or required?**

## Resource Lock

> **How do I protect this resource from changes/deletion?**

## Tags

> **How do I organize or identify resources?**

------------------------------------------------------------------------

# 🔒 Resource Lock Trick

``` text
CanNotDelete
= CAN CHANGE
= CANNOT DELETE

ReadOnly
= CANNOT CHANGE
= CANNOT DELETE
```

------------------------------------------------------------------------

# 🛡️ Defender for Cloud vs. Secure Score

``` text
DEFENDER FOR CLOUD = SECURITY SERVICE
SECURE SCORE       = SECURITY MEASUREMENT
```

### Think Defender for Cloud when:

> The question asks about cloud security posture or workload protection.

### Think Secure Score when:

> The question asks for a **score/measurement** of security posture.

------------------------------------------------------------------------

# 🧱 Defense in Depth vs. Zero Trust

``` text
DEFENSE IN DEPTH = LAYERS
ZERO TRUST       = VERIFY
```

## Defense in Depth

Think of a castle:

``` text
Wall
 ↓
Gate
 ↓
Guard
 ↓
Locked Door
 ↓
Safe
```

If one layer fails, another layer remains.

## Zero Trust

Remember the three principles:

``` text
VERIFY EXPLICITLY
USE LEAST PRIVILEGE
ASSUME BREACH
```

And the phrase:

> **Never trust, always verify.**

------------------------------------------------------------------------

# 🔐 Key Vault

This is a three-word memory item:

``` text
SECRETS
KEYS
CERTIFICATES
```

If you see:

-   Password
-   API key
-   Connection string
-   Encryption key
-   Certificate

Think:

> **Azure Key Vault**

------------------------------------------------------------------------

# 🚨 Microsoft Sentinel

Remember:

``` text
SENTINEL = SIEM
```

SIEM:

> **Security Information and Event Management**

### Think Sentinel when:

-   Collecting security events.
-   Analyzing security logs.
-   Detecting threats.
-   Investigating incidents.
-   Security operations.

### Memory Phrase

> **Sentinel watches.**

------------------------------------------------------------------------

# 🖥️ Azure Dedicated Host

``` text
DEDICATED HOST = PHYSICAL SERVER FOR ONE CUSTOMER
```

If the scenario specifically requires dedicated physical Azure server
hardware:

> **Think Azure Dedicated Host.**

------------------------------------------------------------------------

# 📊 Monitor vs. Advisor vs. Service Health

This is one of the best exam memory tricks:

``` text
MONITOR
= WHAT IS HAPPENING?

ADVISOR
= WHAT SHOULD I IMPROVE?

SERVICE HEALTH
= IS AZURE HAVING A PROBLEM?
```

### Keywords

  Question Says...                       Think
  -------------------------------------- --------------------
  Metrics                                **Monitor**
  Logs                                   **Monitor**
  Telemetry                              **Monitor**
  Recommendations                        **Advisor**
  Improve cost/performance/reliability   **Advisor**
  Azure outage                           **Service Health**
  Planned Azure maintenance              **Service Health**

------------------------------------------------------------------------

# 💵 Pricing vs. TCO vs. Cost Management

Remember the timeline:

``` text
BEFORE AZURE
     |
     v
TCO

PLANNING AZURE
     |
     v
PRICING CALCULATOR

RUNNING AZURE
     |
     v
COST MANAGEMENT
```

### Memory Trick

``` text
Pricing = WHAT WILL AZURE COST?
TCO     = ON-PREM vs. AZURE
Cost Mgmt = WHAT AM I SPENDING?
```

------------------------------------------------------------------------

# 💰 Pay-As-You-Go vs. Reservation vs. Spot VM

``` text
PAYG        = FLEXIBLE
RESERVATION = COMMIT
SPOT        = INTERRUPTIBLE
```

## Reservation

Think:

> **Predictable + long-term = commit and save**

## Spot VM

Think:

> **Cheap because Azure can take it back**

The key word is:

> **Eviction**

If the workload can stop and restart later, Spot may fit.

------------------------------------------------------------------------

# 📈 SLA Memory Tricks

``` text
SLA = AVAILABILITY COMMITMENT
```

### More 9s

``` text
MORE 9s
   =
MORE AVAILABILITY
   =
LESS DOWNTIME
```

### Composite SLA

Remember:

> **Multiply, don't add.**

``` text
99.9% × 99.9%
= 99.8001%
```

Adding dependent services can lower the overall composite SLA.

------------------------------------------------------------------------

# 🛒 Azure Marketplace

Easy one:

``` text
MARKETPLACE = SHOP
```

If the question asks where to find Microsoft or third-party Azure
solutions:

> **Azure Marketplace**

------------------------------------------------------------------------

# 🚀 Preview vs. GA

``` text
PREVIEW = TEST
GA      = RELEASED
```

### Private vs. Public Preview

``` text
Private Preview = LIMITED GROUP
Public Preview  = BROADER ACCESS
```

### GA

``` text
GA = GENERALLY AVAILABLE
   = GENERAL PRODUCTION RELEASE
```

------------------------------------------------------------------------

# 🎯 Keyword → Answer

Use this for rapid review.

  Keyword / Requirement          Think
  ------------------------------ ------------------------
  On-prem + Azure                **Hybrid Cloud**
  Multiple cloud providers       **Multi-Cloud**
  OS control                     **IaaS / VM**
  Managed application platform   **PaaS**
  Finished software              **SaaS**
  Inside one Azure region        **Availability Zone**
  Two regions                    **Region Pair**
  Billing boundary               **Subscription**
  Logical container              **Resource Group**
  Azure management layer         **ARM**
  Infrastructure as Code         **ARM Template**
  Outside Azure                  **Azure Arc**
  Web app                        **App Service**
  Event-driven                   **Functions**
  Simple container               **ACI**
  Kubernetes                     **AKS**
  Private network                **VNet**
  Traffic rules                  **NSG**
  Central firewall               **Azure Firewall**
  Traffic flood                  **DDoS Protection**
  Objects                        **Blob Storage**
  File shares                    **Azure Files**
  Messages                       **Queue Storage**
  Relational                     **Azure SQL Database**
  Global NoSQL                   **Cosmos DB**
  Who are you?                   **Authentication**
  What can you do?               **Authorization**
  Permissions                    **RBAC**
  Resource rules                 **Azure Policy**
  Prevent deletion               **Resource Lock**
  Organize                       **Tags**
  Security posture               **Defender for Cloud**
  Security measurement           **Secure Score**
  Layers                         **Defense in Depth**
  Never trust                    **Zero Trust**
  Secrets/keys/certs             **Key Vault**
  SIEM                           **Sentinel**
  Metrics/logs                   **Monitor**
  Recommendations                **Advisor**
  Azure outage                   **Service Health**
  Estimate Azure cost            **Pricing Calculator**
  On-prem vs. Azure cost         **TCO Calculator**
  Actual spending                **Cost Management**
  Long-term predictable usage    **Reservation**
  Can be evicted                 **Spot VM**
  Availability commitment        **SLA**
  Third-party Azure solution     **Marketplace**
  General production release     **GA**

------------------------------------------------------------------------

# ⚠️ Words That Should Get Your Attention

When reading a question, watch for these words:

``` text
MANAGED
SERVERLESS
RELATIONAL
NoSQL
ON-PREMISES
HYBRID
MULTI-CLOUD
METRICS
RECOMMENDATION
OUTAGE
POLICY
PERMISSION
SECRET
SIEM
EVICT
COMMIT
AVAILABILITY
```

Often, one or two words reveal what concept Microsoft is testing.

------------------------------------------------------------------------

# 🧠 If You Only Remember 25 Things

1.  **Authentication = Who are you?**
2.  **Authorization = What can you do?**
3.  **RBAC = Who can do it?**
4.  **Policy = What is allowed?**
5.  **Locks = Protect resources.**
6.  **Tags = Organize resources.**
7.  **Monitor = Observe.**
8.  **Advisor = Recommend.**
9.  **Service Health = Azure problems.**
10. **Key Vault = Secrets + Keys + Certificates.**
11. **Sentinel = SIEM.**
12. **Defense in Depth = Layers.**
13. **Zero Trust = Never trust, always verify.**
14. **Region Pair = Region ↔ Region.**
15. **Availability Zone = Inside one region.**
16. **ARM = Manage Azure.**
17. **ARM Template = Infrastructure as Code.**
18. **Azure Arc = Manage beyond Azure.**
19. **Functions = Event-driven/serverless.**
20. **ACI = Run containers; AKS = orchestrate containers.**
21. **SQL = Relational; Cosmos DB = NoSQL/global.**
22. **Pricing Calculator = Azure estimate.**
23. **TCO = On-premises vs. Azure.**
24. **Reservation = Commit; Spot = Can be evicted.**
25. **SLA = Availability commitment.**

------------------------------------------------------------------------

# 🏁 Final Memory Strategy

When you review, do not repeatedly reread definitions.

Try this instead:

``` text
SEE THE SERVICE
      ↓
SAY ITS JOB OUT LOUD
      ↓
NAME THE SERVICE IT IS
MOST EASILY CONFUSED WITH
      ↓
EXPLAIN THE DIFFERENCE
```

Example:

``` text
Azure Advisor
     ↓
Gives recommendations
     ↓
Often confused with Azure Monitor
     ↓
Monitor observes
Advisor recommends
```

If you can explain the **difference between similar services**, you are
much more likely to recognize the correct answer in a scenario question.

> \[!TIP\] Use `comparison-table.md` when two concepts still feel
> similar, and use `cram-sheet.md` when you want a fast review of the
> entire course.
