# customer_behaviour_analysis
Data analysis project showcasing customer behaviour analysis using SQL, Python and Power BI.
# 📊 [Project Name] – End-to-End Data Analytics Project

> *One-line summary: e.g., "Analyzing retail sales data to uncover revenue trends, top products, and customer behavior."*

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-PostgreSQL%20%7C%20MySQL%20%7C%20SQL%20Server-orange)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Table of Contents
1. [Overview](#-overview)
2. [Dataset](#-dataset)
3. [Tools & Technologies](#-tools--technologies)
4. [Project Steps](#-project-steps)
5. [Dashboard](#-dashboard)
6. [Results](#-results)
7. [Project Structure](#-project-structure)
8. [How to Run](#-how-to-run)
9. [Author](#-author)

---

## 🔍 Overview

This project demonstrates a complete data analytics workflow, from raw data to business insights. It covers data loading, exploratory data analysis (EDA), cleaning, SQL querying, interactive dashboarding, reporting, and presentation.

**Business Problem:**
*Describe the question you're answering. Example: "Which products, regions, and customer segments drive the most revenue, and where are the opportunities to grow?"*

**Objectives:**
- Clean and prepare raw data for analysis
- Identify key trends, patterns, and outliers
- Answer business questions using SQL
- Build an interactive Power BI dashboard for stakeholders
- Communicate findings through a report and presentation

---

## 📂 Dataset

| Item | Details |
|------|---------|
| **Source** | *e.g., Kaggle / company data / public API (add link)* |
| **Size** | *e.g., 10,000 rows × 15 columns* |
| **Time Period** | *e.g., Jan 2022 – Dec 2023* |
| **Format** | CSV |

**Key Columns:**

| Column | Description |
|--------|-------------|
| `order_id` | Unique order identifier |
| `order_date` | Date of purchase |
| `customer_id` | Unique customer identifier |
| `product_category` | Category of the product |
| `sales` | Revenue generated |
| `region` | Customer region |

*(Update the table with your actual columns.)*

---

## 🛠 Tools & Technologies

| Purpose | Tool |
|---------|------|
| Data Loading, EDA & Cleaning | Python (Pandas, NumPy, Matplotlib, Seaborn) |
| Database & Querying | PostgreSQL / MySQL / SQL Server |
| Dashboard | Power BI |
| Reporting | Word / PDF |
| Presentation | Gamma (AI-powered slides) |
| Version Control | Git & GitHub |

---

## 🚀 Project Steps

### 1. Data Loading
Loaded the dataset into Python using Pandas and reviewed its structure, data types, and size.

### 2. Exploratory Data Analysis (EDA)
- Summary statistics and distributions
- Missing value and duplicate checks
- Outlier detection
- Trend, category, and correlation analysis with visualizations

### 3. Data Cleaning
- Handled missing values and removed duplicates
- Fixed data types and standardized formats
- Treated outliers and created new features (e.g., month, year, profit margin)
- Exported the cleaned dataset for SQL and Power BI

### 4. SQL Analysis
Imported the cleaned data into a relational database and wrote queries to answer business questions, using:
- `JOIN`s, `GROUP BY`, and aggregations
- Subqueries and CTEs
- Window functions (e.g., `RANK()`, running totals)

**Sample Query:**
```sql
SELECT product_category,
       SUM(sales) AS total_sales,
       RANK() OVER (ORDER BY SUM(sales) DESC) AS sales_rank
FROM sales_data
GROUP BY product_category;
```

### 5. Power BI Dashboard
Connected Power BI to the cleaned data, built a data model, created DAX measures, and designed an interactive dashboard with filters and KPIs.

### 6. Report
Documented the methodology, key insights, and recommendations in a written report.

### 7. Presentation
Created a concise, visual slide deck with Gamma to present findings to non-technical stakeholders.

---

## 📈 Dashboard

![Dashboard Preview](images/dashboard.png)

**Key Features:**
- KPI cards: Total Sales, Profit, Orders, Average Order Value
- Time-series trend analysis
- Breakdown by category, region, and customer segment
- Interactive slicers and filters

🔗 **Live / Demo Link:** *[Add link if published]*

---

## ✅ Results

**Key Insights:**
- 📌 *Insight 1: e.g., "Technology category generated 38% of total revenue."*
- 📌 *Insight 2: e.g., "Sales peak in Q4, rising ~25% above the yearly average."*
- 📌 *Insight 3: e.g., "The West region has the highest sales but the lowest profit margin."*

**Recommendations:**
- *e.g., Focus marketing spend on high-performing categories during Q4.*
- *e.g., Review discounting strategy in low-margin regions.*

📄 **Deliverables:**
- [Full Report](reports/report.pdf)
- [Presentation (Gamma)](#) *(add link)*

---

## 📁 Project Structure

```
├── data/
│   ├── raw/                 # Original dataset
│   └── cleaned/             # Cleaned dataset
├── notebooks/
│   └── eda_and_cleaning.ipynb
├── sql/
│   └── queries.sql
├── dashboard/
│   └── dashboard.pbix
├── reports/
│   └── report.pdf
├── presentation/
│   └── slides.pdf
├── images/
│   └── dashboard.png
├── requirements.txt
└── README.md
```

---

## ⚙️ How to Run

**1. Clone the repository**
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

**2. Install Python dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the analysis notebook**
```bash
jupyter notebook notebooks/eda_and_cleaning.ipynb
```

**4. Set up the database**
- Create a database in PostgreSQL, MySQL, or SQL Server
- Import `data/cleaned/cleaned_data.csv` into a table
- Run the queries in `sql/queries.sql`

**5. Open the dashboard**
- Open `dashboard/dashboard.pbix` in **Power BI Desktop**
- Update the data source path if prompted, then click **Refresh**

---

## 👤 Author

**[Your Name]**
Data Analyst | Python • SQL • Power BI

📧 your.email@example.com
🔗 [LinkedIn](https://linkedin.com/in/your-profile) | 💻 [GitHub](https://github.com/your-username)

---

⭐ *If you found this project helpful, please consider giving it a star!*
