# 🛒 Supermarket Sales Analytics Dashboard  
### End-to-End Data Analytics Portfolio Project

This project is a complete, real-world **end-to-end data analytics portfolio project** built using **Python, MySQL, and Power BI**.  
It simulates how data analysts work in retail and FMCG domains — from raw data cleaning and exploratory analysis to database integration and business-ready dashboards.

The focus of this project is not just visualization, but the **entire analytics workflow**: data preprocessing, feature engineering, EDA, SQL-based data storage, and insight-driven reporting.

---

## 📌 Project Overview

The objective of this project is to analyze supermarket sales data and answer key business questions such as:

- How do sales and profit vary across product categories?
- Do member customers purchase more than normal customers?
- Which branch performs better in terms of profit?
- How do sales change over time?
- At what time of day are sales highest?

The project follows a **real-world analytics pipeline**, where cleaned and engineered data is stored in a database and consumed by a BI tool for interactive analysis.

---

## 📁 Dataset Overview

- **Source:** Supermarket Sales Dataset (Kaggle)  
- **Rows:** 1000  
- **Columns:** 17  
- **Data Type:** Transaction-level supermarket sales data  

Each row represents a single transaction recorded at a supermarket branch.

### 🧾 Key Columns
- `invoice_id` – Unique transaction identifier  
- `branch`, `city` – Store information  
- `customer_type`, `gender` – Customer attributes  
- `product_line` – Product category  
- `unit_price`, `quantity`, `sales`, `gross_income` – Financial metrics  
- `date`, `time` – Transaction timestamp  
- `payment`, `rating` – Payment method and customer rating  

---

## 🔧 Project Workflow

### 1️⃣ Data Cleaning & Preparation (Python – Pandas)
- Loaded raw CSV data into Jupyter Notebook
- Standardized column names
- Checked for missing values and duplicates
- Validated and corrected data types
- Converted date and time fields into datetime format

---

### 2️⃣ Feature Engineering
Created additional features to support deeper analysis:
- `month`
- `day_name`
- `is_weekend`
- `hour`
- `time_of_day` (Morning / Afternoon / Evening)

---

### 3️⃣ Exploratory Data Analysis (EDA) – Python

The following business-driven insights were explored using Pandas and Matplotlib:

- **Sales vs Profit by Product Line**  
  Higher sales generally align with higher profit, though the relationship varies across product categories.

- **Unit Price vs Quantity Sold**  
  No strong negative relationship was observed between unit price and quantity sold.

- **Member vs Normal Customers**  
  Member customers spend slightly more per transaction and purchase marginally higher quantities.

- **Profit by Branch**  
  Profit levels are relatively balanced across branches, with Giza showing a slight lead.

- **Sales by Time of Day**  
  Afternoon generates the highest sales across all branches.

---

## 🗄️ Database Integration (MySQL)

After data cleaning and feature engineering:
- Data was stored in a MySQL database named **`sales_analysis`**
- A table **`sales_transactions`** was created
- Data was inserted using **SQLAlchemy**

This simulates a production-like setup where BI tools consume data from a centralized database.

---

## 📊 Power BI Dashboard

The Power BI dashboard connects directly to the MySQL database and includes the following pages:

### 🏠 Home
- Landing page with navigation and project context

### 📈 Overview
- KPI cards (Total Sales, Total Profit, Quantity Sold, Average Rating)
- Sales trend over time
- Sales by branch
- Sales by product line
- Interactive slicers

### 🔍 Insights
- Product performance analysis
- Customer behavior comparison
- Branch-level profitability
- Time-based sales patterns

---

## 📊 Dashboard Preview

<img width="1380" height="775" alt="image" src="https://github.com/user-attachments/assets/df85c418-1069-45c5-9a0f-c7e5eee69958" />
<img width="1375" height="776" alt="image" src="https://github.com/user-attachments/assets/dce83d02-f7db-4345-9265-d8ef533be1e9" />
<img width="1378" height="776" alt="image" src="https://github.com/user-attachments/assets/4d9862f9-5112-4ef7-a206-d66cfa27e0e1" />

---

## 📊 Key Business Insights (Summary)

- Afternoon is the highest sales period across branches  
- Member customers demonstrate slightly higher purchase behavior  
- Product categories with higher sales generally generate higher profit  
- Branch profitability is balanced with minor variations  

---

## 🛠️ Tools & Technologies Used

- **Python** (Pandas, Matplotlib)
- **MySQL**
- **Power BI**
- **Jupyter Notebook**

---

## ✅ Conclusion

This project demonstrates a complete **end-to-end analytics workflow**, closely resembling real-world data analyst responsibilities. It highlights the importance of data cleaning, feature engineering, and exploratory analysis before building dashboards. By combining Python, SQL, and Power BI, the project delivers scalable, business-focused insights rather than isolated visualizations.

---

## 👨‍💻 Author

**Shubham Zarkar**  
Aspiring Data Analyst | Python • SQL • Power BI  

---

### ⭐ Thanks for checking out the project!

If you found this project useful, feel free to **star ⭐ the repository**, fork it, or use it as inspiration for your own analytics portfolio.


