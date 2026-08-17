[Lesson-17-Lab-17-Governance-and-Compliance.md](https://github.com/user-attachments/files/31150649/Lesson-17-Lab-17-Governance-and-Compliance.md)
# Lab 17 — Governance & Compliance

## Objective

This lab reinforces **Lesson 17 — Governance & Compliance**.

Unlike many Azure labs, this exercise is primarily about **research, navigation, and recognizing the correct governance or compliance resource**.

By the end, you should be able to:

- Review the Azure governance hierarchy.
- Explore the Cloud Adoption Framework.
- Browse Microsoft Purview.
- Browse the Microsoft Trust Center.
- Locate Azure compliance information.
- Review sovereign Azure environments.
- Distinguish governance, compliance, privacy, and legal resources.
- Apply the concepts to AZ-900 scenarios.

---

# Prerequisites

- Completed **Lesson 17 — Governance & Compliance**
- Web browser
- Microsoft Learn access

An Azure subscription is not required for most of this lab.

---

# Part 1 — Review the Governance Hierarchy

### Links

- **Azure Resource Manager Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview
- **Management Groups:** https://learn.microsoft.com/en-us/azure/governance/management-groups/overview

Complete the hierarchy:

```text
[ __________________ ]
          |
          v
[ __________________ ]
          |
          v
[ __________________ ]
          |
          v
[ __________________ ]
```

Choose from:

- Management Group
- Subscription
- Resource Group
- Resource

## Questions

Which level can organize multiple subscriptions?

**Answer:** _______________________________________________

Which level acts as a logical container for related resources?

**Answer:** _______________________________________________

Why can applying governance at a higher scope be useful?

**Answer:** _______________________________________________

---

# Part 2 — Explore the Cloud Adoption Framework

### Links

- **Cloud Adoption Framework:** https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/
- **Cloud Adoption Framework Overview:** https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/overview

## Steps

1. Open the Cloud Adoption Framework.
2. Review the main methodologies.
3. Locate information related to:
   - Strategy
   - Plan
   - Ready
   - Adopt
   - Govern
   - Secure
   - Manage
4. Choose one methodology and read its overview.

Complete the table:

| Methodology | Main Idea |
|---|---|
| Strategy | ______________________________ |
| Plan | ______________________________ |
| Ready | ______________________________ |
| Adopt | ______________________________ |
| Govern | ______________________________ |
| Secure | ______________________________ |
| Manage | ______________________________ |

## Think About It

Is the Cloud Adoption Framework primarily a technical enforcement tool or a collection of adoption guidance?

**Answer:** _______________________________________________

### Exam Thinking

> **Cloud Adoption Framework = guidance for the cloud journey.**

---

# Part 3 — Explore Microsoft Purview

### Links

- **Microsoft Purview:** https://learn.microsoft.com/en-us/purview/
- **Microsoft Purview Portal:** https://purview.microsoft.com/

## Steps

1. Open the Microsoft Purview documentation.
2. If your account has appropriate access, browse the Microsoft Purview portal.
3. Do not change company governance or security configurations.
4. Look for concepts involving:
   - Data governance
   - Data catalog
   - Data discovery
   - Classification
   - Data lineage

## Questions

What is Microsoft Purview primarily used for?

**Answer:** _______________________________________________

What is a data catalog useful for?

**Answer:** _______________________________________________

What does data lineage help an organization understand?

**Answer:** _______________________________________________

### Exam Thinking

> **Microsoft Purview = understand and govern organizational data.**

---

# Part 4 — Explore the Microsoft Trust Center

### Links

- **Microsoft Trust Center:** https://www.microsoft.com/en-us/trust-center
- **Service Trust Portal:** https://servicetrust.microsoft.com/

## Steps

1. Open the Microsoft Trust Center.
2. Browse information related to:
   - Security
   - Privacy
   - Compliance
3. Open the Service Trust Portal link.
4. Review the types of compliance and audit resources available.
5. You do not need to download reports for this lab.

## Questions

What type of information is available through the Trust Center?

**Answer:** _______________________________________________

What is the general purpose of the Service Trust Portal?

**Answer:** _______________________________________________

### Exam Thinking

> **Trust Center = Microsoft's security, privacy, and compliance information.**

---

# Part 5 — Explore Azure Compliance Documentation

### Links

- **Azure Compliance:** https://learn.microsoft.com/en-us/azure/compliance/
- **Microsoft Compliance Offerings:** https://learn.microsoft.com/en-us/compliance/regulatory/offering-home

## Steps

1. Open the Azure compliance documentation.
2. Browse the available compliance information.
3. Look for examples of:
   - Global standards
   - Regional requirements
   - Industry-specific requirements
4. Choose one compliance offering and review its overview.

## Questions

Why would an organization review Azure Compliance Documentation before moving a regulated workload to Azure?

**Answer:** _______________________________________________

Does Microsoft's compliance certification automatically make every customer's workload compliant?

**Answer:** _______________________________________________

### Exam Thinking

> **Compliance Documentation = understand Azure's compliance offerings and certifications.**

---

# Part 6 — Review Sovereign Azure Environments

### Links

- **Azure Government:** https://azure.microsoft.com/en-us/explore/global-infrastructure/government
- **Azure Government Documentation:** https://learn.microsoft.com/en-us/azure/azure-government/documentation-government-welcome
- **Azure Geographies:** https://azure.microsoft.com/en-us/explore/global-infrastructure/geographies

## Steps

1. Review the Azure Government information.
2. Read about how specialized Azure environments differ from the public Azure cloud.
3. Look for concepts involving:
   - Government requirements
   - Regulatory requirements
   - Data residency
   - Isolation
4. Do not worry about memorizing every sovereign geography or region.

## Questions

Why might an organization require a sovereign or government cloud environment?

**Answer:** _______________________________________________

What kinds of requirements might influence that decision?

**Answer:** _______________________________________________

### Exam Thinking

> **Sovereign Azure = specialized cloud environments for government, sovereignty, or regulatory requirements.**

---

# Part 7 — Review Privacy and Legal Resources

### Links

- **Microsoft Privacy Statement:** https://privacy.microsoft.com/en-us/privacystatement
- **Microsoft Product Terms:** https://www.microsoft.com/licensing/terms/
- **Microsoft Products and Services Data Protection Addendum:** https://www.microsoft.com/licensing/docs/view/Microsoft-Products-and-Services-Data-Protection-Addendum-DPA

Review the linked resources at a high level.

You do **not** need to read every legal document in full for AZ-900.

Complete the table:

| Resource | Primary Question |
|---|---|
| Microsoft Privacy Statement | ______________________________ |
| Online service / product terms | ______________________________ |
| Data Protection Addendum | ______________________________ |

### Memory Trick

```text
Privacy Statement = PRIVACY PRACTICES
Service Terms     = RULES
DPA               = DATA PROTECTION
```

---

# Part 8 — Azure Blueprints Legacy Review

### Links

- **Azure Blueprints Documentation:** https://learn.microsoft.com/en-us/azure/governance/blueprints/overview
- **Azure Deployment Stacks:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/deployment-stacks

## Review

Azure Blueprints historically allowed organizations to package governance artifacts such as:

- Policy assignments
- RBAC role assignments
- ARM templates
- Resource Groups

Microsoft has announced Azure Blueprints retirement for **January 31, 2027**.

For this course, treat Azure Blueprints as a **legacy governance concept**.

## Questions

What was the basic purpose of Azure Blueprints?

**Answer:** _______________________________________________

Should Azure Blueprints be a major hands-on focus for a current AZ-900 course?

**Answer:** _______________________________________________

---

# Part 9 — Governance & Compliance Scenarios

Choose from:

- **Cloud Adoption Framework**
- **Microsoft Purview**
- **Microsoft Trust Center**
- **Azure Compliance Documentation**
- **Sovereign Azure environment**
- **DPA**

### Scenario 1

A company needs structured guidance for planning and managing its move to Azure.

**Answer:** ______________________________

### Scenario 2

A company needs to discover, classify, and govern data across its environment.

**Answer:** ______________________________

### Scenario 3

A customer wants broad information about Microsoft's security, privacy, and compliance practices.

**Answer:** ______________________________

### Scenario 4

A regulated organization needs to determine which compliance standards Azure supports.

**Answer:** ______________________________

### Scenario 5

A government organization requires a specialized isolated cloud environment.

**Answer:** ______________________________

### Scenario 6

A legal team wants to understand Microsoft's commitments for processing and protecting customer data.

**Answer:** ______________________________

---

# Part 10 — Final Comparison

Complete the table:

| Question | Resource |
|---|---|
| How should we approach our cloud journey? | __________________ |
| How can we discover and govern our data? | __________________ |
| Where can we learn about Microsoft's trust practices? | __________________ |
| What Azure compliance standards are supported? | __________________ |
| Is there a specialized cloud for government requirements? | __________________ |
| How does Microsoft commit to handling customer data? | __________________ |

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

```text
Management Group
      |
Subscription
      |
Resource Group
      |
Resource
```

Management Groups can organize subscriptions. Resource Groups organize related resources. Higher scopes can simplify applying governance consistently across many child resources.

## Part 2

The Cloud Adoption Framework is guidance rather than an Azure resource-enforcement mechanism.

| Methodology | Main Idea |
|---|---|
| Strategy | Define business goals and motivations |
| Plan | Prepare the adoption plan, people, and digital estate |
| Ready | Prepare the Azure environment |
| Adopt | Migrate, modernize, or build workloads |
| Govern | Establish governance and risk controls |
| Secure | Protect cloud assets |
| Manage | Operate and optimize workloads |

## Part 3

Microsoft Purview provides data-governance capabilities. A data catalog helps users discover and understand data assets. Data lineage helps show where data originates and how it moves or changes.

## Part 4

The Trust Center provides information about Microsoft's security, privacy, and compliance practices. The Service Trust Portal provides access to trust, compliance, and audit-related resources.

## Part 5

Organizations use Azure Compliance Documentation to understand Azure's compliance offerings and how they relate to regulatory requirements. Microsoft compliance does not automatically make a customer's own workloads and configurations compliant.

## Part 6

Sovereign or government environments can address specialized government, sovereignty, compliance, isolation, and data-residency requirements.

## Part 7

| Resource | Primary Question |
|---|---|
| Privacy Statement | What are Microsoft's privacy practices? |
| Service Terms | What are the legal/service rules? |
| DPA | How is customer data processed and protected? |

## Part 8

Azure Blueprints provided repeatable governance packages containing artifacts such as Policy, RBAC, templates, and Resource Groups. It is a legacy service and should not be a major current hands-on focus.

## Part 9

| Scenario | Answer |
|---|---|
| 1 | Cloud Adoption Framework |
| 2 | Microsoft Purview |
| 3 | Microsoft Trust Center |
| 4 | Azure Compliance Documentation |
| 5 | Sovereign Azure environment |
| 6 | DPA |

## Part 10

| Question | Answer |
|---|---|
| Approach cloud journey | Cloud Adoption Framework |
| Discover and govern data | Microsoft Purview |
| Microsoft trust practices | Microsoft Trust Center |
| Azure compliance standards | Azure Compliance Documentation |
| Specialized government cloud | Sovereign Azure environment |
| Customer-data commitments | DPA |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Azure's governance hierarchy.
- Cloud Adoption Framework.
- Microsoft Purview.
- Microsoft Trust Center.
- Azure Compliance Documentation.
- Sovereign Azure environments.
- Microsoft Privacy Statement, service terms, and DPA at a high level.
- Why Azure Blueprints is now a legacy concept.
- Which governance or compliance resource best fits a basic AZ-900 scenario.
