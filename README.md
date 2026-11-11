# Novamart – Retail Data Engineering Project

## 1. Project Overview

Novamart is a retail data engineering project designed to build a scalable data processing and analytics solution using Microsoft Fabric and PySpark.

The project brings together data from multiple retail business areas, including POS sales, e-commerce, inventory, product master, customer master, and returns.

The objective is to process raw data, perform data quality checks, transform data using PySpark, and organize it into a Medallion Architecture (Bronze, Silver, and Gold) for analytical reporting.

## 2. Business Problem

Retail businesses generate data from multiple sources. However, inconsistent schemas, missing values, duplicate records, invalid stock values, and inconsistent customer information can affect reporting accuracy.

This project aims to address these challenges by:

- Integrating data from multiple retail sources.
- Identifying missing, duplicate, and invalid records.
- Standardizing and cleaning raw datasets.
- Building reusable data transformation workflows.
- Preparing trusted datasets for business analytics.

## 3. Project Architecture

The project follows the Medallion Architecture:

- **Bronze Layer:** Stores raw source data.
- **Silver Layer:** Contains cleaned, standardized, and validated data.
- **Gold Layer:** Contains business-ready datasets and aggregations for reporting.

See [Project Architecture](architecture/novamart_architecture.md).

## 4. Data Sources

| Dataset | Description |
|---|---|
| POS Sales | Point-of-sale transaction data |
| E-commerce | Online orders and transaction details |
| Inventory | Product stock and reorder information |
| Customer Master | Customer details and loyalty information |
| Product Master | Product, category, brand, and pricing information |
| Returns | Product return transactions |

## 5. Technologies Used

- Microsoft Fabric
- OneLake
- Lakehouse
- PySpark
- Python
- Delta Lake
- Medallion Architecture
- GitHub

## 6. Current Implementation Progress

- Created Microsoft Fabric workspace and Lakehouse.
- Organized raw source datasets in OneLake.
- Created a PySpark notebook for raw data profiling.
- Performed data quality checks on POS sales, inventory, e-commerce, customer, and product datasets.
- Identified missing values, duplicate records, and invalid stock records.
- Standardized customer master data.
- Created and verified the `silver_customers` Delta table.

## 7. Target Implementation

The remaining development work includes:

- Completing profiling and validation for all source datasets.
- Developing Silver-layer transformations for remaining datasets.
- Building Gold-layer analytical tables.
- Implementing data pipelines and automation.
- Connecting curated data to Power BI for reporting.

## 8. Repository Structure

```text
novamart-retail-analytics/
│
├── notebooks/
│   └── nb_00_profile_raw.ipynb
│
├── architecture/
│   └── novamart_architecture.md
│
├── documentation/
│
├── README.md
└── .gitignore
```

## 9. Project Objective

The final objective is to develop an end-to-end retail data engineering solution that converts raw retail data into clean, reliable, and analytics-ready datasets using Microsoft Fabric and PySpark.

---

**Project:** Novamart – Retail Data Engineering  
**Platform:** Microsoft Fabric  
**Processing:** PySpark and Delta Lake  
**Version Control:** GitHub
