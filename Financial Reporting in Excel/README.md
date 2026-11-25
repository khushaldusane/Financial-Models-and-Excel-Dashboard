# Apex Financial Reporting System: FY 2025

An Excel-based **financial reporting and variance analysis model** for a simulated company, *Apex Consumer Products Pvt. Ltd.* (offices in Mumbai, Pune and Bengaluru). It converts transaction-level ledger data into a dynamic monthly P&L, a department performance report, automated data-quality checks and an executive KPI dashboard.


---

## Overview

| Item | Detail |
|---|---|
| Period | January to December 2025 |
| Transactions | 999 ledger rows |
| Budget records | 480 (5 departments × 12 months × 8 accounts) |
| Chart of accounts | Codes 4000 to 6400 mapped to P&L categories |
| Departments | Sales, Operations, Marketing, Finance, Human Resources |
| Locations | Mumbai, Pune, Bengaluru |
| Currency | INR |

## Key Metrics (FY 2025)

| Metric | Value |
|---|---|
| Gross sales revenue | ₹36,478,037 |
| Net revenue (after returns and discounts) | ₹36,114,086 |
| Gross profit | ₹25,907,758 (**71.7%** gross margin) |
| Total operating expenses | ₹7,892,608 |
| Operating profit (EBIT) | ₹18,015,150 (**49.9%** operating margin) |

## Workbook Structure

| Sheet | Purpose |
|---|---|
| **Dashboard** | KPI scorecards, monthly trend table, regional and department contribution, OPEX structure |
| **Income_Statement** | Dynamic monthly P&L driven by Year / Month / Department / Location inputs (multi-criteria `SUMIFS`), showing Actual vs Budget vs Prior Year with variance and YoY % |
| **Department_Performance** | Monthly department P&L: revenue, returns, COGS, OPEX, operating profit, gross margin % and budget revenue variance |
| **Data_Quality** | Audit control panel with 8 automated reconciliation checks |
| **Raw_Data** | Transaction log with formula-driven Month Start, Account Name and Category lookups |
| **Budget** | Monthly department budget targets by account |
| **Accounts** | Chart of Accounts mapping |
| **Validation_Lists** | Source lists for the drop-down controls |

## Features

- **Dynamic P&L:** pick a year, month, department and location in the yellow input cells and the whole statement recalculates
- **Variance analysis:** Actual vs Budget vs Prior Year with favorable/unfavorable flags
- **Department view:** monthly department P&L with gross margin % and budget revenue variance
- **Executive dashboard:** monthly trend of gross sales, net revenue, COGS, OPEX and operating margin, plus regional and department contribution
- **Data-quality controls:** duplicate transaction IDs, unmapped accounts, missing dates, missing departments, negative amounts, unmapped P&L categories, row count and total-value checksum

## Key Insights

**Monthly trend**
- Sales peaked in **October (₹3.81M)** and were lowest in **August (₹2.06M)**
- Sales fell about **31% from July to August**, and operating margin dropped to **25.7%** in August (against 61.3% in October)

**Departments**

| Department | Gross Revenue | Share | Operating Profit | Op. Margin |
|---|---|---|---|---|
| Sales | ₹12.68M | 34.8% | ₹6.78M | 53.4% |
| Marketing | ₹8.93M | 24.5% | ₹5.30M | 59.4% |
| Operations | ₹7.93M | 21.7% | ₹2.97M | 37.4% |
| Human Resources | ₹4.24M | 11.6% | ₹2.51M | 59.1% |
| Finance | ₹2.69M | 7.4% | ₹0.47M | 17.3% |

- Finance has the weakest operating margin (17.3%); Operations is the next lowest (37.4%)

**Regions**
- **Bengaluru** is the largest at ₹13.29M (about 36%), followed by Mumbai (₹11.75M) and Pune (₹11.44M)
- Return rates are low: Mumbai 0.5%, Pune 1.2%, Bengaluru 1.3%

**Cost structure**
- **Salaries & wages** are the biggest OPEX item at ₹4.36M (about 55% of OPEX), then marketing (₹1.38M), logistics (₹0.91M), rent & utilities (₹0.82M) and software & admin (₹0.42M)

## Known Limitations

- The Data_Quality sheet currently **flags duplicate Transaction IDs** (568 of 999 rows); the other 7 controls pass. This is listed as a follow-up item.
- Budget revenue values are much smaller than actuals, so budget variance percentages are very large. Treat budget variance as illustrative.
- Revenue is tagged to all departments (including Finance and HR) because the data is simulated.

## How to Use

1. Download `Apex Fin Reporting 2025.xlsx` and open it in Excel
2. Start on the **Dashboard** for the annual summary
3. Go to **Income_Statement** and change the yellow cells (Year, Month, Department, Location) to generate a P&L for any slice
4. Use **Department_Performance** to compare departments for a chosen month
5. Check **Data_Quality** to review the audit controls

## Tools & Skills

Microsoft Excel: `SUMIFS`, lookup formulas, data validation drop-downs, conditional flags, dashboard design. Financial reporting: P&L structure, chart of accounts, budget vs actual variance, margin analysis.

## Author

**Khushal Dusane (KD)**: Data Analyst | Excel · SQL · Python · Power BI
Mumbai / Pune, India
