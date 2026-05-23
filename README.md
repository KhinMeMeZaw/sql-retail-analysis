# Retail Sales Business Analysis using SQL

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightblue?logo=sqlite)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow?logo=googlecolab)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> **Portfolio Project — SQL Business Analysis**  
> **Author:** Khin Me Me Zaw | [LinkedIn](https://www.linkedin.com/in/khin-me-me-zaw-a8356317b/) | [GitHub](https://github.com/KhinMeMeZaw)

---

## Project Overview

This project demonstrates a full **SQL-based business analysis workflow** using real-world retail transaction data. It answers 10 meaningful business questions using SQL queries — covering revenue, product performance, customer behavior, and segmentation — all within a Google Colab environment using Python and SQLite.

The project reflects the kind of analysis a data analyst would perform for a retail or e-commerce business to support data-driven decision making.

---

##  Business Questions Answered

| # | Question | Insight Type |
|---|---|---|
| 1 | What is total revenue by country (Top 10)? | Revenue Analysis |
| 2 | Which are the top 10 best-selling products? | Product Performance |
| 3 | What is the monthly revenue trend? | Time Series |
| 4 | Which customers generate the most revenue? | Customer Analysis |
| 5 | What is the average order value per country? | Market Analysis |
| 6 | Which products have the highest cancellation rate? | Quality / Returns |
| 7 | What are the peak sales hours of the day? | Behavioral Analysis |
| 8 | Which month has the lowest sales? | Seasonality |
| 9 | How many unique customers per country? | Market Reach |
| 10 | Who are the most valuable customers? (RFM) | Customer Segmentation |

---

##  Sample Visualizations

| Chart | Description |
|---|---|
| `q1_revenue_by_country.png` | Horizontal bar chart — Top 10 countries by revenue |
| `q2_top_products.png` | Bar chart — Top 10 products by revenue |
| `q3_monthly_trend.png` | Line chart — Monthly revenue trend with fill |
| `q7_peak_hours.png` | Bar chart — Orders by hour of day |
| `q10_rfm_segments.png` | Bar chart — Customer count per RFM segment |

> Screenshots of charts are saved in the `/results` folder.

---

##  Project Structure

```
sql-retail-analysis/
│
├── notebooks/
│   └── SQL_Business_Analysis_Colab.ipynb   # Main analysis notebook
├── results/
│   ├── q1_revenue_by_country.png
│   ├── q2_top_products.png
│   ├── q3_monthly_trend.png
│   ├── q7_peak_hours.png
│   └── q10_rfm_segments.png
└── README.md
```

---

## Dataset

**Online Retail Dataset**
- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
- Records: ~541,000 transactions
- Period: December 2010 – December 2011
- Content: Invoice number, product description, quantity, price, customer ID, country

> The dataset is downloaded automatically inside the notebook — no manual download needed.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.10 | Main programming language |
| SQLite (in-memory) | SQL query execution |
| Pandas | Data loading, cleaning, transformation |
| Matplotlib | Chart generation |
| Google Colab | Development environment |

---

## How to Run

### Option 1 — Google Colab (Recommended)
1. Open [Google Colab](https://colab.research.google.com/)
2. Click **File → Upload Notebook**
3. Upload `SQL_Business_Analysis_Colab.ipynb`
4. Click **Runtime → Run All**
5. All queries and charts will execute automatically

### Option 2 — Local Jupyter Notebook
```bash
# Clone the repo
git clone https://github.com/KhinMeMeZaw/sql-retail-analysis.git
cd sql-retail-analysis

# Install dependencies
pip install pandas matplotlib seaborn openpyxl

# Launch Jupyter
jupyter notebook notebooks/SQL_Business_Analysis_Colab.ipynb
```

---

##  Key Business Insights

- **UK dominates revenue** — accounts for ~85% of total sales; international markets are underdeveloped
- **Top 10 products drive majority of revenue** — classic Pareto (80/20) pattern observed
- **November–December are peak months** — holiday season drives a sharp sales spike
- **Orders peak between 10am–12pm** — optimal window for email marketing and promotions
- **RFM segmentation** identifies 5 actionable customer groups: Champions, Loyal Customers, Potential Loyalists, At Risk, and Lost
- **Some products have high cancellation rates** — signals potential quality or fulfillment issues worth investigating

---

##  SQL Skills Demonstrated

- `GROUP BY` with aggregation (`SUM`, `COUNT`, `AVG`, `ROUND`)
- `ORDER BY` + `LIMIT` for ranking
- `HAVING` clause for post-aggregation filtering
- `CASE WHEN` for conditional logic (cancellation rate)
- `strftime()` for date/time extraction
- `julianday()` for date difference calculation (RFM recency)
- `NULLIF()` to handle division by zero safely
- `COUNT(DISTINCT ...)` for unique value counting
- Subqueries and derived metrics
- Python + SQLite integration via `pd.read_sql_query()`

---

##  About the Author

**Khin Me Me Zaw**
- MSc Digital Transformation Technology, Mae Fah Luang University (2024–Present)
- B.C.Sc Business Information Systems, University of Information Technology (2014–2019)
- Google Data Analytics & Google AI Essentials Certified
- 3+ years experience in data analysis and business development

📧 kmezaw1998@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/khin-me-me-zaw-a8356317b/) | [GitHub Profile](https://github.com/KhinMeMeZaw) | [ML Thesis Project](https://github.com/KhinMeMeZaw/client-potential-prediction-XAI)

---

*Part of my data analyst portfolio. See also: [Client Potential Prediction using ML & XAI](https://github.com/KhinMeMeZaw/client-potential-prediction-XAI)*
