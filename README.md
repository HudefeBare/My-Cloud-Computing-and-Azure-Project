# 📊 Azure Data Fundamentals (DP-900) – Cloud Data Services & Analytics Project

*A hands-on project covering cloud computing fundamentals, Azure data services, data ingestion, and analytical workloads using Microsoft Fabric.*

---

## 🛠 Core Technologies (Visual Overview)

[Azure SQL Database](https://azure.microsoft.com/en-us/products/azure-sql/database/) · [Azure Storage Account](https://azure.microsoft.com/en-us/products/storage/) · [Azure Cosmos DB](https://azure.microsoft.com/en-us/products/cosmos-db/) · [Microsoft Fabric](https://www.microsoft.com/en-us/microsoft-fabric) · Power BI

---

## 🔍 Overview

This repository contains my Week 5 Cloud Computing and Azure Data Fundamentals (DP-900) work, completed as part of the Data Technician training course.

The project covers cloud computing concepts, Azure cost estimation, relational and non-relational data, data ingestion, and analytics using Microsoft Fabric and Power BI. It also includes hands-on Azure labs and a scenario-based solution for a pet shop, "Paws & Whiskers".

---

## 🚀 Skills Demonstrated

### ✔️ Cloud Computing Fundamentals

- Understanding IaaS, PaaS, and SaaS with real-world examples
- Public, private, hybrid, and community cloud models
- Cloud benefits and risks, including scalability, flexibility, reliability, and unexpected costs
- Cloud versus on-premises infrastructure
- Comparing major providers: AWS, Microsoft Azure, and Google Cloud
- Estimating cloud costs using the Azure Pricing Calculator

### ✔️ Relational Data – Azure SQL Database

- Provisioned an Azure SQL Database and SQL server
- Created tables, loaded sample data, and queried it using SQL
- Worked with structured relational data
- Deleted resources after completing the lab to avoid ongoing costs

### ✔️ Non-Relational Data – Azure Storage Account & Azure Cosmos DB

- Explored Blob Storage, Data Lake Storage Gen2, and Azure Files
- Created an Azure Cosmos DB account and added JSON items
- Queried non-relational data using a SQL-like query language

### ✔️ Analytical Workloads – Microsoft Fabric & Power BI

- Explored Lakehouse and real-time analytics concepts in Microsoft Fabric
- Built a Power BI sales report using bar, pie, and map visuals
- Used visualisations to present sales information and support analysis

### ✔️ Data Ingestion

| **Method** | **Description** |
|---|---|
| ⚡ **Eventstreams** | Capture and route real-time streaming data into Fabric |
| 🔄 **Data pipelines** | Move and transform batch data from different sources |
| 📁 **File uploads** | Load CSV, JSON, and Parquet files into storage or a Lakehouse |
| 🗄️ **Direct connections** | Connect Power BI to data sources such as SQL Server and Excel |

### ✔️ SQL Skills

Practised core SQL concepts for querying, filtering, sorting, aggregating, and combining data.

| **SQL Clause** | **Purpose** |
|---|---|
| `SELECT` | Choose columns to return |
| `WHERE` | Filter rows using a condition |
| `ORDER BY` | Sort query results |
| `GROUP BY` | Calculate totals, counts, and averages |
| `JOIN` | Combine related tables |

The following illustrative examples demonstrate these SQL concepts using a sample retail dataset. They are examples of query syntax, not verified outputs from the Azure lab.

**SELECT, WHERE & ORDER BY – Orders over 100**

```sql
SELECT OrderID, ProductName, Revenue
FROM Sales
WHERE Revenue > 100
ORDER BY Revenue DESC;
```

**GROUP BY – Total revenue per category**

```sql
SELECT Category, SUM(Revenue) AS TotalRevenue
FROM Sales
GROUP BY Category
ORDER BY TotalRevenue DESC;
```

**JOIN – Revenue by customer city**

```sql
SELECT c.City, SUM(s.Revenue) AS TotalRevenue
FROM Sales AS s
INNER JOIN Customers AS c
    ON s.CustomerID = c.CustomerID
GROUP BY c.City
ORDER BY TotalRevenue DESC;
```

---

## 📁 Repository Contents

- Cloud computing notes and service model comparisons
- Azure Pricing Calculator estimate
- Azure SQL Database, Storage Account, Cosmos DB, and Fabric lab screenshots
- Power BI sales report
- Data protection, Computer Misuse Act, and copyright notes
- Scenario-based Azure recommendations for "Paws & Whiskers"

---

## 🧠 Key Learning Outcomes

Throughout this project, I strengthened my ability to:

- Identify suitable cloud service models for different business needs
- Estimate Azure costs using the Pricing Calculator
- Distinguish between relational and non-relational data
- Understand Azure SQL Database, Storage Accounts, and Cosmos DB
- Explain data ingestion, storage, analysis, and visualisation in Microsoft Fabric
- Use SQL to query, filter, aggregate, and combine data
- Present data through Power BI visualisations
- Understand relevant legal and data protection principles, including GDPR and the Data Protection Act 2018

---

## 🛠 Tools & Technologies Used

- Microsoft Azure
- Azure SQL Database
- Azure Storage Account
- Azure Cosmos DB
- Microsoft Fabric (Lakehouse and Eventstreams)
- Azure Pricing Calculator
- Skillable Labs
- SQL
- Power BI

---

## 📘 Scenario Work (Example: "Paws & Whiskers" Pet Shop)

The project included designing a proposed Azure-based solution for a pet shop that currently manages its data using spreadsheets.

### ✔️ Data Laws & Compliance

- General Data Protection Regulation (GDPR)
- Data Protection Act 2018
- Computer Misuse Act
- Copyright considerations
- Secure handling of customer and payment data

### ✔️ Azure Service Recommendations

- **Azure SQL Database** for sales, inventory, and customer records
- **Azure Blob Storage** for files and larger datasets
- **Azure Data Factory** for automated data collection and transformation
- **Azure Machine Learning** for potential customer behaviour analysis
- **Azure Synapse Analytics** for large-scale analytics and reporting

*These are proposed services for the scenario, not services claimed to have been implemented.*

### ✔️ Data Modelling & Storage

- Customer, transaction, pet inventory, and product category data
- Data formats: CSV, JSON, and Parquet
- Encryption, access control, backup, and disaster recovery
- Power BI dashboards to support management decisions

---

## 📸 Screenshots

### 1. Azure SQL Database Lab

The Dealership database was provisioned on `sqlserver66287031`, queried using SQL, and deleted after the lab to avoid ongoing charges.

### 2. Azure Storage Account Lab

The `st0rage99` storage account in France Central was used to explore Blob Storage, Data Lake Storage Gen2, and Azure Files.

### 3. Azure Cosmos DB Lab

The `accountonon` Cosmos DB account in West US 2 was used to add and query JSON items, demonstrating non-relational NoSQL data.

### 4. Microsoft Fabric Lab

Explored the Fabric workspace, OneLake catalog, and Real-Time section during the Lakehouse and streaming analytics exercises.

### 5. Power BI Sales Report

Power BI report includes revenue by category (bar chart), quantity by category (pie chart), and revenue by city (map).

<img width="1134" height="672" alt="Screenshot 2026-10-29 at 14 30 04" src="https://github.com/user-attachments/assets/5669ae2f-060f-4bf0-a68f-72c39def24af" />


---

## ✨ About the Author

**Hudefe Bare**  
Aspiring Data Analyst

Data Technician trainee, developing practical skills in:

- Cloud Computing (Microsoft Azure)
- Data Analytics (SQL and Power BI)
- Microsoft Fabric
- Data visualisation and reporting
