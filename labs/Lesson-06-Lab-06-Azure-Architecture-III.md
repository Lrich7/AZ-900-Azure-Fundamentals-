[Lesson-06-Lab-06-Azure-Architecture-III.md](https://github.com/user-attachments/files/31143933/Lesson-06-Lab-06-Azure-Architecture-III.md)
# Lab 06 — Azure Architecture III

## Objective

This lab reinforces **Lesson 6 — Azure Architecture III**.

By the end, you should be able to:

- Explore Azure Resource Manager.
- View and recognize an ARM Template.
- Identify important ARM Template sections.
- Explain Infrastructure as Code.
- Explore Azure Arc.
- Explain how Azure Arc supports hybrid and multi-cloud management.

---

## Prerequisites

- Completed **Lesson 6 — Azure Architecture III**
- Web browser
- Azure account for Azure Portal exploration

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Azure Resource Manager Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview
- **ARM Templates Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/overview
- **Azure Arc Overview:** https://learn.microsoft.com/en-us/azure/azure-arc/overview

> [!NOTE]
> This lab focuses on exploration. You do not need to deploy new paid resources.

---

# Part 1 — Explore Azure Resource Manager

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Resource Manager Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview

## Steps

1. Open the Azure Resource Manager overview.
2. Review how ARM provides a management layer for Azure resources.
3. Open the Azure Portal.
4. Search for **Resource groups**.
5. Open a Resource Group if one is available.
6. Review the resources and management options shown.

If you do not have an existing Resource Group, reviewing the documentation is enough.

## Think About It

What role does Azure Resource Manager play?

**Answer:** _______________________________________________

Is Azure Resource Manager the same thing as an ARM Template?

**Answer:** _______________________________________________

### Exam Thinking

> **ARM = Azure's management and deployment layer.**

---

# Part 2 — View an ARM Template

### Links

- **ARM Templates Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/overview
- **ARM Template Structure:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/syntax
- **Azure Portal:** https://portal.azure.com/

## Option A — Existing Azure Resource

If you have an existing Azure resource:

1. Open the Azure Portal.
2. Open a Resource Group containing a safe test resource.
3. Select the resource.
4. Look for **Export template** or a related template/automation option.
5. Review the generated template if available.
6. Do not redeploy or modify the resource.

## Option B — No Existing Resource

1. Open the **ARM Template Structure** documentation.
2. Review the sample JSON template.
3. Locate the major template sections.

No deployment is required.

---

# Part 3 — Identify ARM Template Sections

### Link

- **ARM Template Structure:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/syntax

Find these sections:

- `$schema`
- `contentVersion`
- `parameters`
- `variables`
- `resources`
- `outputs`

## Record What Each Does

**$schema:** ______________________________________________

**contentVersion:** _______________________________________

**parameters:** ___________________________________________

**variables:** ____________________________________________

**resources:** ____________________________________________

**outputs:** ______________________________________________

### Exam Thinking

```text
parameters = Inputs
variables  = Reusable values
resources  = What gets deployed
outputs    = Returned information
```

---

# Part 4 — Infrastructure as Code

### Links

- **ARM Templates Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/overview
- **Azure Resource Manager Documentation:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/

Review the documentation and compare a template-based deployment with manually creating resources in the Azure Portal.

## Think About It

What is an advantage of storing infrastructure definitions in a file?

**Answer:** _______________________________________________

Why are repeatable templates useful for Development, Testing, and Production?

**Answer:** _______________________________________________

What does **declarative** mean?

**Answer:** _______________________________________________

### Exam Thinking

> **IaC = infrastructure managed and deployed using code instead of only manual configuration.**

---

# Part 5 — Explore Azure Arc

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Arc Overview:** https://learn.microsoft.com/en-us/azure/azure-arc/overview
- **Azure Arc Documentation:** https://learn.microsoft.com/en-us/azure/azure-arc/

## Steps

1. Open the Azure Portal.
2. Search for **Azure Arc**.
3. Open Azure Arc.
4. Review the types of resources and environments shown.
5. Open the Azure Arc Overview documentation.
6. Identify examples of resources Azure Arc can manage outside Azure.

Look for:

- On-premises environments
- Other cloud providers
- Edge locations
- Kubernetes environments

## Think About It

Does Azure Arc require an on-premises resource to be migrated into Azure?

**Answer:** _______________________________________________

What is the main benefit of Azure Arc?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Arc = Azure management beyond Azure.**

---

# Part 6 — Identify the Technology

Choose:

- **Azure Resource Manager**
- **ARM Template**
- **Infrastructure as Code**
- **Azure Arc**

### Scenario 1

An administrator wants a JSON file defining the Azure resources that should be deployed.

**Answer:** ______________________________

### Scenario 2

A company wants to manage supported servers in its on-premises datacenter using Azure management capabilities.

**Answer:** ______________________________

### Scenario 3

A team stores infrastructure definitions in version control and uses them to create consistent environments.

**Answer:** ______________________________

### Scenario 4

An administrator uses Azure's common management layer to organize and manage cloud resources.

**Answer:** ______________________________

---

# Part 7 — Exam Thinking

1. **Azure Resource Manager** = _____________________________
2. **ARM Template** = _____________________________________
3. **Infrastructure as Code** = ____________________________
4. **Azure Arc** = _________________________________________
5. **parameters** = ________________________________________
6. **resources** = _________________________________________
7. **outputs** = ___________________________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

Azure Resource Manager provides Azure's management and deployment layer.

ARM and an ARM Template are related but not the same. ARM is the management layer; an ARM Template is a JSON definition used to describe resources for deployment.

## Part 3

- **$schema:** Points to the schema used to validate the template structure.
- **contentVersion:** Tracks the template version.
- **parameters:** Inputs supplied during deployment.
- **variables:** Reusable values.
- **resources:** Azure resources to deploy.
- **outputs:** Information returned after deployment.

## Part 4

Infrastructure as Code allows infrastructure definitions to be automated, reused, versioned, and standardized.

**Declarative** means describing the desired final state rather than every procedural step.

## Part 5

Azure Arc does not require supported resources to be migrated into Azure. It extends Azure management and governance capabilities to resources outside Azure.

## Part 6

| Scenario | Answer |
|---|---|
| 1 | ARM Template |
| 2 | Azure Arc |
| 3 | Infrastructure as Code |
| 4 | Azure Resource Manager |

## Part 7

- **Azure Resource Manager:** Azure management and deployment layer.
- **ARM Template:** JSON file defining Azure resources to deploy.
- **Infrastructure as Code:** Provisioning and managing infrastructure using code.
- **Azure Arc:** Extends Azure management to supported resources outside Azure.
- **parameters:** Deployment inputs.
- **resources:** Items that should be deployed.
- **outputs:** Information returned after deployment.

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- ARM vs. ARM Template.
- ARM Template vs. Infrastructure as Code.
- The important sections of an ARM Template.
- Why repeatable infrastructure definitions are useful.
- What Azure Arc does.
- Why Azure Arc is useful in hybrid and multi-cloud environments.
