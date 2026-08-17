# Lab 08 — Compute

## Objective

This lab reinforces **Lesson 8 — Compute**.

By the end, you should be able to:
- Explore the creation of a Windows Virtual Machine.
- Explore Virtual Machine Scale Sets.
- Explore Azure App Service.
- Explore Azure Functions.
- Explore Azure Container Instances.
- Explore Azure Kubernetes Service.
- Compare the purpose of the major Azure compute services.

---

## Prerequisites
- Completed **Lesson 8 — Compute**
- Web browser
- Azure account if completing resource-creation activities

### Start Here
- **Azure Portal:** https://portal.azure.com/
- **Azure Compute Fundamentals:** https://learn.microsoft.com/en-us/training/modules/azure-compute-fundamentals/
- **Create a Windows VM:** https://learn.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-portal

> [!IMPORTANT]
> Creating a Virtual Machine can create billable resources. You can complete the learning portion by reviewing the creation screens and stop before deployment if you do not want to incur charges.

---

# Part 1 — Explore a Windows Virtual Machine

### Links
- **Azure Portal:** https://portal.azure.com/
- **Create a Windows VM:** https://learn.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-portal
- **Virtual Machines Documentation:** https://learn.microsoft.com/en-us/azure/virtual-machines/

## Steps
1. Open the Microsoft Windows VM quickstart.
2. Open the Azure Portal.
3. Search for **Virtual machines**.
4. Select **Create** and review the VM creation options.
5. Follow the current Microsoft quickstart if you want to complete the deployment.
6. Pay attention to:
   - Subscription
   - Resource Group
   - VM name
   - Region
   - Availability options
   - Operating system image
   - VM size
   - Administrator account
   - Networking
7. If you do not want to create billable resources, stop before deployment.

## Think About It
Why is an Azure VM considered IaaS?

**Answer:** _______________________________________________

Who manages the guest operating system?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure Virtual Machine = IaaS**

---

# Part 2 — Explore Virtual Machine Scale Sets

### Links
- **Azure Portal:** https://portal.azure.com/
- **VM Scale Sets Overview:** https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview

## Steps
1. Search the Azure Portal for **Virtual machine scale sets**.
2. Open the service.
3. Review the creation options without deploying a Scale Set.
4. Look for settings related to VM instances, scaling, availability, and networking.

## Think About It
How is a Scale Set different from one VM?

**Answer:** _______________________________________________

Why is autoscaling useful?

**Answer:** _______________________________________________

### Exam Thinking
> **VM Scale Set = scalable group of virtual machines.**

---

# Part 3 — Explore Azure App Service

### Links
- **Azure Portal:** https://portal.azure.com/
- **App Service Overview:** https://learn.microsoft.com/en-us/azure/app-service/overview

## Steps
1. Search for **App Services**.
2. Open the service.
3. Review the creation options without deploying.
4. Look for runtime, operating system, region, and App Service plan choices.

## Think About It
Why would a developer choose App Service instead of a VM?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure App Service = PaaS**

---

# Part 4 — Explore Azure Functions

### Links
- **Azure Portal:** https://portal.azure.com/
- **Azure Functions Overview:** https://learn.microsoft.com/en-us/azure/azure-functions/functions-overview

## Steps
1. Search for **Function App**.
2. Review the available creation options.
3. Do not deploy a resource for this exercise.
4. Review examples of triggers in the documentation.

## Think About It
What makes Azure Functions serverless?

**Answer:** _______________________________________________

Name one event that could trigger a Function.

**Answer:** _______________________________________________

### Exam Thinking
> **Azure Functions = Serverless / FaaS**

---

# Part 5 — Explore Azure Container Instances

### Links
- **Azure Portal:** https://portal.azure.com/
- **ACI Overview:** https://learn.microsoft.com/en-us/azure/container-instances/container-instances-overview

## Steps
1. Search for **Container instances**.
2. Open the service.
3. Review the creation options without deploying.
4. Review Microsoft's ACI overview.

## Think About It
Does ACI require you to manage a Kubernetes cluster?

**Answer:** _______________________________________________

### Exam Thinking
> **ACI = simple, on-demand container execution.**

---

# Part 6 — Explore Azure Kubernetes Service

### Links
- **Azure Portal:** https://portal.azure.com/
- **AKS Overview:** https://learn.microsoft.com/en-us/azure/aks/what-is-aks

## Steps
1. Search for **Kubernetes services**.
2. Open the service.
3. Review the creation options without deploying a cluster.
4. Review the AKS overview.
5. Look for concepts involving clusters, nodes, pods, scaling, and the managed control plane.

## Think About It
When would AKS make more sense than ACI?

**Answer:** _______________________________________________

### Exam Thinking
> **AKS = managed Kubernetes orchestration.**

---

# Part 7 — Compare the Compute Services

| Scenario | Best Azure Compute Service |
|---|---|
| Need OS-level control | __________________ |
| Need a group of VMs that can automatically scale | __________________ |
| Need to host a web application without managing servers | __________________ |
| Need code to run when an event occurs | __________________ |
| Need to quickly run a container without Kubernetes | __________________ |
| Need Kubernetes orchestration | __________________ |

---

# Part 8 — Real-World Scenarios

1. An existing Windows Server application needs administrator access to the OS.  
   **Answer:** ______________________________

2. A VM-based website needs more VM instances automatically during heavy traffic.  
   **Answer:** ______________________________

3. A developer wants to host a web API without maintaining the server.  
   **Answer:** ______________________________

4. Code should execute whenever an item is added to a queue.  
   **Answer:** ______________________________

5. A developer needs to run a container without managing Kubernetes.  
   **Answer:** ______________________________

6. A company needs Kubernetes to coordinate many containerized microservices.  
   **Answer:** ______________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Service Review
- **Azure Virtual Machines:** IaaS and OS-level control.
- **Virtual Machine Scale Sets:** Groups of VMs that can scale.
- **Azure App Service:** PaaS for managed web applications and APIs.
- **Azure Functions:** Serverless/FaaS for event-driven code.
- **Azure Container Instances:** Simple container execution without Kubernetes management.
- **Azure Kubernetes Service:** Managed Kubernetes orchestration.

## Part 7

| Scenario | Answer |
|---|---|
| Need OS-level control | Azure Virtual Machines |
| Need automatically scaling VMs | Virtual Machine Scale Sets |
| Host a web application without managing servers | Azure App Service |
| Run code when an event occurs | Azure Functions |
| Run a container without Kubernetes | Azure Container Instances |
| Need Kubernetes orchestration | Azure Kubernetes Service |

## Part 8

| Scenario | Answer |
|---|---|
| 1 | Azure Virtual Machines |
| 2 | Virtual Machine Scale Sets |
| 3 | Azure App Service |
| 4 | Azure Functions |
| 5 | Azure Container Instances |
| 6 | Azure Kubernetes Service |

</details>

---

# Lab Cleanup

If you created a Windows VM or other resources during this lab, remove the lab resources when finished unless you intentionally want to keep them.

### Links
- **Manage Resource Groups:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal
- **Azure Portal:** https://portal.azure.com/

> [!CAUTION]
> Verify a Resource Group contains only lab resources before deleting it. Deleting the Resource Group deletes all resources inside it.

---

# Lab Complete

Before moving on, make sure you can explain:
- VM vs. App Service.
- VM vs. Virtual Machine Scale Sets.
- App Service vs. Azure Functions.
- ACI vs. AKS.
- Which service best fits a basic compute scenario.
