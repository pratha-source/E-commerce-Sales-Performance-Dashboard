Retail Data Pipeline: SQL + Python + Power BI 🚀

📌 Project Overview:-
This project demonstrates an end-to-end data analytics workflow. It simulates a professional environment where data is extracted from a SQL database, processed using Python for advanced business logic, and finally visualized in an interactive Power BI dashboard.

The goal was to move beyond simple visualization and build a robust ETL (Extract, Transform, Load) pipeline to identify high-value sales trends and regional profit margins.

🛠️ Tech Stack:-
Language: Python 3.x
Libraries: Pandas, NumPy, Sqlite3
Database: SQL (SQLite)
BI Tool: Power BI Desktop
IDE: VS Code / Jupyter Notebooks

⚙️ The Pipeline
1. Data Extraction (SQL)
Instead of using static flat files, I used the sqlite3 library to create a relational database environment.
Querying: I used SQL SELECT and WHERE statements to extract specific columns and filter for significant transactions (Sales > $200).
Tool: Python-integrated SQL queries.

2. Data Transformation (Python)
Using VS Code and Pandas, I performed feature engineering to add "Business Intelligence" layers to the raw data:
Margin Calculation: Created a custom column for Margin_Percentage to evaluate profitability.
High-Value Tagging: Implemented a lambda function to categorize orders as "High-Value" based on revenue thresholds.
Data Cleaning: Handled missing values and standardized date formats for time-series analysis.

3. Data Visualization (Power BI)
The processed data was imported into Power BI to create a recruiter-ready dashboard.
Executive Insights: A dedicated "Insights" panel summarizing the Western Region's dominance and Technology sector growth.
Interactivity: Integrated Slicers for Categories and Segments to allow stakeholders to drill down into specific data points.
KPI Tracking: High-level cards for Total Sales ($2.26M) and Units Sold (9.8K).

📊 Dashboard Preview
<img width="875" height="489" alt="Screenshot 2026-03-19 231022" src="https://github.com/user-attachments/assets/ca8cdd91-b99d-4734-bd44-763ca3008d36" />

💡 Key Business Findings
Top Performer: The Western Region accounts for over 31% of total revenue.
Profit Leader: Technology is the highest-value category, despite lower order volume compared to Office Supplies.
Risk Area: Identified specific "High-Value" segments where profit margins are below 10%, suggesting a need for pricing adjustments.

📂 How to Run
Clone the repo: git clone https://github.com/your-username/your-repo-name
Run the Jupyter Notebook in the notebooks/ folder to generate the final_dashboard_data.csv.
Open the .pbix file in the dashboard/ folder to view the interactive report.
