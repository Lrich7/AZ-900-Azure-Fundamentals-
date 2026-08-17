[Lesson-06-Azure-Architecture-III.md](https://github.com/user-attachments/files/31148615/Lesson-06-Azure-Architecture-III.md)

# Lesson 6 — Azure Architecture III

## 📖 Microsoft Learn

**Azure Resource Manager Documentation**  
https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview

**Azure Arc Overview**  
https://learn.microsoft.com/en-us/azure/azure-arc/overview

### Focus
- Azure Resource Manager (ARM)
- Azure Resource Manager Templates
- Infrastructure as Code (IaC)
- Azure Arc

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Azure Resource Manager | 9:57 | https://youtu.be/g4u0NL2-3XM |
| Describe the Purpose of Azure Arc | 7:23 | https://youtu.be/cW6_rvDYSHg |

---

# Azure Resource Manager (ARM)

**Azure Resource Manager (ARM)** is Azure's management layer for creating, updating, organizing, and deleting Azure resources.

When you perform management actions through tools such as the Azure Portal, those requests are handled through Azure Resource Manager.

### Real-World Thinking

ARM provides a common management layer instead of every Azure service having a completely separate management system.

### Exam Thinking

> **Azure Resource Manager = Azure's management and deployment layer for resources.**

Do not confuse **Azure Resource Manager** with an **ARM Template**.

---

# ARM Templates

An **Azure Resource Manager Template**, commonly called an **ARM Template**, is a JSON file that defines the Azure resources you want to deploy and their configurations.

ARM Templates allow infrastructure to be deployed consistently, repeatedly, and automatically.

```text
ARM Template
     |
     v
Azure Resource Manager
     |
     v
Azure Resources
```

## Declarative Deployment

ARM Templates use a **declarative** format.

You describe **what you want the final environment to look like**, rather than writing every individual step required to create it.

### Real-World Thinking

Instead of manually creating the same virtual network, storage account, and other resources repeatedly, an administrator can define the infrastructure in a template and reuse it.

### Exam Thinking

> **ARM Template = JSON file that defines what Azure resources should be deployed.**

---

# Key Sections of an ARM Template

| Section | Purpose |
|---|---|
| **$schema** | Points to the schema used to validate the JSON structure |
| **contentVersion** | Tracks the template version |
| **parameters** | Inputs that can change between deployments |
| **variables** | Reusable values inside the template |
| **resources** | Azure resources that should be deployed |
| **outputs** | Information returned after deployment |

### Easy Way to Remember

```text
$schema        = Validate structure
contentVersion = Template version
parameters     = Inputs
variables      = Reusable values
resources      = What gets created
outputs        = Returned information
```

---

# Benefits of ARM Templates

## Repeatable
The same template can build the same type of environment multiple times.

## Organized
Multiple related resources can be defined and deployed together.

## Idempotent
Repeated deployments work toward the desired state defined by the template.

### Real-World Thinking

The same infrastructure definition could be reused for:

```text
Development
Testing
Production
```

with different parameter values for each environment.

### Exam Thinking

> **ARM Templates help make Azure deployments consistent and repeatable.**

---

# Infrastructure as Code (IaC)

**Infrastructure as Code (IaC)** is the practice of provisioning and managing infrastructure using code or configuration files instead of manually configuring resources through a graphical interface.

## Main Benefits

- Automates infrastructure deployment.
- Helps standardize environments.
- Reduces repetitive manual configuration.
- Allows infrastructure definitions to be stored in version control.
- Helps create consistent Development, Testing, and Production environments.

### Real-World Thinking

An infrastructure template stored in GitHub can be reviewed, versioned, changed, and reused similarly to application code.

### Exam Thinking

> **Infrastructure as Code = use code to automate and standardize infrastructure deployments.**

ARM Templates are one way to implement Infrastructure as Code in Azure.

---

# Azure Arc

**Azure Arc** extends Azure's management and governance capabilities beyond Azure.

It allows supported resources outside Azure to be managed using Azure management tools.

Examples include resources in:

- On-premises datacenters
- Other cloud providers
- Edge locations
- Kubernetes environments

```text
                    Azure
                      |
                  Azure Arc
                      |
        +-------------+-------------+
        |             |             |
    On-Premises   Other Clouds     Edge
```

Azure Arc can provide a unified way to apply policies, security, monitoring, and management across hybrid and multi-cloud environments.

### Real-World Thinking

A company can keep supported servers in its own datacenter while using Azure Arc to extend Azure management capabilities to them.

### Exam Thinking

> **Azure Arc = extends Azure management to resources outside Azure.**

> **Azure Arc does not mean the resource has been migrated into Azure.**

---

# ARM vs. ARM Templates vs. IaC vs. Azure Arc

| Concept | Purpose |
|---|---|
| **Azure Resource Manager** | Management and deployment layer for Azure resources |
| **ARM Template** | JSON definition of Azure resources to deploy |
| **Infrastructure as Code** | Practice of managing infrastructure using code |
| **Azure Arc** | Extends Azure management to supported resources outside Azure |

### Easy Way to Remember

```text
ARM          = Manage Azure resources
ARM Template = Define resources with JSON
IaC          = Infrastructure defined as code
Azure Arc    = Manage beyond Azure
```

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 06 Lab — Azure Architecture III](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-06-Lab-06-Azure-Architecture-III.md)**

### Lab Focus

- Explore Azure Resource Manager.
- View an ARM Template.
- Identify important ARM Template sections.
- Explore Azure Arc.
- Review Azure Arc documentation.
- Practice identifying ARM, ARM Templates, IaC, and Azure Arc.

> [!TIP]
> All hands-on activities for this lesson are kept in the separate lab file.

---

# Quick Check

| Question | Answer |
|---|---|
| Azure management and deployment layer | Azure Resource Manager |
| JSON file defining Azure resources | ARM Template |
| Managing infrastructure using code | Infrastructure as Code |
| Extends Azure management outside Azure | Azure Arc |
| Template section containing deployable items | resources |
| Template section used for deployment inputs | parameters |

---

# Before Moving On

You should be able to:

- Explain what Azure Resource Manager does.
- Explain the purpose of ARM Templates.
- Explain what Infrastructure as Code means.
- Identify the major sections of an ARM Template.
- Explain what Azure Arc is.
- Explain which types of environments Azure Arc can help manage.
- Explain the benefits of hybrid and multi-cloud management with Azure Arc.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **ARM** | Azure management and deployment layer |
| **ARM Template** | JSON file defining resources to deploy |
| **Declarative** | Describe the desired result |
| **IaC** | Infrastructure managed using code |
| **parameters** | Deployment inputs |
| **variables** | Reusable template values |
| **resources** | Azure items to deploy |
| **outputs** | Information returned after deployment |
| **Azure Arc** | Extends Azure management beyond Azure |
