![Prohect Banner](banner.png)

# AdventureWorks 2016 — Extended  
**Transforming operational history into insight-driven business recovery**

[![MS Fabric](https://img.shields.io/badge/MS%20Fabric-Cloud-blue?logo=microsoft)](https://learn.microsoft.com/en-us/fabric/get-started)
[![Power BI](https://img.shields.io/badge/Power%20BI-Business%20Analytics-yellow?logo=power-bi)](https://powerbi.microsoft.com/)
[![Data Engineering](https://img.shields.io/badge/Data%20Engineering-ETL-orange?logo=apache-airflow)](https://en.wikipedia.org/wiki/Data_engineering)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-Database-red?logo=microsoftsqlserver)](https://www.microsoft.com/en-us/sql-server)
[![Power BI Gateway](https://img.shields.io/badge/Power%20BI%20Gateway-Connect-green?logo=power-bi)](https://learn.microsoft.com/en-us/data-integration/gateway/service-gateway-install)
[![Data Pipelines](https://img.shields.io/badge/Data%20Pipelines-Fabric-blueviolet?logo=apache-airflow)](https://learn.microsoft.com/en-us/fabric/data-pipelines)
[![Fabric Lakehouse](https://img.shields.io/badge/Fabric%20Lakehouse-Data%20Lake-lightblue?logo=databricks)](https://learn.microsoft.com/en-us/fabric/overview)
[![Report Writing](https://img.shields.io/badge/Report%20Writing-Documentation-green?logo=read-the-docs)](https://en.wikipedia.org/wiki/Technical_writing)
[![Business Intelligence](https://img.shields.io/badge/Business%20Intelligence-BI-yellow?logo=tableau)](https://en.wikipedia.org/wiki/Business_intelligence)
[![Analytics Development](https://img.shields.io/badge/Analytics%20Development-Data%20Insights-orange?logo=apache-superset)](https://en.wikipedia.org/wiki/Data_analysis)

> *An end-to-end, reproducible analytics experience built on Microsoft Fabric & Power BI.*

---

## 🚀 Executive Summary

This project reimagines the legendary **AdventureWorks 2016** dataset as a modern, enterprise-grade analytics showcase.  
It demonstrates how raw historical data can be converted into **executive-ready dashboards**, **root cause analysis**, and **actionable recovery playbooks** — bridging business goals with technical excellence.

**Key Value:**
- Enterprise-scale reproducibility using Fabric & Power BI
- Storytelling dashboards designed for decision-makers
- Governed, documented, and performance-tuned semantic models
- Real-world business scenarios for sales, product, and customer analytics

---

## 🏢 What is AdventureWorks?

**AdventureWorks** is Microsoft’s flagship sample database — a fictional manufacturing and retail company that produces and sells bicycles and related accessories.  
Originally designed to demonstrate SQL Server features, it has become a global benchmark dataset for showcasing modern data engineering, analytics, and visualization techniques.

This **Extended Edition** has 10 years Reseller data from 2005 - 2014, transforming it from a static demo into a **real-world enterprisse analytics case study** that mirrors how organizations evolve from historical data to actionable business intelligence. 


## 🧭 System Architecture

![Architecture](Architecture.png)

---

## 📊 Live Report Gallery

Below are embedded, fully interactive Power BI reports hosted as `.html` files on GitHub Pages.  
> 💡 *Best viewed in full-screen mode for high-resolution visuals.*

### 1️⃣ 📈 Executive Performance Dashboard

[🔗 View Performance Report (New tab)](https://awesomeanil.github.io/adventureworks-2016-extended/Performance.html)


<iframe title="Performace" width="600" height="486" src="https://app.powerbi.com/view?r=eyJrIjoiMTQ4OWRmYjMtMzNkNi00MmI3LTk0YzYtOWFjMWMzYTMxYzIyIiwidCI6ImY2NTRlNzkxLWY4NTgtNDZkNi05MWE5LTE5YzlmZTA4YTc0ZiJ9" frameborder="0" allowFullScreen="true"></iframe>

---

### 2️⃣ 🏪 Reseller Sales Dashboard

[🔗 View Resller Sales Report](https://awesomeanil.github.io/adventureworks-2016-extended/ResellerSales.html)

[![Reseller Report](https://img.shields.io/badge/View-Reseller%20Report-green)](https://awesomeanil.github.io/adventureworks-2016-extended/ResellerSales.html)

---

### 3️⃣ 🌐 Internet Customer Sales Dashboard

[🔗 View Internet Sales Report](https://awesomeanil.github.io/adventureworks-2016-extended/InternetSales.html)

[![Internet Report](https://img.shields.io/badge/View-Internet%20Report-blue)](https://awesomeanil.github.io/adventureworks-2016-extended/InternetSales.html)


---

## 🧩 Project Structure

| Path | Purpose |
|------|----------|
| `docs/` | Full documentation: architecture, governance, and playbooks |
| `power bi/` | pdf of Power BI reports |
| `reports/` | Internet Sales, Reseller Sales CSV's |
| `images/` | for images and screenshots |
| `sample_data/` | Sample datasets and dictionaries (synthesized or masked) |

---

## 🧠 Business Scenarios

| Area | Use Case | KPI Focus |
|------|-----------|-----------|
| **Sales Recovery** | Identify top declining product families | Quota Attainment %, YoY Delta |
| **Customer Intelligence** | Segment profitable vs at-risk customers | Retention %, Margin Contribution |
| **Product Performance** | Detect overstock and replenishment risk | Inventory Aging, Fill Rate |
| **Operational Efficiency** | Uncover channel and region variance | Cycle Time, Lead Response |

---

## ⚙️ Technical Highlights

- **Fabric-based Lakehouse** pattern with structured zones  
- **Delta-style parquet tables** for data reproducibility  
- **Semantic model design** using dimensional schemas and DAX measures  
- **Interactive dashboards** tailored for storytelling and decision velocity  

---

## 🧰 How to Run Locally

> Requires Docker, Python 3.10+, and Power BI Desktop.

```bash
# Clone
git clone https://github.com/AwesomeAnil/adventureworks-2016-extended.git
cd adventureworks-2016-extended

# Start reproducible environment
docker-compose up --build -d

# (or) manually run ETL
python scripts/etl/load_stage.py --config configs/local.yml

# Launch Jupyter notebooks
http://localhost:8888
```
---

## 📘 Documentation Index

| Document | Description |
|-----------|--------------|
| [Analysis_flow](Analysis_flow.md) | End-to-end system overview and workflows |
| [EXEC_1PAGER](EXEC_1PAGER.md) | EXEC 1 Page Summary |
| [PRESENTATION](PRESENTATION.md) | Board-room ready Presentation |
| [Contributing](Contributing.md) | Contributing guidelines |
| [Environment](Environment.md) | Setting up your environment |
| [Configuration](Configuration.md) | Configurations |


---

## 🏁 Outcomes & Value

| Stakeholder | Outcome |
|--------------|----------|
| **Executives** | Clear story from KPIs → Root Cause → Recovery Plan |
| **Analysts** | Reusable models and validated data lineage, Governance, controls |
| **Developers** | Modular ETL, semantic model, and Governance, Data Engineerig, Fabric OneLake, Fabric Warehouses |

---

## 📍 Roadmap

- [ ] CI for notebook reproducibility  
- [ ] ML-driven anomaly detection (v2)  
- [ ] Advanced scenario simulation & forecasting module  
- [ ] Multi-tenant deployment template  

---

## 👤 Author

**Anil Jacob**  
*Data Strategy • BI Governance • Analytics Leadership*  
🌐 [GitHub](https://github.com/AwesomeAnil)  
💼 [Reach me on LinkedIn](https://linkedin.com/in/anil-jacobs)  

---

> “Data only matters when it drives better business outcomes.”  
> — *AdventureWorks Extended, by Anil Jacob*
