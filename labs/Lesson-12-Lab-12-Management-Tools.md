[Lesson-12-Lab-12-Management-Tools.md](https://github.com/user-attachments/files/31149219/Lesson-12-Lab-12-Management-Tools.md)
# Lab 12 — Management Tools

## Objective

This lab reinforces **Lesson 12 — Management Tools**.

By the end, you should be able to:

- Explore Azure Monitor.
- Review Metrics and Logs.
- Review the Azure Activity Log.
- Explore Azure Advisor.
- Explore Azure Service Health.
- View an ARM Template from an Azure resource when available.
- Identify the correct Azure management tool for common AZ-900 scenarios.

---

## Prerequisites

- Completed **Lesson 12 — Management Tools**
- Web browser
- Azure account with access to the Azure Portal

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Introduction to Azure Management and Governance:** https://learn.microsoft.com/en-us/training/modules/intro-to-azure-management-and-governance/

> [!IMPORTANT]
> This is primarily an exploration lab. Use test resources when possible and do not modify production resources, monitoring rules, or company configurations.

---

# Part 1 — Explore Azure Monitor

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Monitor Overview:** https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/overview

## Steps

1. Open the Azure Portal.
2. Search for **Monitor**.
3. Open **Azure Monitor**.
4. Review the available monitoring areas.
5. Look for options involving:
   - Metrics
   - Logs
   - Alerts
   - Workbooks
   - Activity Log
6. Do not create or change alert rules on production resources.

## Think About It

What type of information does Azure Monitor collect?

**Answer:** _______________________________________________

What is the difference between a metric and a log?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Monitor = metrics, logs, telemetry, and alerts.**

---

# Part 2 — Explore Metrics

### Links

- **Azure Monitor Metrics:** https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/data-platform-metrics
- **Azure Portal:** https://portal.azure.com/

## Steps

1. In Azure Monitor, locate **Metrics**.
2. Select a safe test resource if one is available.
3. Review the available metrics.
4. Look for examples such as CPU, requests, storage, or network activity.
5. Change the time range if available and observe how the chart changes.
6. Do not change production monitoring settings.

## Think About It

Are metrics generally numerical measurements or detailed event records?

**Answer:** _______________________________________________

Give one example of a useful resource metric.

**Answer:** _______________________________________________

---

# Part 3 — Explore Logs

### Links

- **Azure Monitor Logs Overview:** https://learn.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs
- **Log Analytics Overview:** https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-overview

## Steps

1. In Azure Monitor, locate **Logs**.
2. Review the Log Analytics interface if your account has an available workspace or resource.
3. Look at the query interface.
4. Notice that Azure Monitor Logs can use **Kusto Query Language (KQL)**.
5. You do not need to learn KQL syntax for this AZ-900 lab.

## Think About It

What is the purpose of Azure Monitor Logs?

**Answer:** _______________________________________________

Which query language is commonly used with Azure Monitor Logs?

**Answer:** _______________________________________________

### Exam Thinking

> **Metrics = measurements**  
> **Logs = detailed records**

---

# Part 4 — Explore the Azure Activity Log

### Links

- **Azure Activity Log:** https://learn.microsoft.com/en-us/azure/azure-monitor/platform/activity-log

## Steps

1. In Azure Monitor, locate **Activity Log**.
2. Review recent events if your subscription contains activity.
3. Look at fields such as:
   - Operation
   - Status
   - Time
   - Subscription
   - Resource
4. Open a safe event to review additional details.

## Think About It

Would the Activity Log help identify a management operation performed on an Azure resource?

**Answer:** _______________________________________________

What information might help identify when a change occurred?

**Answer:** _______________________________________________

### Exam Thinking

> **Activity Log = subscription-level record of Azure resource management events.**

---

# Part 5 — Explore Azure Advisor

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Advisor Overview:** https://learn.microsoft.com/en-us/azure/advisor/advisor-overview

## Steps

1. Search the Azure Portal for **Advisor**.
2. Open Azure Advisor.
3. Review the recommendations available to your subscription.
4. Look for recommendation categories such as:
   - Cost
   - Security
   - Reliability
   - Performance
   - Operational excellence
5. Do **not** apply recommendations to production resources as part of this lab.

## Think About It

What is Azure Advisor's primary purpose?

**Answer:** _______________________________________________

If Azure recommends resizing an underutilized resource to reduce spending, which recommendation category does that relate to?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Advisor = personalized best-practice recommendations.**

---

# Part 6 — Explore Azure Service Health

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Service Health Overview:** https://learn.microsoft.com/en-us/azure/service-health/overview

## Steps

1. Search the Azure Portal for **Service Health**.
2. Open the service.
3. Review the available sections.
4. Look for:
   - Service issues
   - Planned maintenance
   - Health advisories
5. If available, review **Resource Health** for an individual safe test resource.

## Think About It

Which tool would you use to check whether Microsoft is experiencing an Azure service issue?

**Answer:** _______________________________________________

What is the difference between Service Health and Resource Health?

**Answer:** _______________________________________________

### Exam Thinking

```text
Service Health  = Azure service problems affecting you
Resource Health = Health of an individual resource
```

---

# Part 7 — View an ARM Template

### Links

- **ARM Templates Overview:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/overview
- **Export an ARM Template:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/export-template-portal
- **Azure Portal:** https://portal.azure.com/

## Steps

If you have access to a safe Azure resource:

1. Open the resource in the Azure Portal.
2. Look for an option such as **Export template** or **Automation script**.
3. Open the generated template.
4. Review the JSON without changing or deploying anything.
5. Look for sections describing:
   - Resource type
   - Resource name
   - Properties
   - Parameters

If you do not have an existing resource, review Microsoft's ARM Template documentation instead.

## Think About It

What format are ARM Templates written in?

**Answer:** _______________________________________________

What does **Infrastructure as Code** mean?

**Answer:** _______________________________________________

Why are templates useful for repeated deployments?

**Answer:** _______________________________________________

### Exam Thinking

> **ARM Templates = repeatable Azure infrastructure deployment using JSON.**

---

# Part 8 — Management Tool Scenarios

Choose from:

- **Azure DevOps**
- **Azure Functions**
- **Logic Apps**
- **ARM Templates**
- **Azure Monitor**
- **Azure Advisor**
- **Azure Service Health**

### Scenario 1

A development team needs Git repositories and automated CI/CD pipelines.

**Answer:** ______________________________

### Scenario 2

A small block of code should run whenever a file is uploaded.

**Answer:** ______________________________

### Scenario 3

A company needs a low-code workflow that connects multiple business services.

**Answer:** ______________________________

### Scenario 4

An administrator needs to deploy the same Azure infrastructure repeatedly.

**Answer:** ______________________________

### Scenario 5

An administrator needs to review CPU metrics and application logs.

**Answer:** ______________________________

### Scenario 6

An administrator wants Azure to recommend ways to reduce cost and improve reliability.

**Answer:** ______________________________

### Scenario 7

Users report an Azure application is unavailable and the administrator wants to know whether Microsoft has an active service outage.

**Answer:** ______________________________

---

# Part 9 — Monitor, Advisor, or Service Health?

Choose the best answer:

- **Azure Monitor**
- **Azure Advisor**
- **Azure Service Health**

### Question 1

What is happening with my VM's CPU usage?

**Answer:** ______________________________

### Question 2

How can I improve the cost efficiency of my Azure resources?

**Answer:** ______________________________

### Question 3

Is Azure experiencing a service issue that affects my subscription?

**Answer:** ______________________________

### Memory Trick

```text
Monitor        = OBSERVE
Advisor        = RECOMMEND
Service Health = MICROSOFT / AZURE SERVICE STATUS
```

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

Azure Monitor collects and analyzes telemetry such as metrics and logs and can support alerts and visualization.

## Part 2

Metrics are numerical measurements collected over time. Examples include CPU usage, request counts, storage operations, and network activity.

## Part 3

Logs provide detailed records that can be queried and analyzed. Azure Monitor Logs commonly uses **Kusto Query Language (KQL)**.

## Part 4

Yes. The Activity Log records Azure resource-management events and can help identify operations, status, time, and affected resources.

## Part 5

Azure Advisor provides personalized recommendations. Reducing spending on an underutilized resource relates to **Cost**.

## Part 6

Use **Azure Service Health** to review Azure service issues affecting your environment.

Service Health focuses on Azure service events relevant to subscriptions. Resource Health focuses on the health of an individual resource.

## Part 7

ARM Templates are JSON files that define Azure resources and configurations as code.

Infrastructure as Code means defining infrastructure in code or configuration files so deployments can be automated and repeated consistently.

## Part 8

| Scenario | Answer |
|---|---|
| 1 | Azure DevOps |
| 2 | Azure Functions |
| 3 | Logic Apps |
| 4 | ARM Templates |
| 5 | Azure Monitor |
| 6 | Azure Advisor |
| 7 | Azure Service Health |

## Part 9

| Question | Answer |
|---|---|
| VM CPU usage | Azure Monitor |
| Improve cost efficiency | Azure Advisor |
| Azure service issue | Azure Service Health |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Azure Monitor and the difference between Metrics and Logs.
- Azure Advisor.
- Azure Service Health and Resource Health.
- The Azure Activity Log.
- ARM Templates and Infrastructure as Code.
- Azure DevOps.
- Azure Functions vs. Logic Apps.
- Which Azure management tool best fits a basic AZ-900 scenario.
