# Lab 10 — Storage

## Objective

This lab reinforces **Lesson 10 — Storage**.

By the end, you should be able to:

- Explore or create an Azure Storage Account.
- Explore Blob Storage.
- Explore Azure Files.
- Explore Queue Storage.
- Explore Table Storage.
- Compare Azure SQL Database and Azure Cosmos DB.
- Identify Azure Storage redundancy options.
- Explore Azure Database Migration Service.
- Choose the correct storage or database service for common scenarios.

---

## Prerequisites

- Completed **Lesson 10 — Storage**
- Web browser
- Azure account if completing resource-creation activities

### Start Here

- **Azure Portal:** https://portal.azure.com/
- **Azure Storage Fundamentals:** https://learn.microsoft.com/en-us/training/modules/azure-storage-fundamentals/
- **Create a Storage Account:** https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create

> [!IMPORTANT]
> You can complete much of this lab by reviewing Azure Portal configuration screens and Microsoft documentation. You do not need to deploy every service.

---

# Part 1 — Explore a Storage Account

### Links

- **Azure Portal:** https://portal.azure.com/
- **Create a Storage Account:** https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create
- **Storage Account Overview:** https://learn.microsoft.com/en-us/azure/storage/common/storage-account-overview

## Steps

1. Open Microsoft's **Create a Storage Account** guide.
2. Open the Azure Portal.
3. Search for **Storage accounts**.
4. Select **Create**.
5. Review the available configuration options.
6. Pay attention to:
   - Subscription
   - Resource Group
   - Storage account name
   - Region
   - Performance
   - Redundancy
7. If you have an appropriate lab subscription, you may create a test Storage Account.
8. Otherwise, stop before deployment.

## Think About It

What is the purpose of a Storage Account?

**Answer:** _______________________________________________

Which setting determines how Azure maintains additional copies of the data?

**Answer:** _______________________________________________

### Exam Thinking

> **Storage Account = top-level resource for Azure Storage services.**

---

# Part 2 — Explore Blob Storage

### Links

- **Blob Storage Introduction:** https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction
- **Azure Portal:** https://portal.azure.com/

## Steps

If you created or have access to a safe test Storage Account:

1. Open the Storage Account.
2. Locate **Containers** under the data storage options.
3. Review how containers organize blobs.
4. If appropriate, create a test container.
5. Do not upload sensitive or company data.

If you do not have a Storage Account, review the Blob Storage documentation instead.

## Think About It

What type of data is Blob Storage designed for?

**Answer:** _______________________________________________

What is the hierarchy from Storage Account to an individual Blob?

**Answer:** _______________________________________________

### Exam Thinking

```text
Storage Account -> Container -> Blob
```

---

# Part 3 — Explore Azure Files

### Links

- **Azure Files Introduction:** https://learn.microsoft.com/en-us/azure/storage/files/storage-files-introduction
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open a safe test Storage Account if available.
2. Locate **File shares**.
3. Review the available file-share options.
4. Review the Azure Files documentation.
5. Identify the file-sharing protocols mentioned.

## Think About It

Which common protocols can Azure Files support?

**Answer:** _______________________________________________

What traditional on-premises resource is Azure Files similar to?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Files = managed cloud file shares.**

---

# Part 4 — Explore Queue Storage

### Links

- **Azure Queue Storage Introduction:** https://learn.microsoft.com/en-us/azure/storage/queues/storage-queues-introduction
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open a safe test Storage Account if available.
2. Locate **Queues**.
3. Review how queues are organized.
4. Review Microsoft's Queue Storage documentation.
5. Think about how an application could place work into a queue for another component to process later.

## Think About It

Why are queues useful for asynchronous processing?

**Answer:** _______________________________________________

What does Queue Storage primarily hold?

**Answer:** _______________________________________________

### Exam Thinking

> **Queue Storage = application messages.**

---

# Part 5 — Explore Table Storage

### Links

- **Azure Table Storage Overview:** https://learn.microsoft.com/en-us/azure/storage/tables/table-storage-overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open a safe test Storage Account if available.
2. Locate **Tables**.
3. Review the Table Storage interface.
4. Review Microsoft's Table Storage documentation.
5. Identify:
   - Entity
   - Partition Key
   - Row Key

## Think About It

Is Table Storage relational or NoSQL?

**Answer:** _______________________________________________

What identifies an entity within a partition?

**Answer:** _______________________________________________

### Exam Thinking

> **Table Storage = structured non-relational / NoSQL data.**

---

# Part 6 — Azure SQL Database vs. Azure Cosmos DB

### Links

- **Azure SQL Database:** https://learn.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview
- **Azure Cosmos DB:** https://learn.microsoft.com/en-us/azure/cosmos-db/introduction
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Search the Azure Portal for **SQL databases**.
2. Review the service without creating a database.
3. Search for **Azure Cosmos DB**.
4. Review the service without creating an account.
5. Review the linked Microsoft documentation.
6. Complete the comparison below.

| Question | Azure SQL Database | Azure Cosmos DB |
|---|---|---|
| Relational or NoSQL? | __________ | __________ |
| Based on SQL Server? | __________ | __________ |
| Designed strongly around global distribution? | __________ | __________ |

## Think About It

Which service would you choose for a traditional relational application database?

**Answer:** _______________________________________________

Which service is designed for globally distributed NoSQL workloads?

**Answer:** _______________________________________________

---

# Part 7 — Explore Storage Redundancy

### Links

- **Azure Storage Redundancy:** https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy
- **Azure Portal:** https://portal.azure.com/

Review Microsoft's redundancy documentation and complete the table.

| Option | Where Copies Are Protected |
|---|---|
| **LRS** | __________________________________ |
| **ZRS** | __________________________________ |
| **GRS** | __________________________________ |
| **GZRS** | __________________________________ |

## Scenario Questions

### Scenario 1

You want redundancy within a local physical location in the primary region.

**Answer:** ______________________________

### Scenario 2

You want protection across Availability Zones in the same region.

**Answer:** ______________________________

### Scenario 3

You want data replicated to a secondary region.

**Answer:** ______________________________

### Scenario 4

You want Availability Zone redundancy in the primary region plus replication to another region.

**Answer:** ______________________________

### Exam Thinking

```text
LRS  = Local
ZRS  = Zones
GRS  = Geographic region
GZRS = Zones + Geographic region
```

---

# Part 8 — Explore Azure Database Migration Service

### Links

- **Azure Database Migration Service Overview:** https://learn.microsoft.com/en-us/azure/dms/dms-overview
- **Azure Portal:** https://portal.azure.com/

## Steps

1. Open the Azure Portal.
2. Search for **Azure Database Migration Service**.
3. Review the service without creating a migration project.
4. Review Microsoft's DMS overview.
5. Identify the general purpose of the service.

## Think About It

What is Azure Database Migration Service designed to help move?

**Answer:** _______________________________________________

Where are those database workloads generally being moved?

**Answer:** _______________________________________________

### Exam Thinking

> **Azure Database Migration Service = helps migrate databases to Azure.**

---

# Part 9 — Storage Scenarios

Choose from:

- **Blob Storage**
- **Azure Files**
- **Queue Storage**
- **Table Storage**
- **Azure SQL Database**
- **Azure Cosmos DB**
- **Azure Database Migration Service**

### Scenario 1

A company needs cloud storage for images, video files, and backups.

**Answer:** ______________________________

### Scenario 2

Employees need a managed shared file location using familiar file-sharing protocols.

**Answer:** ______________________________

### Scenario 3

An application needs to place messages into a backlog for background processing.

**Answer:** ______________________________

### Scenario 4

An application needs inexpensive structured NoSQL key/attribute storage.

**Answer:** ______________________________

### Scenario 5

An application requires a managed relational SQL database.

**Answer:** ______________________________

### Scenario 6

A worldwide application requires a globally distributed NoSQL database.

**Answer:** ______________________________

### Scenario 7

A company wants help moving an existing database workload into Azure.

**Answer:** ______________________________

---

# Answer Key

<details>
<summary><strong>Click to reveal answers</strong></summary>

## Part 1

A Storage Account provides the top-level Azure resource for Azure Storage services. The redundancy setting controls how additional copies of data are maintained.

## Part 2

Blob Storage is designed for unstructured object data.

```text
Storage Account -> Container -> Blob
```

## Part 3

Azure Files supports managed cloud file shares and can support protocols such as SMB and NFS.

## Part 4

Queue Storage primarily stores messages and can separate application components so work can be processed asynchronously.

## Part 5

Table Storage is NoSQL. The Row Key uniquely identifies an entity within its partition.

## Part 6

| Question | Azure SQL Database | Azure Cosmos DB |
|---|---|---|
| Relational or NoSQL? | Relational | NoSQL |
| Based on SQL Server? | Yes | No |
| Designed strongly around global distribution? | No | Yes |

## Part 7

| Option | Protection |
|---|---|
| **LRS** | Local physical location |
| **ZRS** | Availability Zones in the primary region |
| **GRS** | Primary region plus secondary region |
| **GZRS** | Availability Zones plus secondary region |

Scenarios: **1 LRS, 2 ZRS, 3 GRS, 4 GZRS**

## Part 8

Azure Database Migration Service helps move supported database workloads into Azure.

## Part 9

| Scenario | Answer |
|---|---|
| 1 | Blob Storage |
| 2 | Azure Files |
| 3 | Queue Storage |
| 4 | Table Storage |
| 5 | Azure SQL Database |
| 6 | Azure Cosmos DB |
| 7 | Azure Database Migration Service |

</details>

---

# Lab Cleanup

If you created a Storage Account or other test resources, remove them when finished unless you intentionally want to keep them.

### Links

- **Manage Resource Groups:** https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal
- **Azure Portal:** https://portal.azure.com/

> [!CAUTION]
> Verify that a Resource Group contains only lab resources before deleting it. Deleting the Resource Group deletes all resources inside it.

---

# Lab Complete

Before moving on, make sure you can explain:

- Blob vs. Files vs. Queue vs. Table Storage.
- Azure SQL Database vs. Azure Cosmos DB.
- LRS vs. ZRS vs. GRS vs. GZRS.
- The purpose of Azure Database Migration Service.
- Which Azure storage or database service best fits a basic AZ-900 scenario.
