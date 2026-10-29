📊 Azure Data Fundamentals (DP‑900) – Cloud Data Services & Analytics Project
A hands‑on project covering cloud computing basics, relational and non‑relational data in Azure, and analytical workloads in Microsoft Fabric.

🧰 Core Technologies (Visual Overview)
Azure SQL Database · Azure Storage Account · Azure Cosmos DB · Microsoft Fabric Lakehouse · Eventstreams · Power BI

🔎 Overview
This repository contains my Week 5 Azure Data Fundamentals (DP‑900) work, completed on the Data Technician training course. It walks through cloud computing concepts, Azure cost estimation, and three hands‑on labs: relational data (Azure SQL Database), non‑relational data (Azure Storage Account and Azure Cosmos DB) and large‑scale analytics (Microsoft Fabric and Power BI). It finishes with a scenario‑based Azure solution design for a pet shop, "Paws & Whiskers".

🚀 Skills Demonstrated
✅ Cloud Computing Basics
IaaS, PaaS and SaaS, with real‑world examples
Public, private, hybrid and community cloud models
Benefits and risks of moving to the cloud (scalability, cost savings, flexibility, reliability, unexpected costs)
Cloud vs on‑premises, and the main providers (AWS, Microsoft Azure, Google Cloud)
Cost estimation with the Azure Pricing Calculator (Design an enterprise BI solution template)
✅ Relational Data – Azure SQL Database
Provisioned an Azure SQL Database and SQL server
Created tables, loaded sample data and queried it with SQL
Cleaned up resources to avoid ongoing costs
✅ Non‑Relational Data – Azure Storage Account & Azure Cosmos DB
Created a storage account and explored Blob storage, Data Lake Storage Gen2 and Azure Files
Created a Cosmos DB account, added JSON items and queried them with a SQL‑like language
✅ Analytical Workloads – Microsoft Fabric Lakehouse
Explored data analytics and real‑time analytics in Microsoft Fabric
Built a Power BI sales report (bar, pie and map visuals)
✅ Data Ingestion
Method	Description
⚡ Eventstreams	Capture and route real‑time streaming data into Fabric
🔄 Data pipelines (Azure Data Factory / Fabric)	Move and transform batch data from different sources
📁 File upload	Load CSV, JSON and Parquet files into a Lakehouse or storage account
🗄️ Direct connections	Connect Power BI to data sources such as SQL Server and Excel
✅ SQL Skills
Core SQL used to analyse retail and sales data:

Clause	Purpose
SELECT	Choose the columns to return
WHERE	Filter rows by a condition
ORDER BY	Sort results
GROUP BY	Aggregate data (totals, counts, averages)
JOIN	Combine related tables
The queries below are illustrative examples on a sample retail dataset, written to show the syntax. They are not copied from the lab screenshots.

-- SELECT + WHERE + ORDER BY: top orders over 100
SELECT OrderID, ProductName, Revenue
FROM Sales
WHERE Revenue > 100
ORDER BY Revenue DESC;

-- GROUP BY: total revenue per product category
SELECT Category, SUM(Revenue) AS TotalRevenue
FROM Sales
GROUP BY Category
ORDER BY TotalRevenue DESC;

-- JOIN: revenue by customer city
SELECT c.City, SUM(s.Revenue) AS TotalRevenue
FROM Sales AS s
INNER JOIN Customers AS c ON s.CustomerID = c.CustomerID
GROUP BY c.City
ORDER BY TotalRevenue DESC;
📁 Repository Contents
Cloud concepts notes and service model tables
Azure Pricing Calculator estimate
Lab screenshots (Azure SQL, Storage Account, Cosmos DB, Fabric, Power BI)
Computer Misuse Act, copyright and data protection notes
Scenario‑based Azure recommendations for "Paws & Whiskers"
🧠 Key Learning Outcomes
Throughout this project, I strengthened my ability to:

Choose the right cloud service model (IaaS, PaaS or SaaS) for a business
Estimate Azure costs using the Pricing Calculator
Tell relational and non‑relational data apart and pick the right Azure service for each
Work with Azure SQL Database, Storage Accounts and Cosmos DB
Follow data from ingestion to analysis to visualisation in Microsoft Fabric
Apply UK law on computer misuse, copyright and data protection (GDPR, DPA 2018)
🛠 Tools & Technologies Used
Microsoft Azure
Azure SQL Database
Azure Storage Account
Azure Cosmos DB
Microsoft Fabric (Lakehouse, Eventstreams)
Azure Pricing Calculator
Skillable labs
Power BI
📘 Scenario Work (Example: "Paws & Whiskers" Pet Shop)
The project included designing an Azure‑based solution for a pet shop that currently keeps its data in spreadsheets.

✅ Data Laws & Compliance
GDPR
Data Protection Act 2018
Secure handling of customer and payment data
✅ Azure Service Recommendations
Azure SQL Database for sales, inventory and customer data
Azure Blob Storage for large datasets
Azure Data Factory for automated data collection
Azure Machine Learning for customer behaviour analysis
Azure Synapse Analytics for sales trends
✅ Data Modelling & Storage
Customer, transaction, pet inventory and product category data
Formats: CSV, JSON, Parquet
Encryption, access control, backup and disaster recovery
Power BI dashboards for management insight
📸 Screenshots
1. Azure SQL Database lab
Azure SQL Database lab The Azure portal after completing the lab: the Dealership database on sqlserver66287031 was provisioned, queried with SQL, then deleted to stop charges. The lab panel confirms relational data was created and queried in the cloud.

2. Azure Storage Account lab
Azure Storage Account lab The dp900-lab-rg resource group holding the st0rage99 storage account (France Central). This part covered blob storage, Data Lake Storage Gen2 and Azure Files before the group was deleted.

3. Azure Cosmos DB lab
Azure Cosmos DB lab The accountonon Cosmos DB account (West US 2, provisioned throughput, Online). JSON items were added and queried with a SQL‑like language, showing non‑relational NoSQL data.

4. Microsoft Fabric lab
Microsoft Fabric lab The Fabric "My workspace" at the end of the analytics lab, after the workspace was removed. The left menu shows OneLake catalog and Real‑Time, the areas used for Lakehouse storage and streaming ingestion.

5. Power BI sales report
Power BI sales report The final Power BI Desktop report: revenue by category (bar chart), quantity by category (pie chart) and revenue by city (map).

✨ About the Author
[Your Name]

Data Technician trainee

Building skills in:

Cloud Computing (Azure)
Data Analytics (SQL, Power BI)
Microsoft Fabric
