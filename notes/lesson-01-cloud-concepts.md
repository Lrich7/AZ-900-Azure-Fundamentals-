# Lesson 1 — Cloud Concepts I

## 📖 Learning Objectives

By the end of this lesson you should be able to:

- Explain what cloud computing is.
- Explain the differences between CapEx and OpEx.
- Describe the Consumption-Based Pricing model.
- Explain the Shared Responsibility Model.

---

## 🎥 Recommended Videos (John Savill)

| Topic | Length | Link |
|-------|:------:|------|
| CapEx, OpEx & Consumption-Based Pricing | 7:13 | https://youtu.be/WiwV9wb0GMo |
| High Availability & Scalability | 15:24 | https://youtu.be/JRbhGzGzoOA |

---

## ☁️ What is Cloud Computing?

Cloud computing is the **on-demand delivery of computing services**—including servers, storage, databases, networking, software, analytics, and AI—over the internet.

Instead of purchasing and maintaining physical hardware, organizations can access these resources whenever they need them while only paying for what they use.

Cloud computing provides:

- Scalability
- Flexibility
- High Availability
- Reduced infrastructure management

### AZ-900 Key Points

- ✅ On-demand resources
- ✅ Pay only for what you use
- ✅ Accessible from anywhere
- ✅ Scale resources quickly
- ✅ Microsoft manages much of the infrastructure

---

## 🌎 Cloud Services

![Azure Services](../images/azure-services-diagram.png)

| Azure Service | Purpose |
|---------------|---------|
| Virtual Machines | Run Windows or Linux servers |
| Storage | Store files, backups, and application data |
| Databases | Managed relational and NoSQL databases |
| Networking | Connect Azure resources securely |
| Internet of Things (IoT) | Connect and manage smart devices |
| Machine Learning | Build and train ML models |
| AI | Add intelligent features to applications |

### Real-World Example

Instead of purchasing a physical server to host your company's website, you can deploy an Azure Virtual Machine.

As traffic increases, you can increase CPU, memory, or storage within minutes instead of purchasing additional hardware.

---

# 💰 CapEx vs OpEx

## CapEx (Capital Expenditure)

Money spent on long-term assets such as:

- Buildings
- Servers
- Networking equipment
- Storage hardware

These assets are depreciated over several years.

### Examples

- Purchasing servers
- Buying networking equipment
- Building a datacenter

---

## OpEx (Operational Expenditure)

Ongoing day-to-day operating expenses.

Examples include:

- Software subscriptions
- Cloud services
- Utilities
- Rent
- Employee salaries

These expenses occur as they are used.

### Examples

- Microsoft Azure
- Microsoft 365
- Internet service
- Monthly cloud subscriptions

---

## 💳 Consumption-Based Pricing

Azure uses a **pay-as-you-go** pricing model.

Instead of paying for hardware upfront, you only pay for the cloud resources you consume.

### Example

If you run an Azure Virtual Machine for **10 hours**, you pay for **10 hours** of compute.

If you stop and deallocate the VM, compute charges stop (although storage charges may still apply).

---

## 🔐 Shared Responsibility Model

![Shared Responsibility Model](../images/shared-responsibility-model.png)

> 💡 **Memory Trick**
>
> **The closer something is to your data, the more responsibility you have.**

---

### You Are Responsible For

- Protecting your data
- Managing user access
- Passwords and MFA
- Guest operating system updates
- Application configuration
- Firewall rules

---

### Microsoft Is Responsible For

- Physical datacenters
- Physical servers
- Storage hardware
- Networking infrastructure
- Power
- Cooling
- Physical security

---

## 📌 Exam Tips

### CapEx

Think:

> "Buying"

Physical hardware that you own.

---

### OpEx

Think:

> "Renting"

Monthly or usage-based expenses.

---

### Consumption Pricing

Remember:

> **Only pay for what you use.**

---

### Shared Responsibility

Microsoft secures:

- The cloud

You secure:

- Your data
- Your users
- Your applications

---

## 🧪 Hands-on Lab

Practice navigating Azure before creating resources.

➡️ **Lesson 01 Lab – Explore the Azure Portal**

---

## ✅ Before Moving On

You should now be able to:

- [ ] Define cloud computing.
- [ ] Explain CapEx vs OpEx.
- [ ] Explain Consumption-Based Pricing.
- [ ] Explain the Shared Responsibility Model.
