# Vrinda Store Annual Sales Analysis Dashboard (2022)

An interactive Excel dashboard that analyzes one year of order data for **Vrinda Store**, an Indian online fashion retailer selling across multiple e-commerce marketplaces. The dashboard turns ~31,000 raw orders into clear answers about *who buys, where they buy, when they buy and through which channel* so the business can target its sales and marketing better.

---

## Business Objective

Identify the customer segments, regions and sales channels that contribute most to revenue, and recommend how to improve sales in the following year.

## Dataset

| Item | Detail |
|---|---|
| Source file | `Vrinda Store Data Analysis dashboard.xlsx` |
| Period | January to December 2022 |
| Volume | 31,047 orders (all statuses) |
| Total sales | ₹2.12 crore (₹21,176,377) |
| Currency | INR |

**Columns:** Order ID, Cust ID, Gender, Age, Age Group, Date, Month, Status, Channel, SKU, Category, Size, Qty, Currency, Amount, Ship-city, Ship-state, Ship-postal-code, Ship-country, B2B

**Workbook structure**
- `Data`: cleaned order-level data
- `Work`: pivot tables behind each chart
- `Dashboard`: final one-page visual report with insights and conclusion

## Data Preparation

- Removed duplicates and checked for blanks/inconsistent entries
- Standardized text fields (for example gender labels, state and city names, and quantity values stored as text such as "One" vs 1)
- Created an **Age Group** column (Teenager / Adult / Senior Citizen) from customer age
- Extracted **Month** from the order date for trend analysis
- Built pivot tables on the cleaned data and linked them to charts on the dashboard

## Dashboard Views

1. **Sales vs Orders:** monthly sales amount and order count
2. **Men vs Women:** share of sales by gender
3. **Order Status:** Delivered, Returned, Cancelled, Refunded
4. **Top 5 States:** states by sales amount
5. **Orders by Age and Gender:** age-group split for men and women
6. **Sales Channels:** order share by marketplace

## Key Findings

**Overall**
- Total sales of **₹21.18M** across **31,047 orders** (average order value about ₹682)
- **92.2%** of orders were delivered; cancellations, returns and refunds together were **7.8%**

**Customers**
- **Women drive ~64% of revenue** (₹13.56M vs ₹7.61M for men) and ~69% of orders
- Adults are the largest age group at about **76%** of orders (women adults alone: 52.4%)

**Geography**
- Top 5 states by sales: **Maharashtra (₹2.99M), Karnataka (₹2.65M), Uttar Pradesh (₹2.10M), Telangana (₹1.71M), Tamil Nadu (₹1.68M)**
- The top 3 states contribute about **37%** of sales and the top 5 about **53%**

**Channels**
- **Amazon (35.5%), Myntra (23.4%) and Flipkart (21.6%)** together account for about **80%** of orders
- Ajio 6.2%, Nalli 4.8%, Meesho 4.5%, Others 4.1%

**Trend**
- Sales peaked in **March (₹1.93M)** and declined through the year to a low of about **₹1.62M in November** (roughly 16% below the March peak)

## Recommendations

- **Target women customers (adult age group) in Maharashtra, Karnataka and Uttar Pradesh** with ads, offers and coupons
- **Focus promotions on Amazon, Myntra and Flipkart**, which bring ~80% of orders
- **Counter the second-half sales decline** with seasonal and festival campaigns
- **Reduce returns/cancellations** (~8% of orders) by improving size guides and product descriptions
- Grow the lower-performing segments (men, teenagers, smaller channels) with targeted offers

## Tools & Skills Used

- **Microsoft Excel:** data cleaning, formulas, pivot tables, pivot charts, dashboard design
- Data analysis, data visualization, business insight generation

## How to Use

1. Download the `.xlsx` file and open it in Microsoft Excel
2. Go to the **Dashboard** sheet for the final report
3. Open the **Work** sheet to see the pivot tables behind each chart
4. Open the **Data** sheet to explore the cleaned source data

## Author

**Khushal Dusane**: Aspiring Data Analyst | SQL · Python · Power BI · Excel
