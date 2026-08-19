[comparison-table.md](https://github.com/user-attachments/files/31230304/comparison-table.md)

# AZ-900 Comparison Tables

Use this page for quick review of concepts that are easy to confuse on
the AZ-900 exam.

> \[!TIP\] Focus on understanding **why you would choose one option over
> another**, not just memorizing definitions.

------------------------------------------------------------------------

## ☁️ Cloud Models

  ---------------------------------------------------------------------------
  Model             Infrastructure        Best For          Key Idea
  ----------------- --------------------- ----------------- -----------------
  **Public Cloud**  Cloud provider        Most cloud        Shared provider
                                          workloads         infrastructure

  **Private Cloud** Single organization   Maximum control   Dedicated
                                                            environment

  **Hybrid Cloud**  Public +              Organizations     Connect cloud and
                    private/on-premises   using both        on-premises
                                          environments      

  **Multi-Cloud**   Multiple cloud        Using services    More than one
                    providers             from several      cloud provider
                                          providers         
  ---------------------------------------------------------------------------

**Exam shortcut:** Public = Provider → Private = Organization → Hybrid =
Mix → Multi-Cloud = Multiple providers

------------------------------------------------------------------------

## 💰 CapEx vs. OpEx

                       CapEx                      OpEx
  -------------------- -------------------------- --------------------------
  **Meaning**          Capital Expenditure        Operational Expenditure
  **Payment**          Large upfront investment   Ongoing expense
  **Example**          Buying servers             Paying monthly for Azure
  **Traditional IT**   Common                     Less common
  **Cloud**            Reduced                    Common
  **Memory Trick**     **Buy it**                 **Use it / pay for it**

------------------------------------------------------------------------

## 🏗️ IaaS vs. PaaS vs. SaaS

  ----------------------------------------------------------------------------
                    IaaS              PaaS               SaaS
  ----------------- ----------------- ------------------ ---------------------
  **You Manage**    OS, apps, data    Apps and data      Mostly
                                                         usage/configuration

  **Provider        Physical          Infrastructure +   Almost everything
  Manages**         infrastructure    OS/platform        

  **Control**       Highest           Medium             Lowest

  **Management      Highest           Medium             Lowest
  Effort**                                               

  **Example**       Azure Virtual     Azure App Service  Microsoft 365
                    Machines                             

  **Think**         Rent              Build apps         Use software
                    infrastructure                       
  ----------------------------------------------------------------------------

``` text
MORE CUSTOMER CONTROL                     LESS CUSTOMER CONTROL
        |                                           |
        v                                           v
     IaaS  ---------------->  PaaS  ---------------->  SaaS
MORE MANAGEMENT                           LESS MANAGEMENT
```

------------------------------------------------------------------------

## 🌎 Region vs. Availability Zone vs. Region Pair

  -----------------------------------------------------------------------
                    Region            Availability Zone Region Pair
  ----------------- ----------------- ----------------- -----------------
  **What is it?**   Geographic Azure  Physically        Two associated
                    location          separate location Azure regions
                                      within a region   

  **Scope**         Regional          Inside one region Across regions

  **Protects        ---               Datacenter/zone   Regional disaster
  Against**                           failure           

  **Primary         Host Azure        High availability Disaster recovery
  Purpose**         resources                           / resiliency

  **Think**         Location          Separate          Another region
                                      datacenter        
                                      locations         
  -----------------------------------------------------------------------

**Exam shortcut:** Zone failure → **Availability Zones** · Regional
disaster → **Region Pair**

------------------------------------------------------------------------

## 🏢 Azure Resource Hierarchy

  -----------------------------------------------------------------------
  Level                   Contains                Main Purpose
  ----------------------- ----------------------- -----------------------
  **Management Group**    Subscriptions           Governance across
                                                  subscriptions

  **Subscription**        Resource Groups         Billing and access
                                                  boundary

  **Resource Group**      Resources               Logical organization

  **Resource**            ---                     Actual Azure service
  -----------------------------------------------------------------------

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

## 🛠️ ARM vs. ARM Templates vs. Azure Arc

  --------------------------------------------------------------------------
                    Azure Resource    ARM Template      Azure Arc
                    Manager                             
  ----------------- ----------------- ----------------- --------------------
  **Purpose**       Manage/deploy     Define            Extend Azure
                    Azure resources   infrastructure as management outside
                                      code              Azure

  **Key Idea**      Management layer  Repeatable        Hybrid/multi-cloud
                                      deployment        management

  **Think**         Manage            Deploy            Extend

  **Exam Keyword**  Management        JSON / IaC        On-premises / other
                                                        clouds
  --------------------------------------------------------------------------

**Memory trick:** ARM = Manage · ARM Template = Define/Deploy · Arc =
Extend

------------------------------------------------------------------------

## 💻 Azure Compute Services

  -----------------------------------------------------------------------
  Service                 Type                    Best For
  ----------------------- ----------------------- -----------------------
  **Virtual Machines**    IaaS                    Maximum OS/control

  **VM Scale Sets**       IaaS                    Groups of automatically
                                                  scaling VMs

  **App Service**         PaaS                    Web apps and APIs

  **Azure Functions**     Serverless              Event-driven code

  **Container Instances   Container Service       Simple container
  (ACI)**                                         execution

  **Azure Kubernetes      Managed Kubernetes      Container orchestration
  Service (AKS)**                                 
  -----------------------------------------------------------------------

### Common Exam Decisions

  -----------------------------------------------------------------------
  Scenario                            Choose
  ----------------------------------- -----------------------------------
  Need OS-level control               **Virtual Machine**

  Automatically scale many VMs        **VM Scale Sets**

  Host a web application without      **App Service**
  managing servers                    

  Run code when an event occurs       **Azure Functions**

  Quickly run a container             **Azure Container Instances (ACI)**

  Manage complex containerized        **Azure Kubernetes Service (AKS)**
  workloads                           
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🌐 Public vs. Private Endpoints

                            Public Endpoint     Private Endpoint
  ------------------------- ------------------- ---------------------------
  **Address**               Public              Private IP
  **Internet Accessible**   Yes                 No direct public exposure
  **VNet Integration**      Not required        Yes
  **Exposure**              Higher              Lower
  **Think**                 Internet entrance   Private entrance

------------------------------------------------------------------------

## 💾 Azure Storage Services

  -----------------------------------------------------------------------
  Service                 Best For                Think
  ----------------------- ----------------------- -----------------------
  **Blob Storage**        Images, video, backups, Objects/files
                          unstructured files      

  **Azure Files**         Shared SMB/NFS file     Network drive
                          shares                  

  **Queue Storage**       Messages between        Messages
                          application components  

  **Table Storage**       NoSQL structured data   Key/value

  **Azure SQL Database**  Relational data         SQL

  **Azure Cosmos DB**     Globally distributed    Global NoSQL
                          NoSQL                   
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🛡️ Storage Redundancy

  -----------------------------------------------------------------------
                          Copies/Location         Protects Against
  ----------------------- ----------------------- -----------------------
  **LRS**                 3 copies in one         Hardware failure
                          datacenter              

  **ZRS**                 3 copies across         Zone/datacenter failure
                          Availability Zones      

  **GRS**                 Primary region +        Regional disaster
                          secondary region        

  **GZRS**                Availability Zones +    Zone + regional failure
                          secondary region        
  -----------------------------------------------------------------------

**Memory trick:** L = Local · Z = Zones · G = Geographic · GZ =
Geographic + Zones

------------------------------------------------------------------------

## 📊 Azure Monitor vs. Advisor vs. Service Health

  Service                    Question It Answers
  -------------------------- -----------------------------------------
  **Azure Monitor**          What is happening with my resources?
  **Azure Advisor**          How can I improve my resources?
  **Azure Service Health**   Is Azure having a problem affecting me?

------------------------------------------------------------------------

## 🔐 Authentication vs. Authorization

                 Authentication              Authorization
  -------------- --------------------------- ---------------------------
  **Question**   Who are you?                What can you do?
  **Occurs**     First                       After authentication
  **Example**    Sign in with password/MFA   Permission to modify a VM
  **Think**      Identity                    Permissions

> **Authenticate first → Authorize second.**

------------------------------------------------------------------------

## 👤 Entra ID vs. RBAC vs. Conditional Access

  -----------------------------------------------------------------------
                    Microsoft Entra   RBAC              Conditional
                    ID                                  Access
  ----------------- ----------------- ----------------- -----------------
  **Purpose**       Identity          Resource          Conditional
                    management        permissions       access decisions

  **Controls**      Identities        What users can do Whether/how
                                                        access is granted

  **Think**         Who you are       What you can do   Under what
                                                        conditions
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🔑 MFA vs. SSO

  -----------------------------------------------------------------------
                          MFA                     SSO
  ----------------------- ----------------------- -----------------------
  **Purpose**             Increase authentication Reduce repeated
                          security                sign-ins

  **How**                 Multiple authentication One sign-in for
                          factors                 multiple apps

  **Example**             Password + phone        Sign into Microsoft 365
                          approval                once

  **Think**               Verify more             Sign in less
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🏛️ RBAC vs. Azure Policy vs. Resource Locks vs. Tags

  Service             Primary Question
  ------------------- -----------------------------------------
  **RBAC**            **WHO** can perform actions?
  **Azure Policy**    **WHAT** is allowed or required?
  **Resource Lock**   How do I prevent changes/deletion?
  **Tags**            How do I organize/categorize resources?

``` text
WHO?       → RBAC
WHAT?      → Azure Policy
PROTECT?   → Resource Lock
ORGANIZE?  → Tags
```

------------------------------------------------------------------------

## 🔒 Resource Locks

  Lock                Modify?   Delete?
  ------------------ --------- ---------
  **CanNotDelete**      ✅        ❌
  **ReadOnly**          ❌        ❌

------------------------------------------------------------------------

## 🛡️ Security Services

  -----------------------------------------------------------------------
  Service                             Primary Purpose
  ----------------------------------- -----------------------------------
  **Microsoft Defender for Cloud**    Security posture management and
                                      threat protection

  **Network Security Group (NSG)**    Control inbound and outbound
                                      network traffic

  **Azure Firewall**                  Managed network firewall

  **Azure DDoS Protection**           Protect against Distributed
                                      Denial-of-Service attacks

  **Azure Key Vault**                 Securely store secrets, keys, and
                                      certificates

  **Microsoft Sentinel**              Cloud-native SIEM and SOAR

  **Azure Dedicated Hosts**           Dedicated physical servers for
                                      Azure VMs
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🧠 Defense in Depth vs. Zero Trust

  -----------------------------------------------------------------------
                          Defense in Depth        Zero Trust
  ----------------------- ----------------------- -----------------------
  **Concept**             Multiple security       Never trust, always
                          layers                  verify

  **Goal**                If one layer fails,     Verify every access
                          others remain           request

  **Think**               Layers                  Verification
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 💵 Pricing Calculator vs. TCO Calculator vs. Cost Management

  -----------------------------------------------------------------------
  Tool                    Purpose                 Think
  ----------------------- ----------------------- -----------------------
  **Pricing Calculator**  Estimate future Azure   What will Azure cost?
                          costs                   

  **TCO Calculator**      Compare on-premises     Should we move to
                          costs with Azure        Azure?

  **Azure Cost            Monitor and optimize    What are we spending?
  Management**            Azure spending          
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🚀 Preview vs. Generally Available (GA)

  -----------------------------------------------------------------------
                          Preview                 Generally Available
                                                  (GA)
  ----------------------- ----------------------- -----------------------
  **Purpose**             Testing/evaluation      Production

  **Fully Released**      No                      Yes

  **Support/SLA**         May be limited          Standard support/SLA
                                                  where applicable

  **Production**          Generally avoid for     Yes
                          critical workloads      
  -----------------------------------------------------------------------

**Exam shortcut:** Production workload → **Generally Available (GA)**

------------------------------------------------------------------------

# 🎯 Know These Cold

  If the question says...                 Think...
  --------------------------------------- ---------------------------
  Who are you?                            **Authentication**
  What can you do?                        **Authorization / RBAC**
  Rules for Azure resources               **Azure Policy**
  Prevent deletion                        **Resource Lock**
  Organize resources                      **Tags**
  Monitor metrics/logs                    **Azure Monitor**
  Recommendations                         **Azure Advisor**
  Azure outage/maintenance                **Azure Service Health**
  Secrets/keys/certificates               **Azure Key Vault**
  Multiple security layers                **Defense in Depth**
  Never trust, always verify              **Zero Trust**
  Event-driven code                       **Azure Functions**
  Web app without server management       **Azure App Service**
  Full OS control                         **Azure Virtual Machine**
  Extend Azure management outside Azure   **Azure Arc**
  Infrastructure as code                  **ARM Template**
  Estimate Azure price                    **Pricing Calculator**
  Compare on-premises costs with Azure    **TCO Calculator**

------------------------------------------------------------------------

## Final Review Tip

When reviewing these tables, do not focus only on definitions. Practice
identifying the **Azure service or concept that best fits a scenario**.
AZ-900 questions often provide a business requirement and ask you to
select the most appropriate Azure solution.
