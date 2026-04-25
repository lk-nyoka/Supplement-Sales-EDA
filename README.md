# 💊 Supplement Sales — EDA, Visualisation & SQL Analysis (2020–2025)

An end-to-end data analysis project on weekly supplement sales data
covering EDA, storytelling visualisation, and SQL business analysis.
Built as part of my Data Science learning journey.

---

## 📌 Project Overview

This project analyses 4,384 rows of weekly supplement sales data spanning
January 2020 to April 2025. It covers three phases — exploratory data
analysis, dedicated visualisation storytelling, and SQL business queries
using SQLite inside a Jupyter notebook.

**Business Goal:** Understand what drives revenue in supplement sales
and identify opportunities to increase profit.

**Key Questions Answered:**
1. Which categories and products generate the most revenue?
2. How do discounts affect sales and profit?
3. Which platform performs best?
4. Are returns affecting profits?
5. How does revenue change over time?
6. Which location generates the most units sold?
7. Which platform and location combo generates the most revenue?
8. What is the return rate per platform?
9. What are the top 3 products per category by revenue?
10. What is net revenue per platform after accounting for returns?

---

## 📂 Dataset & Resources

- **Dataset:** [Supplement Sales Data 2020–2025](https://www.kaggle.com/datasets/zahidmughal2343/supplement-sales-data)
- **Tutorial:** [Python Data Analysis Project — Supplement Sales](https://www.youtube.com/watch?v=hv-GFdGlKTw&list=PLTsu3dft3CWjDYJuybziwD-iqTcsrHHxN&index=2)

---

## 🛠️ What Was Done

**EDA**
- Loaded and inspected the dataset using `.info()`, `.head()`, `.describe()`
- Converted DATE column to datetime and extracted Month and Year
- Analysed distributions of Units Sold, Revenue, and Discount
- Plotted category and platform performance using Seaborn bar charts
- Built an interactive Revenue over Time chart by Category using Plotly
- Created monthly trend charts for Revenue and Units Sold using subplots
- Engineered a Net Revenue column accounting for returns and discounts
- Compared Net Revenue across platforms — Amazon, Walmart, iHerb
- Compared Net Revenue across locations — USA, UK, Canada
- Calculated correlation heatmap across numeric variables

**Visualisation**
- Built a dedicated storytelling notebook answering 5 business questions
- Each chart paired with a business insight and recommended decision
- Identified top performing products — Biotin and Zinc in Vitamins and Minerals
- Found iHerb as the strongest performing platform
- Discovered limited benefit from discounting on revenue
- Identified seasonal revenue spikes for promotion planning

**SQL Analysis**
- Loaded cleaned dataset into SQLite database using Python
- Answered 10 business questions using pure SQL
- Used GROUP BY, HAVING, ORDER BY, LIMIT, CAST and window functions
- Calculated return rate per platform using CAST for float division
- Used RANK() OVER PARTITION BY to find top 3 products per category

---

## 📊 Key Business Insights

- Biotin and Zinc from Vitamins and Minerals are the highest revenue drivers
- iHerb outperforms Amazon and Walmart on Net Revenue
- Discounts show limited impact on overall revenue
- Revenue shows consistent growth with seasonal spikes — promotions should align with peak months
- Returns have a measurable impact on net profitability
- Amazon has the highest return rate at 1.04% vs Walmart at 1.00%

---

## 🧰 Tools & Libraries

- Python 3
- Pandas
- Matplotlib
- Seaborn
- Plotly
- SQLite3
- Jupyter Notebook

---

## 📁 File Structure
supplement-sales-eda/
│
├── Notebook.ipynb              # EDA notebook
├── visualisation.ipynb         # Storytelling visualisation notebook
├── analysis.ipynb              # SQL business analysis notebook
├── supplement_sales.db         # SQLite database
├── data/
│   └── supplement_sales.csv    # Raw dataset
└── README.md                   # Project documentation

---

## 💡 Key Learnings

- Starting with a business goal transforms analysis from exploration to decision making
- Each chart should answer a specific question — not just display data
- Net Revenue must account for discounts on returned items — not just full price
- SQLite uses double quotes for column names with spaces — not backticks
- CAST() is required for float division in SQLite
- RANK() OVER (PARTITION BY) finds top N per group — a window function

---

## 👤 Author

**Lindokuhle Nyoka**
[GitHub](https://github.com/lk-nyoka) · [LinkedIn](https://linkedin.com/in/lindokuhle-nyoka-982019245)