[Lesson-03-Cloud-Service-Models.md](https://github.com/user-attachments/files/31077248/Lesson-03-Cloud-Service-Models.md)
# Lesson 3 — Cloud Service Models

## 📖 Microsoft Learn

**Module:** Describe Cloud Service Types  
https://learn.microsoft.com/en-us/training/modules/describe-cloud-service-types/

### Focus
- Infrastructure as a Service (IaaS)
- Platform as a Service (PaaS)
- Software as a Service (SaaS)
- Choosing the appropriate cloud service model

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Differences Between Cloud Service Categories (IaaS / PaaS / SaaS) | 15:16 | https://youtu.be/IqQC1EOQqeU |
| Identify the Right Service Type | 4:01 | https://youtu.be/KH8NH76h2vc |

---

# Cloud Service Models

Cloud service models describe how much of the technology stack is managed by you and how much is managed by the cloud provider.

```text
More Customer Management
          ▲
          │
        IaaS
          │
        PaaS
          │
        SaaS
          │
          ▼
More Provider Management
```

# Infrastructure as a Service (IaaS)

**IaaS** provides core infrastructure such as servers, storage, and networking over the internet.

## Key Components
- **Compute:** Virtual machines and virtual CPUs.
- **Storage:** Resources used to hold data.
- **Networking:** Virtual networks, routers, and firewalls.

## Main Benefits
- No need to purchase physical servers.
- Scale resources based on demand.
- Greater control over the operating system and applications.
- Provider manages the physical infrastructure.

## Real-World Examples
- Microsoft Azure Virtual Machines
- Amazon EC2
- Google Compute Engine
- DigitalOcean Droplets

### Real-World Thinking
Think of IaaS as **renting the computer instead of buying the computer**. You still manage much of what runs on it.

### Exam Thinking
> **IaaS = Most customer control and management responsibility of the three primary service models.**

**Azure Virtual Machines = IaaS**

---

# Platform as a Service (PaaS)

**PaaS** provides a managed environment for building, testing, deploying, and managing applications without requiring the customer to manage the underlying servers.

## Key Components
- **Development Tools**
- **Middleware**
- **Managed Operating Systems**

## Main Benefits
- Focus on application development.
- Less infrastructure management.
- Provider handles operating-system maintenance.
- Easier deployment and scaling.

## Real-World Examples
- Azure App Service
- Azure SQL Database
- AWS Elastic Beanstalk
- Google App Engine
- Heroku

### Real-World Thinking
**You bring the application. The provider manages the platform underneath it.**

### Exam Thinking
> **PaaS = Build and deploy applications without managing the underlying operating system or infrastructure.**

- **Azure App Service = PaaS**
- **Azure SQL Database = PaaS**

---

# Software as a Service (SaaS)

**SaaS** provides a complete application over the internet.

## Key Components
- **Web Delivery**
- **Subscription Model**
- **Central Management**

## Main Benefits
- Little or no installation required.
- Provider manages application updates.
- Provider maintains the underlying infrastructure.
- Minimal technical management for the customer.

## Real-World Examples
- Microsoft 365
- Google Workspace
- Salesforce

### Real-World Thinking
**You simply use the finished software.**

### Exam Thinking
> **SaaS = Finished software managed by the provider and used by the customer.**

**Microsoft 365 = SaaS**

---

# IaaS vs. PaaS vs. SaaS

| Service Model | You Primarily Manage | Provider Primarily Manages | Example |
|---|---|---|---|
| **IaaS** | OS, applications, data and configuration | Physical infrastructure | Azure Virtual Machines |
| **PaaS** | Applications and data | Infrastructure, OS and platform | Azure App Service |
| **SaaS** | Users, data and configuration | Application and underlying platform | Microsoft 365 |

### Easy Way to Remember

```text
IaaS = Manage the MOST
PaaS = Manage the APPLICATION
SaaS = USE the SOFTWARE
```

---

# Azure Functions and Serverless

**Azure Functions** is a serverless compute service, commonly described as **Function as a Service (FaaS)**.

### Real-World Thinking
Instead of creating and maintaining a VM to run a small piece of code, Azure Functions can run that code when an event occurs.

### Exam Thinking
> **Azure Functions = Serverless / FaaS**

The key idea is that **you do not manage the servers**.

---

# Choosing the Right Service Model

### Choose IaaS when:
- You need control over the operating system.
- You need traditional virtual machines.
- You are migrating server workloads.

### Choose PaaS when:
- You want to focus on applications instead of servers.
- You do not want to maintain operating systems.
- You want a managed application or database platform.

### Choose SaaS when:
- You need a finished application.
- You do not need to manage application infrastructure.
- Users simply need access to the software.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 03 Lab — Cloud Service Models](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-03-Lab-03-Cloud-Service-Models.md)**

### Lab Focus
- Explore Azure Virtual Machines.
- Explore Azure App Service.
- Explore Azure Functions.
- Explore Azure SQL Database.
- Identify the service model associated with each service.
- Compare customer versus provider management responsibilities.

> [!TIP]
> The lab is primarily an Azure Portal exploration exercise. You do not need to deploy paid resources.

---

# Quick Check

| Azure Service | Service Model |
|---|---|
| Azure Virtual Machines | IaaS |
| Azure App Service | PaaS |
| Azure Functions | Serverless (FaaS) |
| Azure SQL Database | PaaS |
| Microsoft 365 | SaaS |

---

# Before Moving On

You should be able to:
- Explain the differences between IaaS, PaaS, and SaaS.
- Identify the service model from a service or scenario.
- Explain when each service model is appropriate.
- Recognize Azure Virtual Machines as IaaS.
- Recognize Azure App Service and Azure SQL Database as PaaS.
- Recognize Azure Functions as serverless/FaaS.
- Recognize Microsoft 365 as SaaS.
- Explain how management responsibility changes between IaaS, PaaS, and SaaS.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **IaaS** | Infrastructure provided by the cloud; customer manages more |
| **PaaS** | Managed platform for building and running applications |
| **SaaS** | Finished software delivered over the internet |
| **Azure VM** | IaaS |
| **Azure App Service** | PaaS |
| **Azure SQL Database** | PaaS |
| **Azure Functions** | Serverless / FaaS |
| **Microsoft 365** | SaaS |
| **Management Responsibility** | Decreases from IaaS → PaaS → SaaS |
