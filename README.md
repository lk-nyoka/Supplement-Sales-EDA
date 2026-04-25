# 💊 Supplement Sales — EDA & Data Visualisation (2020–2025)

An end-to-end data analysis and visualisation project on weekly supplement
sales data across multiple platforms and locations.
Built as part of my Data Science learning journey.

---

## 📌 Project Overview

This project analyses 4,384 rows of weekly supplement sales data spanning
January 2020 to April 2025. It covers two phases — exploratory data
analysis to understand the data, and a dedicated visualisation notebook
that answers specific business questions through storytelling with charts.

**Business Goal:** Understand what drives revenue in supplement sales
and identify opportunities to increase profit.

**Key Questions Answered:**
1. Which categories and products generate the most revenue?
2. How do discounts affect sales and profit?
3. Which platform performs best?
4. Are returns affecting profits?
5. How does revenue change over time?

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

---

## 📊 Key Business Insights

- Biotin and Zinc from Vitamins and Minerals are the highest revenue drivers
- iHerb outperforms Amazon and Walmart on Net Revenue
- Discounts show limited impact on overall revenue
- Revenue shows consistent growth with seasonal spikes — promotions should align with peak months
- Returns have a measurable impact on net profitability

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
├── Notebook.ipynb              # EDA notebook
├── visualisation.ipynb         # Storytelling visualisation notebook
├── data/
│   └── supplement_sales.csv    # Raw dataset
└── README.md                   # Project documentation

---

## 💡 Key Learnings

- Starting with a business goal transforms analysis from exploration to decision making
- Each chart should answer a specific question — not just display data
- Net Revenue must account for discounts on returned items — not just full price
- Time series grouping with `.dt.to_period("M")` simplifies monthly aggregations
- Subplots with `sharex=True` make multi-metric trend comparisons cleaner

---

## 👤 Author

**Lindokuhle Nyoka**
[GitHub](https://github.com/lk-nyoka) · [LinkedIn](https://linkedin.com/in/lindokuhle-nyoka-982019245)