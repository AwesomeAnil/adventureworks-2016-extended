# ⚙️ Configuration

---

## 🔧 Environment Setup and Configuration Steps

This section details the step-by-step configuration and setup required to replicate the AdventureWorks 2016 Extended Reseller & Internet Sales analysis project.

### 1. Create a Microsoft Fabric Trial Capacity
- Visit [Microsoft Fabric Trial Capacity](https://learn.microsoft.com/en-us/fabric/get-started)
- Sign in using your Microsoft or Azure account.
- Activate the Fabric trial which provides access to Lakehouse, Data Pipelines, and other Fabric components.

### 2. Download AdventureWorks 2016 `.bak` File
- Download the AdventureWorks2016 `.bak` file from the official Microsoft repository:  
  [AdventureWorks 2016 Sample Database on GitHub](https://github.com/microsoft/sql-server-samples/releases/tag/adventureworks)
- Save the file locally for restoration.

### 3. Restore AdventureWorks 2016 Backup to Local SQL Server
- Install SQL Server Express or Developer Edition and SQL Server Management Studio (SSMS) if not already installed.
- Open SSMS and connect to your local SQL Server instance.
- Right click `Databases` → `Restore Database` → Select the downloaded AdventureWorks2016 `.bak` file → Complete the restore process.

### 4. Configure Power BI Gateway for Local SQL Server
- Download and install the Power BI Gateway from the Microsoft website:  
  [Power BI Gateway](https://learn.microsoft.com/en-us/data-integration/gateway/service-gateway-install)
- Sign in with the same Microsoft account you used for Fabric.
- Add a data source pointing to your restored AdventureWorks SQL Server database.
- Configure credentials and test connectivity.

### 5. Create and Run Copy Data Pipeline in Microsoft Fabric
- Log into your Microsoft Fabric workspace.
- Navigate to the Data Engineering or Pipelines section.
- Create a new Copy Data pipeline job.
- Set the source as your on-prem SQL Server (via the Power BI Gateway data source).
- Select AdventureWorks tables needed (Reseller Sales, Internet Sales, Product, Customer, Date, etc.).
- Set the destination as your Fabric Lakehouse.
- Run the pipeline and monitor its execution until complete.

---

This setup allows your Fabric workspace to contain the AdventureWorks data ready for analytics and reporting using Power BI.
