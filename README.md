# 🛒 E-commerce Sales Analysis: SQL & Python Pipeline

An end-to-end data engineering and analysis project. This project automates the migration of raw e-commerce data from CSV files into a MySQL database and provides deep-dive business insights using SQL window functions and Python visualizations.

## 📂 Project Structure
- `notebooks/`
    - `CSV_to_SQL.ipynb`: Python script for ETL (Extract, Transform, Load) to MySQL.
    - `Ecommerce_Sales.ipynb`: SQL-based analysis and Seaborn/Matplotlib visualizations.
- `requirements.txt`: List of necessary Python libraries.
- `data/`: Contains sample datasets (full data hosted externally).

## 📊 Dataset
Due to the large size (100MB+), the full dataset is hosted on Google Drive.
- **[Download Full Dataset Here](https://drive.google.com/drive/folders/1pwsltDrJ2OfskANWtcNQ2xjSlhbusQk_?usp=drive_link)**

The dataset includes 7 tables: `customers`, `geolocation`, `order_items`, `orders`, `payments`, `products`, and `sellers`.

## 🚀 Key Features
- **Automated Schema Mapping:** The ETL script dynamically detects data types to create MySQL tables automatically.
- **Advanced SQL Queries:** - Used `DENSE_RANK()` and Window Functions to identify top-spending customers.
  - Calculated year-over-year sales growth and order distribution by city.
- **Data Visualization:** Created bar plots and trend lines to visualize customer behavior and payment patterns.

## 🛠️ Installation & Setup
1. **Clone the Repo:**
   ```bash
   git clone [https://github.com/gouravpatidar326/Ecommerce-Sales-Analysis.git](https://github.com/gouravpatidar326/Ecommerce-Sales-Analysis.git)
