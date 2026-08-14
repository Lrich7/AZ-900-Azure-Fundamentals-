
# Lab 03 — Cloud Service Models

## Objective

This lab reinforces **Lesson 3 — Cloud Service Models**.

By the end, you should be able to identify IaaS, PaaS, SaaS, and Serverless/FaaS and recognize common Azure examples.

---

## Prerequisites

- Completed **Lesson 3 — Cloud Service Models**
- Web browser
- Azure account for portal exploration

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Microsoft Learn — Describe Cloud Service Types:** https://learn.microsoft.com/en-us/training/modules/describe-cloud-service-types/

> [!NOTE]
> You do **not** need to deploy paid resources. The lab can be completed by reviewing the creation screens and documentation.

---

# Part 1 — Azure Virtual Machines (IaaS)

### Links
- **Azure Portal:** https://portal.azure.com/
- **Virtual Machines Documentation:** https://learn.microsoft.com/en-us/azure/virtual-machines/

## Steps
1. Open the Azure Portal.
2. Search for **Virtual machines**.
3. Open **Virtual machines**.
4. Select **Create** to review the available options. Do not complete the deployment.
5. Look for:
   - Operating system image
   - VM size
   - Disks
   - Networking
   - Administrator account

## Think About It
Why is Azure Virtual Machines considered IaaS?

**Answer:** _______________________________________________

Who manages the guest operating system?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure Virtual Machines = IaaS**

---

# Part 2 — Azure App Service (PaaS)

### Links
- **Azure Portal:** https://portal.azure.com/
- **App Service Overview:** https://learn.microsoft.com/en-us/azure/app-service/overview

## Steps
1. Open the Azure Portal.
2. Search for **App Services**.
3. Open **App Services**.
4. Select **Create** to review the available options.
5. Do not complete the deployment.
6. Compare what you see with the VM creation process.

## Think About It
Why is Azure App Service considered PaaS?

**Answer:** _______________________________________________

What server-management work does Azure remove compared with using a VM?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure App Service = PaaS**

---

# Part 3 — Azure Functions (Serverless / FaaS)

### Links
- **Azure Portal:** https://portal.azure.com/
- **Azure Functions Overview:** https://learn.microsoft.com/en-us/azure/azure-functions/functions-overview

## Steps
1. Open the Azure Portal.
2. Search for **Function App**.
3. Open **Function App**.
4. Review the available creation options.
5. Do not create a resource unless you intentionally want to experiment.

## Think About It
What is the main idea behind serverless computing?

**Answer:** _______________________________________________

Why might a developer use a Function instead of maintaining a VM for a small event-driven task?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure Functions = Serverless / FaaS**

**Serverless does not mean servers do not exist. It means you do not manage the underlying servers.**

---

# Part 4 — Azure SQL Database (PaaS)

### Links
- **Azure Portal:** https://portal.azure.com/
- **Azure SQL Database Overview:** https://learn.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview

## Steps
1. Open the Azure Portal.
2. Search for **SQL databases**.
3. Open **SQL databases**.
4. Select **Create** to review the configuration options.
5. Do not complete the deployment.

Compare:

```text
SQL Server installed inside an Azure VM
                vs.
        Azure SQL Database
```

## Think About It
Why is Azure SQL Database considered PaaS?

**Answer:** _______________________________________________

Which gives you more operating-system control: SQL Server in an Azure VM or Azure SQL Database?

**Answer:** _______________________________________________

### Exam Thinking
> **Azure SQL Database = PaaS**

---

# Part 5 — Identify the Service Model

Choose **IaaS, PaaS, SaaS, or Serverless/FaaS**.

1. An administrator needs a Windows Server VM and control over its operating system.  
   **Answer:** ______________________

2. Developers want to deploy a web app without maintaining the underlying OS.  
   **Answer:** ______________________

3. Employees use Microsoft 365 for email, Teams, Word, and Excel.  
   **Answer:** ______________________

4. Code should execute automatically when an event occurs without maintaining a server.  
   **Answer:** ______________________

5. A company wants a managed SQL database without maintaining the database server OS.  
   **Answer:** ______________________

---

# Part 6 — Exam Thinking

Complete these without looking back:

1. **IaaS** = ___________________________________________
2. **PaaS** = ___________________________________________
3. **SaaS** = ___________________________________________
4. **Azure Virtual Machines** = __________________________
5. **Azure App Service** = _______________________________
6. **Azure SQL Database** = ______________________________
7. **Azure Functions** = _________________________________
8. **Microsoft 365** = ___________________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Service Exploration
- **Azure Virtual Machines:** IaaS. The customer retains significant management responsibility, including the guest OS.
- **Azure App Service:** PaaS. Azure manages the underlying infrastructure/platform while you focus on the application.
- **Azure Functions:** Serverless/FaaS. You run code without managing the underlying servers.
- **Azure SQL Database:** PaaS. Azure manages more of the underlying database platform.

## Part 5
| Scenario | Answer |
|---|---|
| 1 | IaaS |
| 2 | PaaS |
| 3 | SaaS |
| 4 | Serverless / FaaS |
| 5 | PaaS |

## Part 6
- **IaaS:** Infrastructure as a Service
- **PaaS:** Platform as a Service
- **SaaS:** Software as a Service
- **Azure Virtual Machines:** IaaS
- **Azure App Service:** PaaS
- **Azure SQL Database:** PaaS
- **Azure Functions:** Serverless / FaaS
- **Microsoft 365:** SaaS

</details>

---

# Lab Complete

Before moving on, make sure you can explain:
- The difference between IaaS, PaaS, and SaaS.
- Why Azure Virtual Machines are IaaS.
- Why Azure App Service and Azure SQL Database are PaaS.
- Why Azure Functions is serverless/FaaS.
- Why Microsoft 365 is SaaS.
- How customer management responsibility decreases from IaaS → PaaS → SaaS.
