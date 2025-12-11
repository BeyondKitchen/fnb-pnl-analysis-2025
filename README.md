# 📊 2025 F&B P&L Analysis — Data Cleaning, KPI Reconstruction & Insights

This project analyzes the **2025 Food & Beverage Profit & Loss (P&L)** performance for a hospitality operation.  
The raw P&L export included hidden rows, merged formatting, and inconsistent numeric structures.  
Using Python, I cleaned the dataset and reconstructed all major KPIs for a fully analysis-ready workflow.

---

## 🎯 Project Objectives
- Convert a raw P&L export into a structured and reliable dataset  
- Rebuild core F&B financial metrics:
  - Total Revenues  
  - Total COGS  
  - Salaries & Benefits  
  - Promotional Allowances  
  - Marketing & Sales  
  - Professional Fees  
  - Property & Administration  
  - Total Operating Expenses  
  - Total Departmental Profit  
- Validate calculated values against the original report  
- Visualize revenue, cost, labor, and profit trends  
- Provide insights applicable to real F&B operational decision-making  

---

## 🧹 Data Cleaning Overview
- Removed hidden/merged header rows  
- Standardized numeric and text formats  
- Split combined category labels into structured columns  
- Converted text-based numbers into numeric types  
- Ensured clean category hierarchy for analysis  
- Output a fully validated and structured dataset  

---

## 🧮 KPI Reconstruction
Rebuilt using industry logic:

- COGS % of Revenue  
- Labor Cost % of Revenue  
- Operating Profit %  
- Promotions Impact  
- Departmental Profit Margin  
- Month-over-Month Trend Metrics  

All KPI totals were cross-validated against the raw report.

---

## 📈 Visualizations Included
- Monthly Department Profit (Line Chart)  
- Monthly Profit Margin %  
- Revenue / COGS / Labor Trend Lines  
- Optional variance and anomaly detection visuals  

---

## 🛠 Tools Used
- **Python:** Pandas, NumPy  
- **Visualization:** Matplotlib  
- **Environment:** Google Colab  
- **Version Control:** GitHub  

---

## 📂 Project Structure
fnb-pnl-analysis-2025/
│
├── data/
│ ├── raw/
│ │ └── fnb_pnl_2025_raw.csv
│ ├── processed/
│ │ └── fnb_pnl_actuals_clean_2025.csv
│
├── F&B_PnL_Analysis_2025_Actuals.ipynb
├── README.md
└── .gitignore

---

## 📊 Dataset Description

### **Raw Data (`/data/raw/`)**
`fnb_pnl_2025_raw.csv`  
Unclean file exported from the P&L system with formatting issues, merged headers, and inconsistent numerics.

### **Processed Data (`/data/processed/`)**
`fnb_pnl_actuals_clean_2025.csv`  
Cleaned, structured dataset ready for:
- BI dashboards  
- Profitability modeling  
- Forecasting  
- Operations review  

---

## ▶️ Open in Google Colab
Run the full notebook here:

👉 https://colab.research.google.com/github/BeyondKitchen/fnb-pnl-analysis-2025/blob/main/F%26B_PnL_Analysis_2025_Actuals.ipynb

---

## 📬 Contact
If you'd like additional KPIs, forecasting models, or operational insights, feel free to reach out.
