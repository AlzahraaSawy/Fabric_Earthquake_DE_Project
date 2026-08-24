# 🌍 Worldwide Earthquake Data Engineering Pipeline (Microsoft Fabric)

An end-to-end Data Engineering solution built in **Microsoft Fabric** using the **Medallion Architecture**. This pipeline ingests live seismic event data from the USGS API, processes and cleans it using PySpark, aggregates business metrics, and serves it via Power BI.

---

## 📐 Architecture Overview

`USGS Earthquake API` ➡️ **Bronze (Raw JSON)** ➡️ **Silver (Structured PySpark)** ➡️ **Gold (Analytics)** ➡️ **Power BI Dashboard**

- **Ingestion:** Data Factory Orchestration fetching data from USGS REST API.
- **Processing Engine:** PySpark on Fabric Lakehouse.
- **Orchestration:** Sequential Data Pipeline (Bronze ➔ Silver ➔ Gold).

---

## 📂 Repository Structure

```text
├── notebooks/
│   ├── 01_bronze_ingestion.py
│   ├── 02_silver_cleaning.py
│   └── 03_gold_aggregation.py
├── Dashboard
└── README.md

```
<img width="1389" height="894" alt="Screenshot 2026-08-24 074512" src="https://github.com/user-attachments/assets/0890ea7a-6bed-41eb-b0ae-f8ea8355aa87" />

