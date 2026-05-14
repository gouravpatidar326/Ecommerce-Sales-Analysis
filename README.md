🛒 E-commerce Sales Analysis: SQL & Python Pipeline
An end-to-end data engineering and analysis project. This project automates the migration of raw e-commerce data from CSV files into a MySQL database and provides deep-dive business insights using SQL window functions and Python visualizations.

📂 Project Structure
notebooks/

CSV_to_SQL.ipynb: Python script for ETL (Extract, Transform, Load) to MySQL.

Ecommerce_Sales.ipynb: SQL-based analysis and Seaborn/Matplotlib visualizations.

requirements.txt: List of necessary Python libraries.

📊 Dataset Information
Due to the file size (100MB+), the datasets are hosted externally. You must download them to run the analysis locally.

Full Dataset: Download from Google Drive - https://drive.google.com/drive/folders/1pwsltDrJ2OfskANWtcNQ2xjSlhbusQk_?usp=drive_link

Tables included: customers, geolocation, order_items, orders, payments, products, and sellers.

🚀 Key Features
Automated Schema Mapping: The ETL script dynamically detects pandas data types to generate and execute CREATE TABLE statements in MySQL automatically.

Advanced SQL Analytics: - Utilized DENSE_RANK() and Window Functions to identify top-spending customers per year.

Calculated year-over-year sales growth and geographic order distribution.

Data Visualization: Integrated Seaborn and Matplotlib to visualize payment trends and customer segmentation directly from SQL query results.

🛠️ Installation & Setup
1. Clone the Repo
Bash
git clone https://github.com/gouravpatidar326/Ecommerce-Sales-Analysis.git
cd Ecommerce-Sales-Analysis
2. Install Dependencies
Bash
pip install -r requirements.txt
3. Data Setup (Important)
Create a folder named data in the project root directory.

Download the CSV files from the Google Drive Link.

Place all 7 CSV files inside the data/ folder.

4. Database Configuration
Ensure your MySQL server is running.

Open notebooks/CSV_to_SQL.ipynb.

Locate the mysql.connector.connect() block and update the host, user, and password to match your local MySQL credentials.

5. Execution Order
To reproduce the analysis, run the notebooks in this order:

CSV_to_SQL.ipynb: Processes the CSVs and populates your MySQL database.

Ecommerce_Sales.ipynb: Runs the analytical queries and generates visualizations.
