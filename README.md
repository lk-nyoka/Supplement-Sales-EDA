# 💊 Supplement Sales EDA (2020–2025)

An exploratory data analysis project on weekly supplement sales data
across multiple platforms and locations. Built as part of my Data Science
learning journey.

---

## 📌 Project Overview

This project analyses 4,384 rows of weekly supplement sales data spanning
January 2020 to April 2025. The analysis covers sales trends, platform
performance, category revenue, discount impact, and return rates across
the USA, UK, and Canada.

---

## 📂 Dataset & Resources

- **Dataset:** [Supplement Sales Data 2020–2025](https://www.kaggle.com/datasets/zahidmughal2343/supplement-sales-data)
- **Tutorial:** [Python Data Analysis Project — Supplement Sales](https://www.youtube.com/watch?v=hv-GFdGlKTw&list=PLTsu3dft3CWjDYJuybziwD-iqTcsrHHxN&index=2)

---

## 🛠️ What Was Done

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

---

## 🧰 Tools & Libraries

- Python 3
- Pandas
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook

---

## 📁 File Structure
supplement-sales-eda/
│
├── Notebook.ipynb              # Main EDA notebook
├── data/
│   └── supplement_sales.csv    # Raw dataset
└── README.md                   # Project documentation

---

## 💡 Key Learnings

- Plotly produces interactive charts that communicate trends better than static plots
- Net Revenue must account for discounts on returned items — not just full price
- Time series grouping with `.dt.to_period("M")` simplifies monthly aggregations
- Subplots with `sharex=True` make multi-metric trend comparisons cleaner

---

## 👤 Author

**Lindokuhle Nyoka**
[GitHub](https://github.com/lk-nyoka) · [LinkedIn](https://linkedin.com/in/lindokuhle-nyoka-982019245)
