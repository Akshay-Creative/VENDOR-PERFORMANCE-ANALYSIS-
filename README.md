# 📦 Inventory Analytics & Data Pipeline

An end-to-end data pipeline and analytics project that ingests raw retail/inventory CSV datasets into a SQLite relational database, performs exploratory data analysis (EDA) using Python & SQL, and delivers interactive visual insights through a Power BI dashboard.

---

## 📌 Project Overview

This project simulates a complete business intelligence & ETL (Extract, Transform, Load) workflow:
1. **Data Ingestion (ETL)**: Automatically loads raw inventory and vendor data into a centralized SQLite database (`inventory.db`) with custom logging.
2. **Exploratory Data Analysis (EDA)**: Analyzes stock turnover, purchasing efficiency, vendor invoice accuracy, and profit margins.
3. **Data Visualization**: Features an interactive Power BI dashboard (`dashboard.pbix`) for executive decision-making.

---

## 📁 Repository Structure

```text
├── data/                         # Directory containing raw CSV files
│   ├── begin_inventory.csv       # Starting inventory levels & valuations
│   ├── end_inventory.csv         # Ending inventory levels & valuations
│   ├── purchase_prices.csv       # Catalog purchase prices per item/vendor
│   └── vendor_invoice.csv        # Vendor billing and invoice transactions
├── logs/                         # Pipeline execution logs
│   └── ingestion_db.log          # Automated log outputs
├── ingestion_db.py               # Main Python ETL script for SQLite ingestion
├── Exploratory Data Analysis.ipynb  # Jupyter notebook for deep-dive EDA & SQL analysis
├── excel to db file .ipynb      # Notebook prototype for data ingestion testing
├── dashboard.pbix                # Interactive Power BI report dashboard
├── requirements.txt              # Python dependency file
├── .gitignore                    # Specifies files/folders ignored by Git
└── README.md                     # Project documentation
