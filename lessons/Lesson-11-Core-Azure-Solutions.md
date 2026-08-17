[Lesson-11-Core-Azure-Solutions.md](https://github.com/user-attachments/files/31148772/Lesson-11-Core-Azure-Solutions.md)

# Lesson 11 — Core Azure Solutions

## 📖 Microsoft Learn

**Module:** Explore Azure AI Services  
https://learn.microsoft.com/en-us/training/modules/explore-azure-ai-services/

### Focus
- Internet of Things (IoT)
- Big Data & Analytics
- Azure AI Services
- Azure Machine Learning

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Azure IoT Services | 21:08 | https://youtu.be/22z9ARaKlbU |
| Benefits and Usage of Big Data and Analytics Services | 13:26 | https://youtu.be/LSVewE4mKfE |
| Benefits and Usage of AI Services | 9:21 | https://youtu.be/lgcpRpV3HPc |

---

# Core Azure Solutions

Azure includes services for connecting devices, moving and analyzing large amounts of data, and adding artificial intelligence to applications.

For AZ-900, focus on understanding the **primary purpose** of each service and recognizing which service best fits a basic business scenario.

---

# Internet of Things (IoT)

The **Internet of Things (IoT)** refers to physical devices that connect to networks and exchange data.

Azure provides services for connecting, managing, and analyzing data from IoT devices.

Examples include:

- Sensors
- Manufacturing equipment
- Vehicles
- Smart-building devices
- Environmental monitors

---

# Azure IoT Hub

**Azure IoT Hub** is a managed cloud service that securely connects, monitors, and manages IoT devices.

It supports two-way communication between devices and Azure.

## Common Capabilities

- Collect telemetry from devices
- Send commands from the cloud to devices
- Monitor device connections
- Manage large numbers of connected devices

### Real-World Thinking

A manufacturing company has thousands of sensors reporting temperature and equipment status.

Azure IoT Hub can provide the cloud connection between those devices and Azure.

### Exam Thinking

> **Azure IoT Hub = connect and manage IoT devices.**

Think **device ↔ cloud communication**.

---

# Other Azure IoT Services

## Azure IoT Operations

Helps connect and manage industrial edge environments and process device data closer to where it is generated.

## Azure IoT Central

Provides a more application-focused approach for building and managing IoT solutions using preconfigured capabilities and templates.

## Azure Digital Twins

Allows organizations to create digital representations of physical environments, equipment, and systems.

## Device Provisioning

Helps automatically provision and register large numbers of IoT devices.

### Easy Way to Remember

```text
IoT Hub        = Device communication
IoT Operations = Industrial edge
IoT Central    = Simplified IoT applications
Digital Twins  = Virtual models of physical systems
```

---

# Big Data & Analytics

Azure provides services for storing, moving, processing, and analyzing very large datasets.

Common services include:

- Azure Data Factory
- Azure Synapse Analytics
- Azure Databricks
- Azure Data Lake Storage
- Azure Stream Analytics
- Azure Data Explorer

For AZ-900, the important distinction is the **primary job each service performs**.

---

# Azure Data Factory

**Azure Data Factory** is a cloud-based data integration service used to move, transform, and automate data between different sources.

It allows organizations to build **data pipelines**.

```text
Data Source
     |
     v
Azure Data Factory
     |
 Move / Transform
     |
     v
Destination
```

## Common Uses

- Moving data between systems
- Transforming data
- Automating data movement
- Building ETL/ELT pipelines
- Preparing data for analytics

### Real-World Thinking

A company has information stored in several systems and needs to move and prepare that data before analytics can be performed.

Azure Data Factory can automate that data pipeline.

### Exam Thinking

> **Azure Data Factory = move and transform data.**

Think **data pipeline**.

---

# Azure Synapse Analytics

**Azure Synapse Analytics** is a cloud analytics service that combines capabilities for data integration, data warehousing, and big-data analytics.

It helps organizations analyze large volumes of data for:

- Reporting
- Business intelligence
- Data warehousing
- Large-scale analytics

### Real-World Thinking

A company wants to combine large datasets and analyze them to identify business trends.

Azure Synapse Analytics is designed for large-scale analytics.

### Exam Thinking

> **Azure Synapse Analytics = big-data analytics and data warehousing.**

Think **analyze**.

---

# Other Big Data Services

## Azure Data Lake Storage

Designed for storing large amounts of raw and structured data for analytics workloads.

## Azure Databricks

Provides an Apache Spark-based analytics environment used for data engineering, analytics, and machine-learning workloads.

## Azure Stream Analytics

Processes real-time streams of data.

## Azure Data Explorer

Designed for fast analysis of large volumes of telemetry, logs, and other time-series or streaming data.

---

# Azure AI Services

**Azure AI Services** provides prebuilt artificial-intelligence capabilities that developers can add to applications without building every AI model from scratch.

Examples include:

- Speech
- Vision
- Language
- Translation
- Document processing
- Content Safety

## Speech

Can provide capabilities such as:

- Speech-to-text
- Text-to-speech
- Speech translation

## Vision

Can analyze images and extract useful information.

## Language and Translator

Can analyze natural language and translate text.

## Content Safety

Can help detect harmful or unwanted content in text and images.

### Real-World Thinking

A developer wants an application to recognize speech or analyze images but does not want to build and train the underlying AI model from scratch.

A prebuilt Azure AI service may be appropriate.

### Exam Thinking

> **Azure AI Services = prebuilt AI capabilities and APIs.**

Think **use AI that is already built**.

---

# Azure Machine Learning

**Azure Machine Learning** is a cloud platform for building, training, deploying, and managing machine-learning models.

It provides tools for:

- Preparing data
- Training models
- Deploying models
- Managing machine-learning workflows
- Monitoring ML solutions

### Real-World Thinking

A data-science team wants to create its own predictive model using historical business data.

Azure Machine Learning provides the tools to build and train that model.

### Exam Thinking

> **Azure Machine Learning = build, train, deploy, and manage ML models.**

Think **build your own model**.

---

# Azure AI Services vs. Azure Machine Learning

| Service | Best Fit |
|---|---|
| **Azure AI Services** | Add prebuilt AI capabilities to an application |
| **Azure Machine Learning** | Build and train custom machine-learning models |

### Easy Way to Remember

```text
Azure AI Services      = USE prebuilt AI
Azure Machine Learning = BUILD and TRAIN models
```

---

# How the Services Work Together

One way to think about the services is as a flow of data through an intelligent application:

```text
Azure IoT Hub
COLLECT device data
      |
      v
Azure Data Factory
MOVE / TRANSFORM data
      |
      v
Azure Synapse Analytics
ANALYZE data
      |
      v
Azure Machine Learning
BUILD / TRAIN models
      |
      v
Azure AI Services
ADD prebuilt AI capabilities
```

> [!NOTE]
> These services do not have to be used together or in this exact order. The diagram is a memory aid for their primary purposes.

### Memory Trick

```text
IoT Hub          = Collect
Data Factory     = Move
Synapse          = Analyze
Machine Learning = Train
AI Services      = Use prebuilt AI
```

---

# Comparing Core Azure Solutions

| Service | Primary Purpose |
|---|---|
| **Azure IoT Hub** | Connect and manage IoT devices |
| **Azure Data Factory** | Move and transform data |
| **Azure Synapse Analytics** | Big-data analytics and data warehousing |
| **Azure AI Services** | Prebuilt AI capabilities |
| **Azure Machine Learning** | Build and train ML models |

---

# Choosing the Right Service

### Choose Azure IoT Hub when:
- You need to connect IoT devices to Azure.
- You need two-way device-to-cloud communication.
- You need to collect telemetry from connected devices.

### Choose Azure Data Factory when:
- You need to move data between systems.
- You need automated data pipelines.
- You need to transform or prepare data.

### Choose Azure Synapse Analytics when:
- You need large-scale analytics.
- You need data warehousing.
- You need to analyze large datasets.

### Choose Azure AI Services when:
- You need ready-made AI capabilities.
- You need speech, vision, language, translation, or similar APIs.

### Choose Azure Machine Learning when:
- You need to build your own ML model.
- You need to train or deploy machine-learning models.

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 11 Lab — Core Azure Solutions](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-11-Lab-11-Core-Azure-Solutions.md)**

### Lab Focus

- Explore Azure IoT Hub.
- Explore Azure Data Factory.
- Explore Azure Synapse Analytics.
- Explore Azure AI Services.
- Explore Azure Machine Learning.
- Identify real-world uses for each service.
- Practice selecting the correct service for common AZ-900 scenarios.

> [!TIP]
> Azure Portal exploration and practical service-identification activities are kept in the separate lab.

---

# Quick Check

| Need | Azure Service |
|---|---|
| Connect and manage IoT devices | Azure IoT Hub |
| Move and transform data | Azure Data Factory |
| Analyze large datasets | Azure Synapse Analytics |
| Add prebuilt AI capabilities | Azure AI Services |
| Build and train ML models | Azure Machine Learning |

---

# Before Moving On

You should be able to:

- Explain the purpose of Azure IoT Hub.
- Explain the purpose of Azure Data Factory.
- Explain the purpose of Azure Synapse Analytics.
- Explain Azure AI Services.
- Explain Azure Machine Learning.
- Compare Azure AI Services and Azure Machine Learning.
- Identify which Azure service best fits a common business scenario.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **IoT Hub** | Connect and manage devices |
| **Data Factory** | Move and transform data |
| **Synapse Analytics** | Analyze large datasets |
| **AI Services** | Prebuilt AI |
| **Machine Learning** | Build and train ML models |
