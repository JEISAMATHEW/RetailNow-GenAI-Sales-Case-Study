# RetailNow – From Messy Data to Business Decisions

Excel Data Cleaning + Generative AI for Business Insights

## 📌 Project Overview

This project simulates a real analyst task: cleaning a messy quarterly sales export from **RetailNow**, a mid-sized online retailer, and using Generative AI as an analysis partner to turn cleaned numbers into a board-ready business insights report.

The project follows an end-to-end workflow:

**Messy Raw Data → Excel Cleaning → Pivot Tables & Charts → GenAI-Assisted Insights → Business Recommendations**

## 🏢 Industry

**Retail / E-commerce**

## 💡 Business Scenario

RetailNow sells Electronics, Apparel, Home & Kitchen, Beauty, Sports, Groceries, Books, and Toys across India. Each quarter's raw order export is entered inconsistently by different regional teams, leaving it full of formatting issues. The CEO needed a clean, fast business insights report ahead of a leadership meeting — using whatever tools necessary, including AI.

## 📊 Dataset

**415 order records, 14 columns**, intentionally messy to mirror a real analyst's raw export.

| Column | Meaning | Known Issue(s) |
|---|---|---|
| Order ID | Unique order identifier | Some IDs repeat (duplicate orders) |
| Order Date | Date the order was placed | At least 5 different date formats, plus blanks |
| Customer Name | Customer full name | Mixed case, extra spaces, initials only, some blank |
| Email | Customer email | Some missing |
| City / Region | Delivery location | Inconsistent casing, typos, extra spaces |
| Product Category | Category of product ordered | Many spelling/casing variants of the same category |
| Product Name | Specific product ordered | Mostly clean |
| Quantity | Units ordered | Text values ("N/A", "two"), a suspicious 9999, negatives, blanks |
| Unit Price | Price per unit | Mixed currency symbols/text, thousands separators, blanks |
| Discount (%) | Discount applied | Mixed number/text/percent format, blanks |
| Payment Method | How the order was paid | Inconsistent casing and abbreviations |
| Order Status | Delivered/Shipped/Cancelled/Returned/Pending | Inconsistent casing |
| Customer Rating (1–5) | Post-purchase rating | Blanks and out-of-range values (0, 6, -1) |

## 🧹 Data Cleaning (Part A)

Performed in Excel using formulas, Text-to-Columns, Find & Replace, Power Query, data validation, and conditional formatting:

* Standardized Order Date into one consistent date format
* Standardized Product Category, Region, Payment Method, and Order Status to a single spelling/casing per value
* Cleaned Customer Name (trimmed extra spaces, consistent capitalization)
* Handled Quantity issues: text values, blanks, and suspicious 9999 entries (flagged/handled with a documented rule)
* Cleaned Unit Price by stripping currency symbols and commas into a pure numeric field
* Standardized Discount (%) into one consistent numeric format
* Identified and handled exact duplicate order rows
* Flagged out-of-range Customer Rating values (kept within 1–5)
* Kept the raw data untouched on a separate sheet for auditability

## 🤖 GenAI-Assisted Analysis (Part B)

Used a GenAI tool as an analysis partner (not for coding) to:

* Get specific Excel formula / Power Query suggestions for cleaning blockers
* Turn pivot table summaries into plain-language business insights
* Critically review first-draft insights and challenge unsupported claims
* Rewrite bullet-point findings into a polished, board-ready executive summary

An appendix of the actual prompts used — and what was kept or changed from each AI response — is included in the case study brief.

## 📈 Analysis Built

**Pivot Tables**
* Total revenue by Product Category and Region
* Order count and average order value by Payment Method
* Order Status distribution by Region
* Average Customer Rating by Product Category

**Dashboard Highlights**
* Total Revenue, Order Count, Discounted Amount, Average Rating, and Average Revenue KPIs
* Revenue by Product Category (bar chart)
* Order Status breakdown (pie chart)
* Average Rating by Product Category (bar chart)
* Total Revenue Over Time (trend line)
* Filters for Product Category, Customer Rating, Region, Payment Method, and Order Status

## 🎯 Business Value

* Identifies top-performing and under-performing categories and regions
* Surfaces patterns in cancellations and returns by region
* Flags whether discounting is driving revenue or eating into margin
* Delivers 3–5 concrete, data-backed recommendations for leadership

## 🛠️ Technology / Tools

* **Microsoft Excel** (formulas, Power Query, PivotTables, conditional formatting)
* Generative AI (prompt-based analysis and report writing)
* Data visualization (bar, pie, and trend charts)
* Git & GitHub for version control

## 🔄 Project Workflow

```text
Raw RetailNow Sales Export (415 orders, 14 columns)
      ↓
Excel Data Cleaning (dates, categories, prices, duplicates, outliers)
      ↓
Pivot Tables & Charts (revenue, payment method, status, ratings)
      ↓
GenAI-Assisted Insight Generation & Critical Review
      ↓
Business Insights Report + Recommendations
```

## 📁 Project Structure

```text
RetailNow-GenAI-Sales-Case-Study/
│
├── Retail_Case_Study.xlsx
├── README.md
├── RetailNow_Case_Study_Brief.pdf
├── Retail_Case_Study_using_GenAI.pptx
├── Gen Al Case Study - Retail_Sales_Dashboard.png
├── Gen Al Case Study - Retail_Sales_Prompt.jpg
├── Gen Al Case Study - Retail_Sales.mp4
└── Gen AI Case Study Dataset's Detailed Error.png

```

## 📌 Project Deliverables

* Cleaned workbook with pivot tables and dashboard views
* 1–2 page Business Insights Report for the CEO
* Appendix of GenAI prompts used, with notes on what was kept or changed
* Video walkthrough of the dashboard and analysis

## 🔗 Connect

**Jeisa Mathew**
[LinkedIn](https://www.linkedin.com/in/jeisamathew/) • [GitHub](https://github.com/JEISAMATHEW)
