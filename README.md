https://app.fabric.microsoft.com/groups/344aaa97-5dad-409e-b06f-f0e783a69ca8/warehouses/12e1d2bc-e048-43c3-b2c9-679d7d52c1ac?experience=fabric-developer&clientSideAuth=0


# 🏥 Hospital Data Warehouse (Microsoft Fabric)

This project is a **Hospital Data Warehouse** developed using **Microsoft Fabric**, integrating multiple data sources to support healthcare analytics and decision-making.

---

## 🚀 Overview
The goal of this project is to centralize hospital operational data for analysis of treatments, patient trends, doctor performance, and medicine usage.

---

## 🧱 Architecture

**Tools & Services Used**
- Microsoft Fabric (Data Engineering, Data Warehouse, Power BI)
- PySpark Notebooks for ETL
- Delta Lake Storage
- T-SQL for Querying
- Power BI for Visualization

**Data Flow**
1. Source data imported into Lakehouse
2. PySpark used to transform and load into Delta tables
3. Fact and Dimension tables created following a Star Schema
4. Data Warehouse queried via T-SQL
5. Power BI connected for reporting

---

## 🧩 Star Schema Design

**Fact Table**
- `Fact_Patient_Treatment` — captures treatment, cost, doctor, and diagnosis details

**Dimension Tables**
- `Dim_Doctor`
- `Dim_Department`
- `Dim_Medicine`
- `Dim_Patient`
- `Dim_Date`

![Star Schema](docs/data_model.png)

---

## 🧮 Example Business Queries

Some advanced queries included in `/sql/business_queries.sql`:

- Top performing doctors by treatment success rate  
- Total revenue by department per month  
- Average medicine cost per diagnosis  
- Year-over-year patient growth  
- Treatment frequency by age group  

---

## 📊 Dashboards

Interactive dashboards built with **Power BI in Fabric** visualize:
- Patient admission trends
- Doctor workloads
- Financial performance
- Medicine stock insights

![Dashboard](docs/report_dashboard_screenshot.png)

---

## 👨‍💻 Author
**Nekmal Fernando**  
Bachelor of ICT (Level 3) — Data Warehousing Project  
