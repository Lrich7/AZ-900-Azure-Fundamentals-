[Lesson-12-Management-Tools.md](https://github.com/user-attachments/files/31148777/Lesson-12-Management-Tools.md)

# Lesson 12 — Management Tools

## 📖 Microsoft Learn

**Module:** Introduction to Azure Management and Governance  
https://learn.microsoft.com/en-us/training/modules/intro-to-azure-management-and-governance/

### Focus
- Serverless Computing
- Azure DevOps
- Azure Monitor
- Azure Advisor
- ARM Templates
- Azure Service Health

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Serverless Technologies | 6:54 | https://youtu.be/-xeJGiMw5OE |
| Benefits and Usage of DevOps Technologies | 10:21 | https://youtu.be/-acpNiCa0qY |
| Functionality of Azure Management Solutions | 9:23 | https://youtu.be/6xp-K60ChAk |
| Functionality and Usage of Azure Advisor | 3:22 | https://youtu.be/nqH4NboyEl0 |
| Functionality and Usage of ARM Templates | 6:41 | https://youtu.be/loxcA5MUf-I |
| Functionality and Usage of Azure Monitor | 10:20 | https://youtu.be/v68jL-l9Fww |
| Functionality and Usage of Azure Service Health | 2:58 | https://youtu.be/M1xPK4T4Vls |

---

# Azure Management Tools

Azure provides tools for developing, deploying, monitoring, optimizing, and maintaining cloud resources.

For AZ-900, focus on the **primary purpose** of each tool and recognizing which tool best fits a basic scenario.

---

# Serverless Computing

**Serverless computing** allows applications to run code or workflows without requiring the customer to manage the underlying servers.

Two important Azure serverless services are:

- Azure Functions
- Azure Logic Apps

---

# Azure Functions

**Azure Functions** is a serverless compute service that runs code in response to events.

Common triggers include:

- HTTP requests
- Timers
- Queues
- Storage changes

Azure handles much of the underlying infrastructure and scaling.

### Real-World Thinking

A small piece of code needs to run whenever a file is uploaded to storage.

Instead of maintaining a full server, an Azure Function can run when that event occurs.

### Exam Thinking

> **Azure Functions = serverless event-driven code.**

Think **run code**.

---

# Azure Logic Apps

**Azure Logic Apps** is a cloud service for building automated workflows and integrating applications, services, and data.

It provides a visual workflow designer and connectors for many services.

### Real-World Thinking

A company wants to automatically send an approval request when a business event occurs and then update another system after approval.

Logic Apps can coordinate that workflow with little or no custom code.

### Exam Thinking

> **Azure Logic Apps = automate workflows and connect services.**

Think **workflow**.

---

# Azure Functions vs. Logic Apps

| Service | Primary Purpose |
|---|---|
| **Azure Functions** | Run event-driven code |
| **Logic Apps** | Automate workflows and integrations |

### Easy Way to Remember

```text
Functions  = CODE
Logic Apps = WORKFLOW
```

---

# Azure DevOps

**Azure DevOps** is a collection of development and project-management services that help teams plan, build, test, and deploy applications.

## Core Services

### Azure Boards

Provides work tracking, Kanban boards, backlogs, and planning tools.

### Azure Repos

Provides Git repositories for source-code management.

### Azure Pipelines

Provides CI/CD automation for building, testing, and deploying applications.

### Azure Test Plans

Provides tools for software testing.

### Azure Artifacts

Provides package feeds for sharing development packages and dependencies.

### Real-World Thinking

A software team needs Git repositories, work tracking, and an automated process that builds and deploys code whenever changes are approved.

Azure DevOps provides tools for that development lifecycle.

### Exam Thinking

> **Azure DevOps = plan, build, test, and deploy software.**

### Memory Trick

```text
Boards    = PLAN
Repos     = CODE
Pipelines = BUILD / DEPLOY
Test Plans= TEST
Artifacts = PACKAGES
```

---

# Azure Monitor

**Azure Monitor** is Azure's observability and monitoring service.

It collects, analyzes, and acts on telemetry from Azure and supported hybrid environments.

## Key Capabilities

### Metrics

Numerical measurements collected over time, such as CPU usage or request counts.

### Logs

Detailed records and events that can be queried and analyzed.

### Visualization

Monitoring data can be presented using dashboards, workbooks, and supported visualization tools.

### Alerts

Azure Monitor can trigger alerts or actions when configured conditions are met.

### Real-World Thinking

An administrator needs to know whether a VM is experiencing unusually high CPU usage.

Azure Monitor can collect the metric and support alerts based on configured thresholds.

### Exam Thinking

> **Azure Monitor = collect and analyze metrics, logs, and telemetry.**

Think **what is happening with my resources?**

---

# Azure Advisor

**Azure Advisor** analyzes Azure resource configurations and usage and provides personalized recommendations.

Recommendations can cover areas such as:

- Cost
- Security
- Reliability
- Performance
- Operational excellence

### Real-World Thinking

An administrator wants Azure to identify opportunities to reduce costs or improve the configuration of existing resources.

Azure Advisor can provide recommendations.

### Exam Thinking

> **Azure Advisor = personalized best-practice recommendations.**

Think **what should I improve?**

---

# Azure Monitor vs. Azure Advisor

| Tool | Question It Answers |
|---|---|
| **Azure Monitor** | What is happening? |
| **Azure Advisor** | What should I improve? |

### Easy Way to Remember

```text
Monitor = OBSERVE
Advisor = RECOMMEND
```

---

# Azure Service Health

**Azure Service Health** provides information about Azure service issues, planned maintenance, and advisories that may affect your Azure environment.

## Related Health Views

### Azure Status

Provides a broad public view of Azure service status across regions and services.

### Service Health

Provides a personalized view of service issues, planned maintenance, and advisories relevant to your subscriptions.

### Resource Health

Provides health information for individual Azure resources.

### Real-World Thinking

An Azure application suddenly has problems and the administrator wants to know whether Microsoft is experiencing an Azure service outage affecting the subscription.

Azure Service Health is designed for this situation.

### Exam Thinking

> **Azure Service Health = Azure outages, maintenance, and service advisories.**

---

# Monitor vs. Service Health vs. Resource Health

| Tool | Primary Focus |
|---|---|
| **Azure Monitor** | Performance and telemetry |
| **Service Health** | Azure service issues affecting your environment |
| **Resource Health** | Health of an individual Azure resource |

---

# ARM Templates

**Azure Resource Manager (ARM) Templates** are JSON files that define Azure resources and configurations as code.

This approach is called **Infrastructure as Code (IaC)**.

## Benefits

- Repeatable deployments
- Consistent configurations
- Automation
- Version-controlled infrastructure definitions
- Reduced manual configuration

### Real-World Thinking

An organization needs to deploy the same Azure environment repeatedly for development, testing, and production.

Instead of manually creating every resource each time, an ARM Template can define the infrastructure.

### Exam Thinking

> **ARM Template = deploy Azure infrastructure using JSON Infrastructure as Code.**

Think **repeatable infrastructure deployment**.

---

# How the Tools Fit Together

One way to remember the services is to think about the lifecycle of an application:

```text
Azure DevOps
PLAN / BUILD / DEPLOY APPLICATIONS
        |
        v
ARM Templates
DEPLOY INFRASTRUCTURE
        |
        v
Azure Functions
RUN EVENT-DRIVEN CODE
        |
        v
Logic Apps
AUTOMATE WORKFLOWS
        |
        v
Azure Monitor
OBSERVE PERFORMANCE
        |
        v
Azure Advisor
RECOMMEND IMPROVEMENTS
        |
        v
Azure Service Health
CHECK AZURE SERVICE ISSUES
```

> [!NOTE]
> These tools do not have to be used together or in this exact order. The diagram is a memory aid for their primary purposes.

---

# Comparing the Core Management Tools

| Service | Primary Purpose |
|---|---|
| **Azure DevOps** | Software planning, source control, CI/CD, and development tools |
| **Azure Functions** | Serverless event-driven code |
| **Logic Apps** | Workflow automation and integration |
| **ARM Templates** | Infrastructure as Code deployment |
| **Azure Monitor** | Metrics, logs, telemetry, and alerts |
| **Azure Advisor** | Personalized optimization recommendations |
| **Azure Service Health** | Azure outages, maintenance, and advisories |

---

# Choosing the Right Tool

### Choose Azure DevOps when:
- You need source control.
- You need CI/CD pipelines.
- You need software project tracking.

### Choose Azure Functions when:
- Code should run in response to an event.
- You want serverless compute.

### Choose Logic Apps when:
- You need workflow automation.
- You need to connect multiple services with minimal custom code.

### Choose ARM Templates when:
- You need repeatable Azure infrastructure deployment.
- You want Infrastructure as Code.

### Choose Azure Monitor when:
- You need metrics or logs.
- You need alerts.
- You need to monitor application or resource performance.

### Choose Azure Advisor when:
- You want Azure recommendations.
- You want suggestions for cost, reliability, security, or performance improvements.

### Choose Azure Service Health when:
- You need to know whether Azure has a service issue.
- You need information about planned maintenance or advisories.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 12 Lab — Management Tools](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-12-Lab-12-Management-Tools.md)**

### Lab Focus

- Explore Azure Monitor.
- Review Metrics and Logs.
- Review the Azure Activity Log.
- Explore Azure Advisor recommendations.
- Explore Azure Service Health.
- View an ARM Template from an Azure resource when available.
- Practice identifying the correct management tool for common scenarios.

> [!TIP]
> Azure Portal exploration and practical management activities are kept in the separate lab.

---

# Quick Check

| Need | Azure Tool |
|---|---|
| Source control and CI/CD | Azure DevOps |
| Run event-driven code | Azure Functions |
| Automate a workflow | Logic Apps |
| Deploy infrastructure as code | ARM Templates |
| View metrics and logs | Azure Monitor |
| Receive optimization recommendations | Azure Advisor |
| Check Azure outages and maintenance | Azure Service Health |

---

# Before Moving On

You should be able to:

- Explain serverless computing.
- Compare Azure Functions and Logic Apps.
- Explain the purpose of Azure DevOps.
- Explain Azure Monitor.
- Explain Azure Advisor.
- Explain ARM Templates and Infrastructure as Code.
- Explain Azure Service Health.
- Know when each management tool should be used.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Azure DevOps** | Plan, build, test, deploy |
| **Azure Functions** | Event-driven serverless code |
| **Logic Apps** | Workflow automation |
| **ARM Templates** | Infrastructure as Code |
| **Azure Monitor** | Metrics, logs, telemetry |
| **Azure Advisor** | Recommendations |
| **Azure Service Health** | Azure service issues and maintenance |
