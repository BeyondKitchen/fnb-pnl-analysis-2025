# 📊 2025 F&B P&L Analysis — Data Cleaning, KPI Reconstruction, and Operational Insights

This project analyzes the **2025 Food & Beverage Profit & Loss (P&L)** performance for a hospitality operation.  
The original financial export contained hidden rows, formulas, mixed data types, and non-numeric formatting.  
To build an analysis-ready dataset, I cleaned the file and reconstructed all major KPIs using Python.

This notebook demonstrates my ability to:

- Clean and standardize raw financial datasets  
- Rebuild operational KPIs using business logic  
- Validate calculated totals against the original report  
- Visualize revenue, cost, labor, and profitability trends  
- Deliver actionable insights relevant to operations and management  

---

## 🧭 Project Objectives

1. Convert a raw P&L export into a structured and reliable dataset  
2. Rebuild core F&B financial metrics:
   - Total Revenues  
   - Total COGS  
   - Salaries & Benefits  
   - Promotional Allowances  
   - Marketing & Sales  
   - Professional Fees  
   - Property & Administration  
   - Total Operating Expenses  
   - Total Departmental Expenses  
3. Validate reconstructed totals vs. the original report  
4. Visualize month-over-month trends for decision-making  
5. Create a scalable framework for future P&L periods  

---

## 🧹 1. Data Cleaning Process

The raw spreadsheet contained:

- Hidden non-F&B rows  
- Broken formulas  
- Commas, dashes (“–”), and blank values  
- Mixed numeric and string formats  

### Cleaning steps performed:

- Extracted visible F&B account rows  
- Removed formulas (values only)  
- Stripped whitespace and formatting  
- Converted all month columns to float  
- Standardized missing or invalid values  
- Renamed months to consistent `Jan-25`, `Feb-25`, ... format  

---

## 🧮 2. Business Logic for KPI Reconstruction

All totals were rebuilt manually from the cleaned account-level rows:

### **🔹 Total Revenues**
```
Food Sales
+ Non-Alcoholic Bev. Sales
+ Liquor Sales
+ Beer Sales
+ Wine Sales
+ Retail Sales
+ Tobacco Sales
+ Other Revenue
+ Revenue Complimentary
```

### **🔹 Total COGS**
```
Food Cost
+ Non-alcoholic Beverage Cost
+ Liquor Cost
+ Beer Cost
+ Wine Cost
+ F&B Rebates
+ Spillage / Waste
+ Papergoods
+ Tobacco
```

### **🔹 Salaries & Benefits, Total**
```
Salaries
Overtime
Statutory Holiday Worked
Vacation
Statutory Holiday
Bonus
Union Backpay Accrual
Employer Health Tax Expense
Extended Health Insurance Expense
Workers Compensation
Employer Match - Pension
Employer Match - RRSP
CPP Expense
EI Expense
Misc. Emp Benefits
```

### **🔹 Promotional Allowances, Total**
```
Food Promo Discounts
Employee Comps - Meals and Entertain (Internal)
```

### **🔹 Marketing & Sales, Total**
```
Complimentary Amenities
Player Comps - Meals - HL - Contra
```

### **🔹 Professional Fees, Total**
```
Fees
Research & Development
```

### **🔹 Property & Administration, Total**
```
Licenses & Permits
Equipment Rental
Cleaning Supplies
Replacements Supplies - China/Glass/Ctlry
Paper & Plastic Disposables Supplies
Supplies
Laundry & Dry Cleaning
Telephone
Dues & Subscriptions
Repairs & Maintenance
Bank Charges
Cash (Overages)/Shortages
```

### 🔹 **Total Operating Expenses**
```
Promotional Allowances, Total
+ Marketing & Sales, Total
+ Professional Fees, Total
+ Property & Administration, Total
```

### 🔹 **Total Departmental Expenses**
```
Total Operating Expenses
+ Salaries & Benefits, Total
```

---

## ✔️ 3. Validation

A full comparison table verifies:

- All reconstructed totals match the original report  
- Differences are **0.0** for every KPI  
- Confirms accuracy of the cleaning + logic pipeline  

---

## 📈 4. Visualizations Included

- Department Profit (2025) — line chart  
- Monthly Profit Margin %  
- Optional charts (Revenue vs COGS, Labor %, etc.)

Helps identify variance trends and operational patterns.

---

## 🛠 Tools Used

- **Python:** Pandas, NumPy  
- **Visualization:** Matplotlib  
- **Environment:** Google Colab  
- **Version Control:** GitHub  

---

## 📁 Repository Structure
```
/
│── F&B_PnL_Analysis__2025_Actuals.ipynb   # main analysis notebook
│── fnb_pnl_actuals_clean_2025.csv         # cleaned dataset
│── README.md
└── .gitignore
```

---

## ▶️ Open in Google Colab
Run the notebook instantly:

👉 https://colab.research.google.com/github/BeyondKitchen/fnb-pnl-analysis-2025/blob/main/F%26B_PnL_Analysis__2025_Actuals.ipynb

---

## 📬 Contact  
If you'd like to explore additional metrics, forecasting, or variance analysis, feel free to reach out.

---

