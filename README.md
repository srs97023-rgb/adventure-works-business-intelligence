# adventure-works-business-intelligence
# 🚲 Adventure Works Manufacturing & Sales: End-to-End Analytics

An insight-driven analysis of Adventure Works sales, built four ways: **Excel → SQL → Power BI → Tableau**. Each tool answers a different part of the story, and all four arrive at the same validated numbers.

**$29.36M revenue • 60,398 order lines • 10 sales regions • 18,000+ customers • 41.1% profit margin**

![Project Overview](YOUR_OVERVIEW_IMAGE_LINK)
<img width="800" height="450" alt="image" src="https://github.com/user-attachments/assets/c2067c55-200e-4fc8-9779-2cec7ea29c5f" />

---

## 🧭 Project Roadmap

| Step | Tool | Role in the project | Details |
|---|---|---|---|
| 1 | 📗 **Excel** | Exploratory audit: pivot tables, KPIs and an interactive dashboard | [Excel README](https://github.com/srs97023-rgb/Excel-Project/blob/main/README.md) |
| 2 | 🗄️ **SQL (MySQL)** | Data engineering: merge tables, build a fiscal calendar, model revenue, cost and profit | [SQL README](https://github.com/srs97023-rgb/SQL-Project/blob/main/README.md) |
| 3 | 📊 **Power BI** | Monitoring: star-schema model, KPI cards and slicer-driven Executive Dashboard | [Power BI README](https://github.com/srs97023-rgb/Power-BI-Project/blob/main/README.md) |
| 4 | 📈 **Tableau** | Storytelling: Sales Performance Dashboard for board-level review | [Tableau README](https://github.com/srs97023-rgb/Tableau-Project/blob/main/README.md) |

**Live dashboards:** [Excel](YOUR_EXCEL_LINK) • [Power BI](YOUR_POWER_BI_LINK) • [Tableau](YOUR_TABLEAU_PUBLIC_LINK)

---

## 🎯 Business Questions

- How much revenue, cost and profit are we generating?
- How do sales change by year, quarter and month?
- Which products, customers and regions drive the most revenue?
- Where is profit margin strongest and weakest, and why?

## 🔎 The Story Across the Four Tools

**1. Excel: exploratory audit**
Pivot tables on 60,398 order lines revealed strong seasonality (Q4 is 31% of revenue versus 19% in Q1) and a heavy dependence on one category: **Bikes generate 96.5% of revenue from only 25% of order lines**, while Accessories drive about 60% of volume but just 2.4% of revenue. Margins were also lowest in the two biggest regions, and freight was ruled out as the cause, which pointed to product mix.

**2. SQL: data foundation**
Two raw fact tables (`FactInternetSales` and `Fact_Internet_Sales_New`) were merged with `UNION ALL` into `Fact_Sales_Combined`, enriched with product and customer names, and given a full date and financial calendar. Revenue was recalculated and validated, and a permanent `ProductionCost` (COGS) column confirmed the **41.1% portfolio margin**.

**3. Power BI: live monitoring**
An Executive Dashboard with Total Sales, Production Cost and Profit KPI cards, Year and Quarter slicers, a monthly seasonality trend, a sales-vs-cost combo chart, Top 5 Products and a geographic revenue split. Separate pages rank performance by customer, product and region.

**4. Tableau: executive storytelling**
A single Sales Performance Dashboard that puts Top 5 Products, Top 5 Regions and year, quarter and month trends in one view, with a sales-versus-production-cost chart to show margin pressure next to revenue growth.

---

## 💡 Key Insights

- **Total sales $29.36M**, production cost $17.28M and profit $12.08M, a **41.1% margin**.
- **2013 was the peak year** at $16.35M. 2010 and 2014 contain only partial data.
- **Q4 is the strongest quarter** (about 31% of revenue) and **December is the top month** at $3.21M.
- **Category concentration:** Bikes account for 96.5% of revenue, and the top 5 products are all Mountain-200 bikes ($6.67M, nearly a quarter of sales).
- **Australia is the #1 region** (about 31% of sales), followed by the Southwest and Northwest US.
- **Margin erosion in the biggest markets:** Australia (40.7%) and Southwest (41.5%) have the lowest net margins, versus 43 to 45% in the smallest regions. Freight is a flat 2.5% of sales everywhere, so the gap comes from product mix.
- **Consistent numbers:** the same revenue, cost and profit figures hold in SQL, Excel, Power BI and Tableau.

## 📈 Strategic Recommendations

1. **Category rebalancing:** examine whether Accessories and Clothing are under-priced or under-marketed relative to their order volume.
2. **Regional margin review:** audit the product mix in Australia and the Southwest, the highest-revenue and lowest-margin regions.
3. **Peak-season planning:** build inventory and staffing around the Q4 peak.
4. **Protect the anchor products:** secure supply of the Mountain-200 series while reducing dependence on it.

---

## 🛠️ Tech Stack

| Area | Tools |
|---|---|
| Spreadsheets | Microsoft Excel, Power Query, Pivot Tables, Slicers |
| Database | MySQL (Workbench) |
| BI | Power BI Desktop, Power Query, DAX |
| Visualization | Tableau Desktop / Tableau Public |

## 📁 Repository Structure

```
adventure-works-analytics/
├── README.md              ← you are here
├── Excel/
│   ├── README.md
│   └── EXCEL_ PROJECT_ADVENTURE WORKS.xlsx
│   └── Excel_Dashboard image.jpg
├── SQL/
│   ├── README.md
│   └── SQL_Project_Work_Adventure_works.sql
├── PowerBI/
│   ├── README.md
│   ├── POWER_BI_PROJECT_ADVENTURE_WORKS.pbix
│   └── PowerBI_Dashboard_image.jpg
├── Tableau/
│   ├── README.md
│   ├── TABLEAU_ PROJECT_ADVENTURE WORKS.twbx
│   └── Tableau_Dashboard_image.jpg
└── Presentation/
    └── Adventure_Works_Executive_Analytics_Presentation.pptx
```

> The Excel workbook is about 44 MB, so it is shared through the Drive link above rather than uploaded here.

## 🧠 Skills Demonstrated

Data cleaning and integration • SQL data engineering • Data modeling (star schema) • DAX • Pivot analysis • Interactive dashboard design • KPI design • Cross-tool validation • Business storytelling
