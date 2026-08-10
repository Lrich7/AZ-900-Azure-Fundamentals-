## **Day 2 — Cloud Concepts II & Cloud Models**

<br>

# **Different types of Clouds**

<br>

## **Private Cloud**
**Dedicated to the ONE ORG** 
* **A private cloud is a dedicated computing environment used exclusively by a single organization**, such as a bank's internal server network, a hospital's secure patient data system, or a company's private VMware infrastructure.

##
* Complete control over resources and security.
* Data NOT collocated with other tenants.
* Hosted on-premises or in dedicated Datacenter.
* Greater Cost, fewer benefits of the Public Cloud.
* Natural evolution from tradtional Datacenter.
  
##

* **MANAGED BY:** You or Third Party.
* **SINGLE ORG**
---
<br>

## **Public Cloud**
**Provider infrastructure**
* **A public cloud is a service run by a third-party company.** It lets many people and businesses share the same computer hardware over the internet.
* Popular examples include **Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform**, and consumer tools like **Gmail**.

## 
* No Capital expenditures (CAPEX) to scale UP
* Quick Provisioning and Deprovisioning.
* Pay ONLY for what you USE.
* Built, controlled and maintained by Provider.
## 
* **MANAGED BY:** Cloud provider.
* **GENERAL PUBLIC ACCESS**
---

<br>

## **Hybrid Cloud**
**Both Connected**
* **A classic hybrid cloud example** is an **e-commerce store.** The store keeps its **private customer database on its own secure, local computers (on-premises)**.
* During big shopping events like Black Friday, it uses extra computer power from a public cloud like Amazon Web Services to handle the heavy web traffic.

##
* Provides the MOST FLEXIBILIITY
* Control Security Compliance or Legal.
* Surge to Public Cloud for temporary demand.
* Extra layer of Security between environments.
* EXTRA layer of security
##
*  **Managed by:** You and Provider.
*  **Private and Public interconnected.**
---

<br>

## **Multi-Cloud**
**Multiple Providers**

* A **multi-cloud setup** means a company uses public cloud services from **two or more** different vendors—such as **Amazon Web Services (AWS), Google Cloud Platform (GCP), and Microsoft Azure** at the same time.
*  For example, a global online store might run its main website on AWS, use Google Cloud for data analytics and artificial intelligence, and host user identity databases on Microsoft Azure

##
* Multiple public cloud providers.
* Different Features from Different Providers.
* Manage Resources and security across environments.
* Increasingly common deployment scenarios.
* Supports provider migrations scenarios.
##
*  **Managed by:** You and Provider.
*  **2 or More providers connected.**
---

<br>
<br>

---

## **Azure Arc**

* Microsoft service that lets you manage resources across **Private, Public, Hybrid, and Multi-Cloud** environments.
* Acts as a bridge between Azure and resources running outside of Azure.
* Allows you to manage on-premises servers, edge devices, and resources in other cloud providers (such as AWS and Google Cloud) directly from the Azure portal.
* Extends Azure management and governance to resources regardless of where they are hosted.

> [!NOTE]
> **Remember:** Azure Arc does **not** move your resources into Azure. It simply allows Azure to manage resources that already exist outside of Azure.

```text
                    Azure Portal
                         │
        ┌────────────────┼────────────────┐
        │                │                │
   On-Premises       AWS / Google Cloud   Edge Devices
      Servers             VMs/Kubernetes       IoT
        │                │                │
        └──────────── Azure Arc ──────────┘
```

---

### **What Azure Arc Can Manage**

* **Servers and Virtual Machines:** Windows and Linux machines running on-premises, VMware vSphere, Hyper-V, or other cloud providers.
* **Kubernetes Clusters:** Connect and centrally manage Kubernetes clusters running anywhere.
* **Databases:** Deploy and manage Azure SQL Managed Instance and SQL Server outside of Azure.
* **Azure Services:** Extend selected Azure services to hybrid and multi-cloud environments.

---

### **Core Benefits**

* **One Control Plane:** Manage Azure and non-Azure resources from a single Azure portal.
* **Centralized Governance:** Apply Azure Policy, Role-Based Access Control (RBAC), and resource tagging consistently across all environments.
* **Improved Security:** Use Microsoft Defender for Cloud to monitor and protect hybrid resources.
* **Azure Management Services:** Enable services such as Azure Monitor, Update Manager, and Change Tracking for resources outside Azure.
* **No Additional Azure Arc Management Cost:** Basic Azure Arc server management features are included at no extra charge (additional Azure services may have their own pricing).

---

### **Exam Tip**

✅ **Azure Arc = Manage resources anywhere**

Azure Arc extends Azure's management capabilities to:
- On-premises datacenters
- Other cloud providers (AWS, Google Cloud)
- Edge locations

It **does not** migrate resources into Azure—it only allows Azure to manage them.

<br>

---

## **Azure VMware Solution (AVS)**

* Microsoft service that lets you run **VMware environments natively in Azure**.
* Allows you to migrate existing VMware workloads to Azure with **little or no changes**.
* Uses the same VMware tools administrators already know, making migration easier.
* Ideal for organizations that want to move to Azure without redesigning their applications.

> [!NOTE]
> **Remember:** Azure VMware Solution runs **VMware in Azure**, not Azure virtual machines that happen to have VMware installed.

```text
          On-Premises VMware
      (vSphere • vCenter • vSAN)
                 │
          Lift and Shift
                 │
                 ▼
     Azure VMware Solution (AVS)
                 │
      Managed by Microsoft
                 │
        Connected to Azure Services
```

---

### **Core Components**

* **Private Cloud:** Dedicated VMware environment hosted on Azure infrastructure.
* **VMware Software:** Includes familiar VMware tools such as **vSphere**, **vCenter Server**, **vSAN**, and **NSX**.
* **Microsoft-Managed Infrastructure:** Microsoft manages the physical hardware, networking, and platform updates.
* **Azure Integration:** Easily connect VMware workloads to Azure services like Azure Backup, Azure Monitor, Azure Storage, and Microsoft Defender for Cloud.

---

### **Core Benefits**

* **Lift-and-Shift Migration:** Move existing VMware virtual machines to Azure with minimal changes.
* **Familiar Management:** Continue using VMware tools and existing administrator skills.
* **Hybrid Cloud:** Connect on-premises VMware environments with Azure.
* **Business Continuity:** Use Azure for disaster recovery, backup, and high availability.
* **Scalability:** Increase or decrease resources without purchasing additional on-premises hardware.

---

### **Common Use Cases**

* Migrate an existing VMware datacenter to Azure.
* Expand on-premises capacity without buying more hardware.
* Create a disaster recovery environment in Azure.
* Modernize applications gradually while continuing to run VMware workloads.

---

### **Exam Tip**

✅ **Azure VMware Solution = VMware running in Azure**

Think:

- Existing VMware environment ✔️
- Minimal application changes ✔️
- Same VMware management tools ✔️
- Microsoft manages the infrastructure ✔️
