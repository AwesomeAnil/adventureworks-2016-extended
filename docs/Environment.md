# 🖥️ Environment Setup for AdventureWorks Sales Portfolio Analysis

---

## 🌐 Supported Operating Systems  
- Windows 10/11 (64-bit)  
- macOS (latest versions)  
- Linux (Ubuntu 20.04 LTS or later recommended)  

---

## 🛠️ Required Software & Tools  

| Tool                      | Purpose                                            | Notes                                                   |
|---------------------------|----------------------------------------------------|---------------------------------------------------------|
| **Microsoft Fabric Trial**| Data lakehouse, pipelines, and analytics platform | [Get started here](https://learn.microsoft.com/en-us/fabric/get-started) |
| **SQL Server Express/Developer** | Local relational database server                   | For restoring AdventureWorks `.bak` file                |
| **SQL Server Management Studio (SSMS)** | Database management, backup restore               | Latest version recommended                              |
| **Power BI Desktop**       | Interactive data visualization and reporting       | Use latest stable release                                |
| **Power BI Gateway**       | Connect on-prem SQL Server to Fabric lakehouse     | [Gateway setup guide](https://learn.microsoft.com/en-us/data-integration/gateway/service-gateway-install) |
| **Python 3.8+**            | Optional for advanced analysis, prediction          | With Pandas, Matplotlib packages                         |
| **Docker (optional)**      | Containerized SQL Server for isolated environment   | Recommended for ease of setup                            |

---

## ⚙️ Environment Configuration & Setup  

1. **Install and Configure SQL Server**  
   - Restore [AdventureWorks 2016 `.bak` file](https://github.com/microsoft/sql-server-samples/releases/tag/adventureworks) using SSMS.  
   - Validate connectivity and database integrity.

2. **Set up Power BI Gateway**  
   - Install and configure gateway on the machine hosting SQL Server.  
   - Link SQL Server data source with Microsoft Fabric workspace for secure data ingestion pipelines.

3. **Provision Microsoft Fabric Capacity**  
   - Activate Microsoft Fabric trial capacity (Lakehouse & Pipelines).  
   - Set up pipelines to import AdventureWorks data from SQL Server to Fabric Lakehouse.

4. **Power BI Desktop Setup**  
   - Connect reports to the Fabric Lakehouse datasets.  
   - Use provided dashboards or build custom visualizations as needed.

5. **(Optional) Python Environment**  
   - Set up a virtual environment (`venv` or `conda`).  
   - Install dependencies: `pandas`, `matplotlib`, `scikit-learn` (for any ML workflows).  

---

## 🔒 Security and Best Practices  

- Store sensitive credentials securely (environment variables or secret managers).  
- Do not commit any passwords, keys, or personal data to the repository.  
- Regularly update software to latest stable versions for security and feature improvements.  
- Use version control branches for development and testing to protect main branch stability.

---

## 💡 Troubleshooting Tips  

- Check SQL Server connection settings if data ingestion pipelines fail.  
- Ensure Power BI Gateway is up and running whenever scheduling or refreshing datasets.  
- Use Microsoft Fabric diagnostic logs for pipeline errors and performance monitoring.  

---

This environment setup ensures a robust, secure foundation for enterprise-grade sales data analytics and reporting using Microsoft Fabric, Power BI, and associated tools.

---
