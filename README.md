# 🍪 B&J Biscuit Sales Dashboard

An interactive **Microsoft Excel sales dashboard** for B&J Biscuit that turns 12,000 raw transactions into clear insights on revenue, profit, customers, locations, brands, and payment methods.

![Dashboard Preview](images/dashboard-preview.png)

> The preview above shows the dashboard with the **Chicago** location slicer applied, so its KPI values are for Chicago only. Company-wide totals are in the table below.

---

## 📌 Problem Statement

B&J Biscuit has plenty of sales data, but raw data makes it hard to judge business performance. Management needs one dashboard to monitor sales, find profitable areas, understand customers, and make faster decisions.

## 📊 Key Results (all data, no filters)

| KPI | Value |
|---|---|
| Quantity Sold | 30,50,309 |
| Total COGS | ₹3,47,83,050 |
| Total Revenue | ₹6,15,67,883 |
| Total Profit | ₹2,67,84,833 |
| Profit Margin | 43.5% |
| Period covered | Jan 2024 – Dec 2024 |
| Transactions | 12,000 |

## 🔎 Insights

- **Most profitable brand:** Shortbread (about ₹1.09 Cr profit, ~40% of total profit)
- **Top location by revenue and profit:** San Antonio (11.9% of revenue)
- **Top salesperson:** Travis Doyle
- **Most profitable customer:** Robert Hernandez
- **Best age group:** 60–74 (highest revenue at 24.1% and highest profit)
- **Payment methods:** Revenue is spread almost evenly across Cash, Credit Card, Debit Card and Mobile Payment; Debit Card is slightly ahead (25.4%)

## 🧰 Dashboard Features

- KPI cards: Quantity Sold, COGS, Revenue, Profit, Profit Margin
- "Most profitable" cards: Brand, Location, Customer, Salesperson, Age Group
- Revenue by Age Group, Gender, Payment Method, Product Price Category and Location
- Top 5 Customers by revenue contribution
- Interactive slicers for Payment Type, Location and Age Group
- Toggle between **Absolute Value** and **Percentage** view

## 🗂️ Dataset

| Column | Description |
|---|---|
| Transaction Date | Date of sale |
| Buyer First / Last Name | Customer name |
| Buyer Location | City of purchase |
| Buyer Date of Birth | Used to calculate Age |
| Payment Method | Cash, Credit Card, Debit Card, Mobile Payment |
| Quantity Purchased | Units sold |
| Product Code | Links to brand, cost and unit price (Pro01–Pro10) |
| Sales Representative | Salesperson |
| Gender | Male / Female / Other |

**Calculated columns:** Brand Name, Cost, Unit Price, Age, Age-Group (15-year buckets), Revenue, COGS, Profit, Price Range, Full Name, Week Day, Week Type.

## 🧹 Data Preparation

- Removed duplicate records and corrected missing values
- Standardized date formats and fixed data types
- Created Age Groups and Price Categories
- Added calculated columns for Revenue, COGS, Profit and Profit Margin
- Loaded the cleaned data into the Power Pivot Data Model

## 🛠️ Tools & Techniques

Microsoft Excel · Power Query · Power Pivot / Data Model · PivotTables & PivotCharts · DAX Measures · Slicers · Conditional Formatting

**Excel functions:** `IF`, `SUM`, `SUMIFS`, `COUNTIFS`, `LOOKUP` / `XLOOKUP` / `VLOOKUP`, `INDEX` + `MATCH`, `DATEDIF`, `WEEKDAY`, `FLOOR`, `TEXT`, `YEAR`, `MONTH`

## 📁 Repository Structure

```
bj-biscuit-sales-dashboard/
├── dashboard/
│   └── BJ_Biscuit_Sales_Dashboard.xlsm   # Interactive Excel dashboard
├── presentation/
│   └── BJ_Biscuit_Sales_Dashboard.pdf    # Project presentation
├── images/
│   └── dashboard-preview.png             # Dashboard screenshot
├── README.md
├── LICENSE
└── .gitignore
```

## ▶️ How to Use

1. Download `dashboard/BJ_Biscuit_Sales_Dashboard.xlsm` (click the file → **Download raw file**).
2. Open it in **Microsoft Excel (desktop)**. Slicers and PivotTables need desktop Excel; GitHub and Excel Online won't run them fully.
3. If prompted, click **Enable Editing** and **Enable Content** (the file contains a macro project).
4. Open the **DashBoard** sheet and use the slicers to filter by payment type, location and age group.

## 💼 Business Benefits

- Faster, data-driven decisions
- Spot the most profitable products, locations and salespeople
- Understand customer buying behaviour
- Improve sales and marketing strategy
- Track overall business performance in one view

## 👩‍💻 Author

**T. Gowri**
Connect with me on [LinkedIn](https://www.linkedin.com/) · [GitHub](https://github.com/)

⭐ If you found this project useful, please give it a star!
