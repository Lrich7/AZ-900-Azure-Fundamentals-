[Lesson-08-Compute.md](https://github.com/user-attachments/files/31148642/Lesson-08-Compute.md)

# Lesson 8 — Compute

## 📖 Microsoft Learn

**Module:** Azure Compute Fundamentals  
https://learn.microsoft.com/en-us/training/modules/azure-compute-fundamentals/

### Focus
- Virtual Machines (VMs)
- Virtual Machine Scale Sets
- Azure App Service
- Azure Functions
- Containers
- Azure Kubernetes Service (AKS)

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Describe the Resources Required for Virtual Machines | 6:17 | https://youtu.be/PP5BWZ0cAJo |
| Benefits and Usage of Core Compute Resources | 34:32 | https://youtu.be/yKDSAYDLGrI |

---

# Azure Compute

Azure provides several compute services for running applications, virtual machines, code, and containers.

The right service depends on how much control you need and how much infrastructure you want Azure to manage.

---

# Azure Virtual Machines

**Azure Virtual Machines (VMs)** are software-based computers running in Azure. They provide compute capacity, memory, storage, and networking without requiring you to purchase physical hardware.

## Key Features
- Windows Server and Linux operating systems
- Flexible VM sizes for different workloads
- Pay-as-you-go compute options
- OS-level control

## Common Uses
- Migrating traditional applications
- Development and testing
- Workloads requiring operating-system access
- Custom server configurations

### Real-World Thinking
If an application requires Windows Server and administrators need control over the operating system, an Azure VM is a good fit.

### Exam Thinking
> **Azure Virtual Machines = IaaS**

---

# Virtual Machine Scale Sets

**Azure Virtual Machine Scale Sets (VMSS)** let you create and manage groups of load-balanced virtual machines that can scale based on demand or schedules.

## Key Features
- Automatic scaling
- High availability options
- Large groups of VM instances
- Flexible or Uniform orchestration modes
- Pay for the underlying compute, storage, and networking resources used

### Real-World Thinking
If a website needs more VM instances during heavy traffic, a Scale Set can increase capacity and reduce it again when demand drops.

### Exam Thinking
> **Virtual Machine Scale Sets = groups of VMs that can automatically scale.**

---

# Azure App Service

**Azure App Service** is a fully managed Platform as a Service (PaaS) for hosting web apps, REST APIs, and mobile backends without managing the underlying servers.

## Core Features
- Managed infrastructure
- Windows and Linux hosting
- Built-in runtimes for common development languages
- CI/CD integration
- Multiple pricing and scaling options

### Real-World Thinking
A development team can deploy a web application while Azure handles much of the server and operating-system management.

### Exam Thinking
> **Azure App Service = PaaS**

Think **web application without managing the server**.

---

# Azure Functions

**Azure Functions** is a serverless compute service for running event-triggered code without managing servers.

## Key Features
- Serverless compute
- Event-driven execution
- Automatic scaling options
- Multiple supported programming languages

Functions can respond to events such as:
- HTTP requests
- Timers
- Queues
- Storage or database changes

### Real-World Thinking
Instead of maintaining a VM for a small task, a Function can run only when a particular event occurs.

### Exam Thinking
> **Azure Functions = Serverless / FaaS**

---

# Serverless: Functions and Logic Apps

## Azure Functions
**Code-first:** Run code in response to events.

## Azure Logic Apps
**Workflow-first:** Build automated workflows using a visual designer and connectors.

### Easy Way to Remember

```text
Azure Functions = Run CODE
Azure Logic Apps = Build WORKFLOWS
```

---

# Containers

Containers package code, configuration, and dependencies into lightweight, portable units.

Azure provides several container services.

## Azure Container Instances (ACI)
Simple, on-demand container execution without managing VMs or a Kubernetes orchestrator.

## Azure Container Apps (ACA)
A managed/serverless container platform suited to applications and microservices.

## Azure Kubernetes Service (AKS)
Managed Kubernetes for orchestrating containerized applications.

## Azure Container Registry (ACR)
A private registry for building, storing, and managing container images.

### Exam Thinking
> **ACI = simple container execution**  
> **AKS = managed Kubernetes orchestration**

---

# Azure Kubernetes Service (AKS)

**Azure Kubernetes Service (AKS)** is a managed service for deploying and managing containerized applications with Kubernetes.

## Key Features
- Microsoft-managed control plane
- Scaling capabilities
- Role-based access and security features
- Integration with development and monitoring tools

### Real-World Thinking
If an organization has many containerized microservices that need Kubernetes orchestration, AKS is designed for that workload.

### Exam Thinking
> **AKS = managed Kubernetes service.**

---

# Comparing Azure Compute Services

| Service | Best Fit | Model / Type |
|---|---|---|
| **Azure Virtual Machines** | OS-level control and traditional server workloads | IaaS |
| **Virtual Machine Scale Sets** | Automatically scaling groups of VMs | IaaS |
| **Azure App Service** | Managed web apps and APIs | PaaS |
| **Azure Functions** | Event-driven code | Serverless / FaaS |
| **Azure Container Instances** | Simple on-demand containers | Container Service |
| **Azure Kubernetes Service** | Kubernetes orchestration | Managed Kubernetes |

### Easy Way to Remember

```text
VM       = I need a SERVER
VMSS     = I need MANY SCALING VMs
App      = I need to HOST A WEB APP
Function = I need to RUN CODE ON AN EVENT
ACI      = I need to RUN A CONTAINER
AKS      = I need to ORCHESTRATE CONTAINERS
```

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 08 Lab — Compute](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-08-Lab-08-Compute.md)**

### Lab Focus
- Create or configure a Windows Virtual Machine exercise.
- Explore Virtual Machine Scale Sets.
- Explore Azure App Service.
- Explore Azure Functions.
- Explore Azure Container Instances.
- Explore Azure Kubernetes Service.
- Compare when each compute service should be used.

> [!TIP]
> Portal exploration, resource creation, and other hands-on activities are kept in the separate lab.

---

# Quick Check

| Service | Model / Type |
|---|---|
| Azure Virtual Machines | IaaS |
| Azure Virtual Machine Scale Sets | IaaS |
| Azure App Service | PaaS |
| Azure Functions | Serverless / FaaS |
| Azure Container Instances | Container Service |
| Azure Kubernetes Service | Managed Kubernetes |

---

# Before Moving On

You should be able to:
- Explain when to use Azure Virtual Machines.
- Explain the purpose of Virtual Machine Scale Sets.
- Explain Azure App Service.
- Explain Azure Functions and serverless computing.
- Explain Azure Container Instances vs. Azure Kubernetes Service.
- Know which Azure compute services are IaaS and which are PaaS.
- Choose an appropriate compute service from a basic scenario.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Virtual Machine** | IaaS; OS-level control |
| **VM Scale Set** | Automatically scaling group of VMs |
| **App Service** | PaaS for web apps/APIs |
| **Azure Functions** | Serverless event-driven code |
| **ACI** | Simple container execution |
| **AKS** | Managed Kubernetes |
| **Logic Apps** | Serverless workflow automation |
