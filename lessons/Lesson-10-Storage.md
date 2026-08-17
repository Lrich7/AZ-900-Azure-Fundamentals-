[Lesson-10-Storage.md](https://github.com/user-attachments/files/31148756/Lesson-10-Storage.md)

# Lesson 10 — Storage

## 📖 Microsoft Learn

**Module:** Azure Storage Fundamentals  
https://learn.microsoft.com/en-us/training/modules/azure-storage-fundamentals/

### Focus
- Storage Accounts
- Blob Storage
- Azure Files
- Queue Storage
- Table Storage
- Azure SQL Database
- Azure Cosmos DB
- Storage Redundancy
- Azure Data Migration Service

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Storage Account Resources | 18:04 | https://youtu.be/b8BrfsxLSx8 |
| Benefits and Usage of Database Resources | 13:29 | https://youtu.be/4sQOF9fSOAU |
| Data Movement and Migration Options | 11:47 | https://youtu.be/jNBcXnMTo9s |

---

# Azure Storage

Azure provides several storage services for different types of data.

A **Storage Account** is the top-level Azure resource that provides access to services such as:

- Blob Storage
- Azure Files
- Queue Storage
- Table Storage

The Storage Account also defines settings such as performance, redundancy, and access controls.

### Real-World Thinking

A company may need to store documents, application messages, backups, and structured data. Different Azure Storage services are designed for different data types and access patterns.

### Exam Thinking

> **Storage Account = top-level Azure resource for Azure Storage services.**

---

# Blob Storage

**Azure Blob Storage** is Microsoft's cloud object storage service for large amounts of unstructured data.

Examples include:

- Text files
- Images
- Video
- Audio
- Backups
- Binary files

## Storage Structure

```text
Storage Account
      |
      v
   Container
      |
      v
     Blob
```

### Storage Account
The top-level Azure resource.

### Container
Groups blobs together inside the Storage Account.

### Blob
The individual object or file stored in a container.

---

# Types of Blobs

## Block Blobs

Designed for storing text and binary data.

Common examples include documents, images, videos, and backups.

## Append Blobs

Optimized for data that is continually appended.

A common example is logging.

## Page Blobs

Designed for random-access files.

Page blobs are commonly associated with virtual hard disks.

### Exam Thinking

```text
Block Blob  = Files and objects
Append Blob = Append-heavy data such as logs
Page Blob   = Random-access data / virtual disks
```

---

# Azure Files

**Azure Files** provides fully managed cloud file shares.

It supports standard file-sharing protocols such as:

- SMB
- NFS

File shares can be accessed from supported Windows, Linux, and macOS environments.

## Key Features

### Fully Managed

Microsoft manages the underlying storage infrastructure.

### Hybrid Access

Azure File Sync can help organizations use Azure Files with on-premises Windows file servers.

### Performance Options

Azure Files provides options for general-purpose and higher-performance workloads.

### Real-World Thinking

A company wants to move a traditional shared network drive to Azure while continuing to use familiar file-sharing protocols.

Azure Files is designed for this type of scenario.

### Exam Thinking

> **Azure Files = managed cloud file shares.**

Think **shared folders / file shares**.

---

# Queue Storage

**Azure Queue Storage** stores messages that can be used by different components of an application to communicate.

Queues help applications process work asynchronously.

```text
Application
    |
    v
  Queue
    |
    v
Background Worker
```

## Common Uses

- Backlogs of work
- Background processing
- Communication between application components
- Separating parts of an application so they can operate independently

### Real-World Thinking

A web application receives an order and places a message in a queue. A separate background process can handle the order without forcing the user to wait for all processing to finish.

### Exam Thinking

> **Queue Storage = messages between application components.**

---

# Table Storage

**Azure Table Storage** is a managed NoSQL data store for structured, non-relational data.

It uses a schemaless key/attribute design.

## Core Concepts

### Entity

An individual record stored in a table.

### Partition Key

Groups related entities and helps distribute data.

### Row Key

Uniquely identifies an entity within its partition.

### Schemaless Design

Entities in the same table do not have to contain identical properties.

### Real-World Thinking

Table Storage can be useful for large amounts of structured data that does not require a traditional relational database model.

### Exam Thinking

> **Table Storage = NoSQL key/attribute data.**

---

# Comparing Azure Storage Services

| Storage Service | Best For |
|---|---|
| **Blob Storage** | Files, images, video, backups, unstructured objects |
| **Azure Files** | Shared file shares |
| **Queue Storage** | Application messages |
| **Table Storage** | Structured non-relational / NoSQL data |

### Easy Way to Remember

```text
Blob  = OBJECTS / FILES
Files = SHARED FOLDERS
Queue = MESSAGES
Table = NoSQL DATA
```

---

# Azure SQL Database

**Azure SQL Database** is a fully managed relational database service based on Microsoft SQL Server.

Azure manages many infrastructure tasks such as:

- Updates
- Backups
- High availability
- Platform maintenance

### Real-World Thinking

An application requires relational tables and SQL queries, but the organization does not want to maintain the underlying database server.

Azure SQL Database is designed for this scenario.

### Exam Thinking

> **Azure SQL Database = managed relational SQL database.**

---

# Azure Cosmos DB

**Azure Cosmos DB** is a fully managed NoSQL database service designed for highly scalable and globally distributed applications.

It is designed to support capabilities such as:

- Global distribution
- Low-latency access
- High availability
- Automatic scaling options

### Real-World Thinking

An application has users in multiple parts of the world and needs fast access to NoSQL data across regions.

Azure Cosmos DB may be appropriate.

### Exam Thinking

> **Azure Cosmos DB = globally distributed NoSQL database.**

---

# Azure SQL Database vs. Azure Cosmos DB

| Feature | Azure SQL Database | Azure Cosmos DB |
|---|---|---|
| Data model | Relational | NoSQL |
| SQL Server based | Yes | No |
| Managed Azure database | Yes | Yes |
| Global distribution focus | Not its primary exam identifier | Yes |

### Easy Way to Remember

```text
Azure SQL Database = RELATIONAL
Azure Cosmos DB    = GLOBAL NoSQL
```

---

# Azure Storage Redundancy

Azure Storage can maintain multiple copies of data to improve durability and resiliency.

The major redundancy options covered for AZ-900 are:

- LRS
- ZRS
- GRS
- GZRS

---

# Locally Redundant Storage (LRS)

**LRS** stores multiple copies of data within a single physical location in the primary region.

It protects against local hardware failures but does not protect against the loss of the entire location.

### Exam Thinking

> **LRS = local redundancy in one physical location.**

---

# Zone-Redundant Storage (ZRS)

**ZRS** replicates data across multiple Availability Zones within the primary Azure region.

This provides protection if one Availability Zone becomes unavailable.

### Exam Thinking

> **ZRS = redundancy across Availability Zones in one region.**

---

# Geo-Redundant Storage (GRS)

**GRS** maintains local redundancy in the primary region and asynchronously replicates data to a secondary geographic region.

This adds protection against a regional disaster.

### Exam Thinking

> **GRS = local redundancy + replication to another region.**

---

# Geo-Zone-Redundant Storage (GZRS)

**GZRS** combines zone redundancy in the primary region with replication to a secondary region.

### Exam Thinking

> **GZRS = Availability Zones + another region.**

---

# Comparing Storage Redundancy

| Replication | Primary Protection | Geographic Protection |
|---|---|---|
| **LRS** | Local hardware/location failures | No |
| **ZRS** | Availability Zone failure | No |
| **GRS** | Local redundancy | Secondary region |
| **GZRS** | Availability Zone failure | Secondary region |

### Memory Trick

```text
LRS  = Local
ZRS  = Zones
GRS  = Geographic region
GZRS = Zones + Geographic region
```

As the protection expands, the data is replicated across a wider failure boundary.

---

# Azure Data Migration Service

**Azure Database Migration Service (DMS)** helps migrate databases to Azure.

It can assist organizations moving database workloads from on-premises environments or other locations into supported Azure data platforms.

### Real-World Thinking

A company wants to move an existing database into Azure while simplifying the migration process and reducing downtime where supported.

### Exam Thinking

> **Azure Database Migration Service = helps migrate databases to Azure.**

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 10 Lab — Storage](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-10-Lab-10-Storage.md)**

### Lab Focus

- Create or explore an Azure Storage Account.
- Explore Blob Storage.
- Explore Azure Files.
- Explore Queue Storage.
- Explore Table Storage.
- Compare Azure SQL Database and Azure Cosmos DB.
- Review LRS, ZRS, GRS, and GZRS.
- Explore Azure Database Migration Service.
- Practice selecting the correct storage service for common scenarios.

> [!TIP]
> Azure Portal exploration, resource creation, and practical activities are kept in the separate lab.

---

# Quick Check

| Need | Azure Service / Concept |
|---|---|
| Store unstructured objects | Blob Storage |
| Managed shared file shares | Azure Files |
| Messages between application components | Queue Storage |
| Structured non-relational data | Table Storage |
| Managed relational database | Azure SQL Database |
| Globally distributed NoSQL database | Azure Cosmos DB |
| Local redundancy | LRS |
| Redundancy across Availability Zones | ZRS |
| Replication to another region | GRS |
| Zones plus another region | GZRS |
| Database migration into Azure | Azure Database Migration Service |

---

# Before Moving On

You should be able to:

- Explain the purpose of a Storage Account.
- Compare Blob, File, Queue, and Table Storage.
- Explain when Azure SQL Database is appropriate.
- Explain the purpose of Azure Cosmos DB.
- Compare Azure SQL Database and Azure Cosmos DB.
- Explain the purpose of Azure Database Migration Service.
- Explain the differences between LRS, ZRS, GRS, and GZRS.
- Choose the appropriate storage service from a basic scenario.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **Storage Account** | Top-level Azure Storage resource |
| **Blob Storage** | Object/unstructured storage |
| **Azure Files** | Managed file shares |
| **Queue Storage** | Application messages |
| **Table Storage** | NoSQL key/attribute data |
| **Azure SQL Database** | Managed relational database |
| **Azure Cosmos DB** | Globally distributed NoSQL |
| **LRS** | Local redundancy |
| **ZRS** | Availability Zone redundancy |
| **GRS** | Replication to another region |
| **GZRS** | Zones + another region |
| **Database Migration Service** | Migrate databases to Azure |
