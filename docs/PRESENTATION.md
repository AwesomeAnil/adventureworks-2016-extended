![Banner](banner.png)
# 🌎 AdventureWorks 2016 Extended — ReSeller Sales Performance Analysis (2005–2014)

---

## 🎯 Slide 1: Title & Context
**AdventureWorks 2016 Extended — ReSeller Sales Analysis**  
**Author:** Anilwhatsapp Mon  
**Purpose:** Showcase **technical mastery on MS Fabric** and **commercial insight** via multi-year reseller performance trends.  

> Leverages Fabric for enterprise data integration, historical analytics, and visual storytelling in Power BI.

---

## 💡 Slide 2: Motivation
**Why this analysis matters:**
- Demonstrates how **MS Fabric empowers analysts** to combine enterprise-scale datasets.  
- Historical data analysis reveals **trends, anomalies, and strategic insights**.  
- Visualized through **Power BI dashboards**, enabling **clear executive decision-making**.  
- Highlights skills that stakeholders & decision makers  **value for business intelligence, analytics, and commercial strategy roles**.  

### 📊 **AdventureWorks ReSeller Sales Analysis (2005–2014) Extended Version**



#### 🔹 1️⃣ Enterprise Data Access & Integration
- 🏞️ MS Fabric Lakehouse  
- 🖥️ On-prem SQL Server + Power BI Gateway  
- 🔗 Seamless integration of historical transactional data  

#### 🔹 2️⃣ Historical Analysis
- 📅 10 years of reseller data  
- 📈 Key measures: Avg Sales, Units Sold, Discounts appled, Unit Costs, Unit Prices  & Product Margins
- 🕵️‍♂️ Trend detection, anomaly spotting, scenario comparison  

#### 🔹 3️⃣ Insights & Inferences
- 💵 Revenue spikes vs. margin erosion  
- 🎯 Impact of discount campaigns on profitability  
- 📉 Identify sustainable vs. short-term strategies  

#### 🔹 4️⃣ Showcase Skills
- 📊 Power BI visualizations and dashboards  
- 🏛️ Boardroom-ready insights for executives  
- 💡 Demonstrates technical + business acumen  

---

### 🔹 🎯 Result
- ✅ Convincing storytelling for investors & recruiters  
- ✅ Highlights ability to translate enterprise data into strategic decisions  

---

## 🛠 Slide 3: Technical Architecture (MS Fabric + Power BI)
**Built Using:**
- **MS Fabric Data Lake:** Centralized, scalable repository for historical and transactional data.  
- **Power BI:** Multi-layer analytics and visualization, including:
  - Trend analysis (sales, units, discounts)  
  - Profitability modeling (gross margins, cost analysis)  
  - Scenario comparison (with/without discounts)  
- **Key Benefits of Fabric:**
  - Handles **large-scale datasets** efficiently  
  - Integrates with **Power BI** for instant visualization  
  - Enables **data-driven storytelling for executives and investors**

**[Insert architecture diagram icon + arrows for data flow]**

```mermaid
flowchart TD
    %% Section: Source and SQL Server Setup
    A1[📦 Source: AdventureWorks 2016.bak file] --> A2[🖥️ Install SQL Server + SSMS Docker Image Recommended]
    A2 --> A3[➕ Restore .bak file to SQL Server<br>→ On-Prem Database Ready]

    %% Section: Power BI Gateway
    A3 --> B1[🔌 Install Power BI Gateway]
    
    %% Section: Fabric Pipeline
    B1 --> C1[☁️ MS Fabric Trial Capacity]
    C1 --> C2[🆕 Create New Data Pipeline]
    C2 --> C3[🔗 Use Gateway to connect to SQL Server On-Prem]
    C3 --> C4[🏞️ Destination: AdventureWorks Fabric Lakehouse]
    C4 --> C5[▶️ Run Pipeline to Import Selected Tables]

    %% Section: Power BI Reporting
    C5 --> D1[📊 Build Power BI Reports connecting to AdventureWorks Lakehouse]

    %% Styling: Colors
    classDef source fill:#fef3c7,stroke:#f59e0b,stroke-width:2px,white-space:normal;
    classDef process fill:#dbeafe,stroke:#3b82f6,stroke-width:2px,white-space:normal;
    classDef output fill:#dcfce7,stroke:#16a34a,stroke-width:2px,white-space:normal;

    class A1,A2,A3 source;
    class B1,C1,C2,C3,C4,C5 process;
    class D1 output;

    %% Optional wider styling (if supported by Mermaid renderer)
    style A1 width:250px
    style A2 width:250px
    style A3 width:250px
    style B1 width:250px
    style C1 width:250px
    style C2 width:250px
    style C3 width:250px
    style C4 width:250px
    style C5 width:250px
    style D1 width:250px

```

---

## 📊 Slide 4: Key Measures & Methodology
**Measures Analyzed (FY 2005–2014):**
1. Avg Sales (w/ & w/o Discounts)  
2. Avg Discounts (%)  
3. Avg Product Costs  
4. Avg Unit Prices  
5. Avg Units per Transaction  
6. Gross Margins  
7. Total Sales  
8. Total Units Sold  

**Methodology:**
- Multi-table temporal analysis  
- Scenario comparison (actual vs. hypothetical)  
- Integrated insights on revenue, margin, pricing, and volume  

---

## 🚀 Slide 5: Revenue & Sales Trends
**Observation:**
- Peak **Total Sales in 2010 (\$2.597B)** driven by **transaction/volume surge**, not per-unit increases.  
- Units per transaction remained flat (~3.5 units).  
- Post-2012: sales returned to baseline (~\$948M) as promotional campaigns ended.  

**Total Sales by Fiscal Year & Category]**

![Total Sales](/images/Total_Sales.png)

---

## 💵 Slide 6: Pricing & Discounts Impact
- Discounts introduced 2010–2012 (3 → 13 %)  
- Avg Unit Prices dipped slightly during discount period  
- Gross Margins collapsed (negative for high-cost categories)  
- Revenue spike achieved **at the expense of profitability**  

**Avg Discounts**

![Average Discounts](/images/Avg_Discounts.png)

**Unit Prices**

![Unit Prices](/images/Unit_Price.png)

---

## 📈 Slide 7: Units & Volume Analysis
- **Avg Units per Transaction:** Stable (~3.5 units)  
- **Total Units Sold:** 2010 spike driven by expanded reseller activity  
- Revenue peak is **transaction-driven, not per-unit**  
- Post-promotion normalization by 2014  

**Total Units Sold by Fiscal Year & Category]**

![Total Units Sold](/images/Total_Units_Sold.png)

---

## 🏆 Slide 8: Profitability Insights
- **Category Profitability Hierarchy:** Accessories > Clothing > Components > Bikes  
- Temporary margin collapse 2010–2012 due to discounting strategy  
- Recovery by 2014 aligns with **sustainable pricing and discount strategy**  

**Gross Margins by Category & Year**

![Gross Margins](/images/GM.png)

---

## 🔍 Slide 9: Strategic Inferences
- Promotions boost revenue but reduce margins; careful calibration needed  
- Units per transaction show **resilience of reseller behavior**  
- Enterprise-level tools (Fabric + Power BI) enable **data-driven, boardroom-ready insights**  
- Demonstrates technical + business intelligence skills critical for recruiters  

---

## 🌐 Slide 9B: Internet Customer Sales — Business Insights (FY2010–2013)

### 1️⃣ Overview
The **Internet Sales** channel shows a compelling growth trajectory from FY2010–2013, revealing a deliberate strategic pivot from a *price-led* to a *volume-led* model.  
This section interprets that transformation using 22 aggregated tables (Total Sales, Average Sales, Transaction Counts, Discounts, and Geographical/Product dimensions).

---

### 2️⃣ Growth Composition Analysis
- **Total Sales Amount:** ↑ ~40–50% (FY2010–2013)  
- **Average Sales Amount:** ↓ 15–25% across geographies & products  
- **Transaction Counts:** ↑ 55–65%  

➡️ **Interpretation:**  
Growth was **volume-driven**, not price-driven.  
Management consciously dropped average unit prices to accelerate market share acquisition through penetration and reach.

---

### 3️⃣ Pricing & Margin Dynamics

| Indicator | FY2010 | FY2013 | Δ | Insight |
|------------|--------|--------|---|---------|
| Total Sales | ↑ | ↑↑↑ | +40–50% | Volume-led expansion |
| Avg Sales / Txn | ↓ | ↓↓ | –15–25% | Price dilution |
| Transaction Count | ↑ | ↑↑↑ | +55–65% | Market expansion |
| Discount / Sales Ratio | ~8% | ~12% | +4 pts | Higher promotional spend |

**Key Takeaway:**  
Internet Sales achieved growth by *buying volume*.  
Discounting intensity and lower ticket values indicate a market-penetration strategy that traded short-term margin for customer base growth.

---

### 4️⃣ Geographic & Product Portfolio Insights
- **North America:** Smaller drop in average sale; brand strength protected pricing.  
- **Europe & APAC:** Sharper declines (up to 30%); aggressive expansion through affordability.  
- **Product mix:** Mid-tier SKUs discounted heavily; premium SKUs retained price stability → **“barbell portfolio”** pattern.

➡️ **Interpretation:**  
Revenue grew via diversification, but average yield fell.  
Emerging markets and mid-tier products drove scale; mature markets anchored profitability.

---

### 5️⃣ Strategic Implications

| Theme | Evidence | Implication |
|--------|-----------|-------------|
| Volume-Led Expansion | Rising transactions, falling avg. sale | Market share up; margin pressure |
| Price Elasticity by Region | Europe/APAC more sensitive | Requires localized pricing governance |
| Discount Dependency | Rising discount ratio | Risk of sustained price erosion |
| Product Mix Shift | Mid-tier expansion | Broader reach, thinner margins |
| Margin Recovery Path | Flat avg. revenue per product | Efficiency or premiumization critical |

---

### 6️⃣ Boardroom-Level Conclusions
1. **Growth Quality:** Strong top-line expansion, but structurally margin-dilutive.  
2. **Strategic Intent:** Deliberate penetration phase — volume prioritized over yield.  
3. **Profitability Outlook:** Margin recovery now depends on:
   - Selective **premiumization**  
   - **Discount rationalization**  
   - **Regional pricing discipline**
4. **Future Levers:** Shift toward **yield optimization** — improve average sale value without losing scale.

---

### 7️⃣ Executive Summary
> Between FY2010–2013, Internet Sales delivered impressive top-line growth through a deliberate **volume-first strategy**.  
> While this built market scale, it also created structural margin challenges.  
> The next phase must balance **customer acquisition** with **sustainable yield management** — evolving from *growth-at-any-cost* to *profitable, price-disciplined expansion*.

---

## 📌 Slide 10: Executive Takeaways
1. Short-term revenue spikes can mask margin erosion.  
2. Fabric + Power BI combination enables **high-impact storytelling** from transactional data.  
3. Analysis confirms **pricing, discount, and volume strategies are tightly correlated** with profitability outcomes.  
4. Shows ability to derive **actionable insights** from complex enterprise datasets.  

---

## 📂 Slide 11: Appendix / Charts
- **Avg Sales w/ Discounts**

![Average Sales with Discounts](/images/Avg_sales_w_discounts.png) 

- **Avg Sales w/ Discounts (hypothetical)**

![Average Sales without Discounts](/images/Avg_sales_wo_discounts.png)

- **Product Cost trends**

![Average Product Costs](/images/Avg_Product_Costs.png)

---

## 📝 Slide 12: Licenses & Credits
- **AdventureWorks 2016 Extended Dataset:** Provided by Microsoft for learning and analysis purposes  
  - [Microsoft AdventureWorks Sample Databases](https://github.com/microsoft/sql-server-samples)  
- **Power BI:** Microsoft Power BI Desktop for visualization  
- **MS Fabric:** Microsoft Fabric for enterprise-scale data integration  
- Analysis, markdown preparation, and insights: **AwesomeAnil**  

---

## ✅ Slide 13: Closing / Call-to-Action
- AdventureWorks analysis demonstrates **technical, analytical, and commercial acumen**.  
- Ready for **investor, boardroom, or consultant presentation**.  
- Full Power BI dashboards and Fabric integration are **available for review**.  
- Highlights ability to **translate enterprise data into strategic, actionable insights**.  

