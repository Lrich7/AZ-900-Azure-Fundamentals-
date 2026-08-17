# Lab 11 — Core Azure Solutions

## Objective

This lab reinforces **Lesson 11 — Core Azure Solutions**.

By the end, you should be able to:

- Explore Azure IoT Hub.
- Explore Azure Data Factory.
- Explore Azure Synapse Analytics.
- Explore Azure AI Services.
- Explore Azure Machine Learning.
- Describe a real-world use for each service.
- Choose the correct Azure service for common AZ-900 scenarios.

---

## Prerequisites

- Completed **Lesson 11 — Core Azure Solutions**
- Web browser
- Azure account for Azure Portal exploration

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Explore Azure AI Services:** https://learn.microsoft.com/en-us/training/modules/explore-azure-ai-services/

> [!IMPORTANT]
> This lab is primarily an exploration lab. You do **not** need to deploy IoT, analytics, or AI resources. Some of these services can create billable resources if deployed.

---

# Part 1 — Explore Azure IoT Hub

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure IoT Hub Overview:** https://learn.microsoft.com/en-us/azure/iot-hub/iot-concepts-and-iot-hub

## Steps

1. Open the Azure Portal.
2. Search for **IoT Hub**.
3. Open the IoT Hub service.
4. Review the service and available creation options.
5. Do not deploy an IoT Hub for this fundamentals lab.
6. Review the Microsoft IoT Hub overview.
7. Look for concepts involving:
   - Device-to-cloud communication
   - Cloud-to-device communication
   - Telemetry
   - Device management

## Think About It

What type of devices would connect to IoT Hub?

**Answer:** _______________________________________________

Can IoT Hub support communication in both directions?

**Answer:** _______________________________________________

What type of data might an IoT device send to Azure?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure IoT Hub = connect and manage IoT devices.**

---

# Part 2 — Explore Azure Data Factory

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Data Factory Introduction:** https://learn.microsoft.com/en-us/azure/data-factory/introduction

## Steps

1. Search the Azure Portal for **Data factories**.
2. Open the service.
3. Review the available creation options.
4. Do not create a Data Factory for this lab.
5. Review Microsoft's Data Factory introduction.
6. Look for the term **pipeline**.
7. Identify examples of data sources and destinations.

## Think About It

What is the primary purpose of Azure Data Factory?

**Answer:** _______________________________________________

What is a data pipeline?

**Answer:** _______________________________________________

Why might data need to be transformed before analytics?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Data Factory = move and transform data.**

---

# Part 3 — Explore Azure Synapse Analytics

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Synapse Analytics Overview:** https://learn.microsoft.com/en-us/azure/synapse-analytics/overview-what-is

## Steps

1. Search the Azure Portal for **Azure Synapse Analytics**.
2. Open the service.
3. Review the available workspace options.
4. Do not deploy a Synapse workspace.
5. Review Microsoft's Synapse overview.
6. Look for references to:
   - Data warehousing
   - Big-data analytics
   - Data integration
   - Business intelligence

## Think About It

What type of problem is Azure Synapse Analytics designed to solve?

**Answer:** _______________________________________________

Would Synapse be more closely associated with collecting IoT devices or analyzing large datasets?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Synapse Analytics = big-data analytics and data warehousing.**

---

# Part 4 — Explore Azure AI Services

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure AI Services Documentation:** https://learn.microsoft.com/en-us/azure/ai-services/
- **Explore Azure AI Services:** https://learn.microsoft.com/en-us/training/modules/explore-azure-ai-services/

## Steps

1. Open the Azure Portal.
2. Search for **Azure AI services**.
3. Review the available AI services without creating a resource.
4. Open the Microsoft documentation.
5. Identify examples involving:
   - Speech
   - Vision
   - Language
   - Translation
   - Document processing
   - Content Safety

## Think About It

What is the advantage of using a prebuilt AI service?

**Answer:** _______________________________________________

Which type of AI capability could convert spoken audio into text?

**Answer:** _______________________________________________

Which type of AI capability could analyze an image?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure AI Services = prebuilt AI capabilities.**

---

# Part 5 — Explore Azure Machine Learning

### Links

- **Azure Portal:** https://portal.azure.com/
- **Azure Machine Learning Overview:** https://learn.microsoft.com/en-us/azure/machine-learning/overview-what-is-azure-machine-learning

## Steps

1. Search the Azure Portal for **Machine Learning**.
2. Open Azure Machine Learning.
3. Review the workspace creation options.
4. Do not create a workspace for this fundamentals lab.
5. Review Microsoft's Azure Machine Learning overview.
6. Look for concepts involving:
   - Training
   - Models
   - Deployment
   - Machine-learning workflows

## Think About It

What is the main difference between Azure Machine Learning and Azure AI Services?

**Answer:** _______________________________________________

Which service would you choose if a data scientist needs to train a custom predictive model?

**Answer:** _______________________________________________

### Exam Thinking

```text
AI Services      = USE prebuilt AI
Machine Learning = BUILD / TRAIN models
```

---

# Part 6 — Follow the Data

Match each stage with the Azure service that best fits.

```text
Connected devices
       |
       v
[ __________________ ]
Collect device telemetry
       |
       v
[ __________________ ]
Move and transform data
       |
       v
[ __________________ ]
Analyze large datasets
       |
       v
[ __________________ ]
Build and train predictive models
```

Choose from:

- Azure IoT Hub
- Azure Data Factory
- Azure Synapse Analytics
- Azure Machine Learning

## Think About It

Which service in this flow is primarily responsible for moving data?

**Answer:** _______________________________________________

Which service is primarily responsible for analytics?

**Answer:** _______________________________________________

---

# Part 7 — Real-World Scenarios

Choose from:

- **Azure IoT Hub**
- **Azure Data Factory**
- **Azure Synapse Analytics**
- **Azure AI Services**
- **Azure Machine Learning**

### Scenario 1

A manufacturing company needs to securely connect thousands of sensors to Azure and collect telemetry.

**Answer:** ______________________________

### Scenario 2

A company needs to automatically move and transform information from several systems into an analytics platform.

**Answer:** ______________________________

### Scenario 3

An organization needs to analyze very large datasets for reporting and business intelligence.

**Answer:** ______________________________

### Scenario 4

A developer wants to add speech recognition to an application without building a speech model from scratch.

**Answer:** ______________________________

### Scenario 5

A data-science team wants to train a custom predictive model using historical company data.

**Answer:** ______________________________

### Scenario 6

A developer needs a prebuilt service that can analyze images.

**Answer:** ______________________________

### Scenario 7

A company wants a cloud service focused on data warehousing and large-scale analytics.

**Answer:** ______________________________

---

# Part 8 — Service Identification

Complete the table before checking the answer key.

| Description | Azure Service |
|---|---|
| Connect and manage IoT devices | __________________ |
| Move and transform data | __________________ |
| Big-data analytics and warehousing | __________________ |
| Prebuilt AI APIs and capabilities | __________________ |
| Build and train machine-learning models | __________________ |

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

IoT Hub connects and manages IoT devices and supports device-to-cloud and cloud-to-device communication. Devices may send telemetry such as temperature, location, equipment status, or sensor readings.

## Part 2

Azure Data Factory moves, transforms, and integrates data using data pipelines.

## Part 3

Azure Synapse Analytics is designed for large-scale analytics and data warehousing.

## Part 4

Prebuilt AI services allow developers to add AI capabilities without building every underlying model themselves.

Speech capabilities can convert spoken audio into text. Vision capabilities can analyze images.

## Part 5

Azure AI Services provides prebuilt capabilities, while Azure Machine Learning provides tools for building, training, deploying, and managing custom machine-learning models.

## Part 6

```text
Azure IoT Hub
      |
      v
Azure Data Factory
      |
      v
Azure Synapse Analytics
      |
      v
Azure Machine Learning
```

## Part 7

| Scenario | Answer |
|---|---|
| 1 | Azure IoT Hub |
| 2 | Azure Data Factory |
| 3 | Azure Synapse Analytics |
| 4 | Azure AI Services |
| 5 | Azure Machine Learning |
| 6 | Azure AI Services |
| 7 | Azure Synapse Analytics |

## Part 8

| Description | Azure Service |
|---|---|
| Connect and manage IoT devices | Azure IoT Hub |
| Move and transform data | Azure Data Factory |
| Big-data analytics and warehousing | Azure Synapse Analytics |
| Prebuilt AI APIs and capabilities | Azure AI Services |
| Build and train machine-learning models | Azure Machine Learning |

</details>

---

# Lab Complete

Before moving on, make sure you can explain:

- Azure IoT Hub.
- Azure Data Factory.
- Azure Synapse Analytics.
- Azure AI Services.
- Azure Machine Learning.
- Azure AI Services vs. Azure Machine Learning.
- Which service best fits a basic IoT, data, analytics, or AI scenario.
