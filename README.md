# 📊 Azure Data Fundamentals (DP-900) – Cloud Data Services & Analytics Project

*A hands-on project covering cloud computing fundamentals, Azure data services, and analytical workloads in Microsoft Fabric.*

---

## 🛠 Core Technologies (Visual Overview)

[Azure SQL Database](https://azure.microsoft.com/en-us/products/azure-sql/database/) · [Azure Storage Account](https://azure.microsoft.com/en-us/products/storage/) · [Azure Cosmos DB](https://azure.microsoft.com/en-us/products/cosmos-db/) · [Microsoft Fabric](https://www.microsoft.com/en-us/microsoft-fabric) · Power BI

---

## 🔍 Overview

This repository contains my Week 5 Azure Data Fundamentals (DP-900) work, completed as part of the Data Technician training course.

The project covers cloud computing concepts, Azure cost estimation, relational and non-relational data services, data ingestion, and analytics using Microsoft Fabric and Power BI. It also includes hands-on Azure labs and a scenario-based solution design for a pet shop, "Paws & Whiskers".

---

## 🚀 Skills Demonstrated

### ✔️ Cloud Computing Fundamentals

- Understanding IaaS, PaaS, and SaaS with real-world examples
- Public, private, hybrid, and community cloud models
- Benefits and risks of cloud adoption, including scalability, flexibility, reliability, and unexpected costs
- Comparing cloud services with on-premises infrastructure
- Understanding major cloud providers: AWS, Microsoft Azure, and Google Cloud
- Estimating cloud costs using the Azure Pricing Calculator

### ✔️ Relational Data – Azure SQL Database

- Provisioned an Azure SQL Database and SQL server
- Created tables, loaded sample data, and queried it using SQL
- Worked with structured relational data
- Deleted resources after completing the lab to avoid ongoing costs

### ✔️ Non-Relational Data – Azure Storage Account & Azure Cosmos DB

- Created a storage account and explored Blob Storage, Data Lake Storage Gen2, and Azure Files
- Created an Azure Cosmos DB account
- Added JSON items and queried data using a SQL-like query language
- Explored non-relational NoSQL data storage

### ✔️ Analytical Workloads – Microsoft Fabric & Power BI

- Explored data analytics and real-time analytics in Microsoft Fabric
- Worked with Lakehouse concepts and data storage
- Built a Power BI sales report using bar, pie, and map visuals
- Connected data analysis with visual reporting and business insights

### ✔️ Data Ingestion

| **Method** | **Description** |
|---|---|
| ⚡ **Eventstreams** | Capture and route real-time streaming data into Fabric |
| 🔄 **Data pipelines** | Move and transform batch data from different sources |
| 📁 **File uploads** | Load CSV, JSON, and Parquet files into a Lakehouse or storage account |
| 🗄️ **Direct connections** | Connect Power BI to data sources such as SQL Server and Excel |

### ✔️ SQL Skills

Core SQL used to query, filter, sort, summarise, and combine retail and sales data.

| **SQL Clause** | **Purpose** |
|---|---|
| `SELECT` | Choose the columns to return |
| `WHERE` | Filter rows using a condition |
| `ORDER BY` | Sort results |
| `GROUP BY` | Calculate totals, counts, and averages |
| `JOIN` | Combine related tables |

Example queries using a sample retail dataset:

**SELECT, WHERE & ORDER BY – Orders over 100**

```sql
SELECT OrderID, ProductName, Revenue
FROM Sales
WHERE Revenue > 100
ORDER BY Revenue DESC;
```

**GROUP BY – Total revenue per product category**

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

*These are illustrative examples written to demonstrate SQL syntax on a sample retail dataset. They are not copied from the lab screenshots.*

---

## 📁 Repository Contents

- Cloud computing concepts and service model notes
- Azure Pricing Calculator estimate
- Azure SQL Database, Storage Account, Cosmos DB, and Fabric lab screenshots
- Power BI sales report
- Computer Misuse Act, copyright, and data protection notes
- Scenario-based Azure recommendations for "Paws & Whiskers"

---

## 🧠 Key Learning Outcomes

Throughout this project, I strengthened my ability to:

- Identify suitable cloud service models for different business requirements
- Estimate Azure costs using the Pricing Calculator
- Distinguish between relational and non-relational data
- Work with Azure SQL Database, Storage Accounts, and Cosmos DB
- Understand data ingestion, storage, analysis, and visualisation in Microsoft Fabric
- Use SQL to filter, sort, aggregate, and combine data
- Create Power BI visualisations to communicate sales insights
- Apply relevant UK data protection and legal principles, including GDPR and the Data Protection Act 2018

---

## 🛠 Tools & Technologies Used

- Microsoft Azure
- Azure SQL Database
- Azure Storage Accounts
- Azure Cosmos DB
- Microsoft Fabric (Lakehouse and Eventstreams)
- Azure Pricing Calculator
- Skillable Labs
- SQL
- Power BI

---

## 📘 Scenario Work (Example: "Paws & Whiskers" Pet Shop)

The project included designing an Azure-based solution for a pet shop that currently manages its data using spreadsheets.

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
- **Azure Synapse Analytics** for large-scale sales analysis and reporting

### ✔️ Data Modelling & Storage

- Customer, transaction, pet inventory, and product category data
- Data formats: CSV, JSON, and Parquet
- Encryption, access controls, backup, and disaster recovery
- Power BI dashboards to support management decisions

---

## 📸 Screenshots

### 1. Azure SQL Database Lab

The Azure portal after completing the lab. The Dealership database on `sqlserver66287031` was provisioned, queried using SQL, and then deleted to prevent ongoing charges.

### 2. Azure Storage Account Lab

The `dp900-lab-rg` resource group containing the `st0rage99` storage account in France Central. The lab explored Blob Storage, Data Lake Storage Gen2, and Azure Files before the resources were removed.

### 3. Azure Cosmos DB Lab

The `accountonon` Cosmos DB account in West US 2. JSON items were added and queried using a SQL-like language, demonstrating non-relational NoSQL data storage.

### 4. Microsoft Fabric Lab

The Fabric "My workspace" environment at the end of the analytics lab. The OneLake catalog and Real-Time sections were explored as part of the Lakehouse and streaming analytics exercises.

### 5. Power BI Sales Report

The final Power BI Desktop report, featuring revenue by category (bar chart), quantity by category (pie chart), and revenue by city (map visual).

---

## ✨ About the Author

**Hudefe Bare**  
Aspiring Data Analyst

Data Technician trainee

Developing practical skills in:

- Cloud Computing (Microsoft Azure)
- Data Analytics (SQL and Power BI)
- Microsoft Fabric
- Data visualisation and reporting
