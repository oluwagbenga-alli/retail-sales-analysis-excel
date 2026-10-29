# Retail Sales Analysis & Dashboard (Excel)

## Project Overview

This project analyses the Sample Superstore retail dataset using Microsoft Excel. The goal was to understand which product categories, sub-categories, regions and time periods contribute most to sales and profit, and identify areas that may require further investigation.

I used Excel to inspect data quality, create PivotTables, analyse performance patterns, and build an interactive-style visual dashboard using charts and KPI cards.

## Business Questions

- Which product category has the highest sales and profit?
- Which regions perform best and worst in terms of sales and profit?
- How do sales and profit vary across months?
- Which product sub-categories generate the highest and lowest profits?
- Do higher average discount rates appear alongside lower profits in any sub-categories?

## Dataset

- **Dataset:** Sample Superstore
- **Source:** Tableau Sample Data
- **Dataset link:** https://public.tableau.com/app/learn/sample-data?qt-overview_resources=1
- **File format:** Excel workbook
- **Sheet analysed:** Orders

The dataset contains fictional retail transaction data, including order and shipping dates, product categories, regional information, sales, quantities, discounts and profits.

The People and Returns sheets were not included in this analysis.

## Tools and Excel Features

- Microsoft Excel
- Data inspection and cleaning checks
- Column filters
- Find & Select → Go To Special → Blanks
- Remove Duplicates
- PivotTables
- Clustered bar and column charts
- Number and percentage formatting
- KPI cards and dashboard layout

## Methodology

### 1. Data Acquisition and File Management

I accessed Tableau's Sample Data page, located the Sample Superstore dataset and downloaded the Excel workbook.

I saved the file in a folder on my Mac named `Retail Sales Analysis`. I preserved the original workbook and worked on a separate copy to avoid modifying the source file.

### 2. Data Inspection

Before making changes, I reviewed the column headings and inspected the Orders sheet to assess data quality.

The checks focused on:

- Missing or blank cells
- Duplicate records
- Date and numeric data types
- Unusual or unexpected values
- Potentially incomplete postal codes

### 3. Data Cleaning and Quality Checks

**Missing values:** I selected the dataset and used Excel's Go To Special feature to locate blank cells. Excel returned “No cells were found,” indicating that no blank cells were detected by this check.

**Duplicate records:** I used Excel's Remove Duplicates feature and reviewed the selected columns. Excel reported that no duplicate values were found.

**Data types:** I checked that Order Date and Ship Date were recognised as dates, while Sales, Profit, Quantity and Discount were stored in appropriate numeric formats.

**Unusual values:** I used column filters to inspect values that might require further investigation, including unexpected text in numeric fields and negative or unusually large values.

**Postal code observation:** Some postal code entries contained only three characters, including examples such as `M7A`, `B3H` and `H1A`. I flagged these as potentially incomplete but retained the original values because their correct forms could not be verified. Postal codes were not required for the planned sales and profit analysis.

No other data changes were documented at this stage.

### 4. PivotTable Analysis

I created PivotTables to summarise the data and compare performance across several dimensions.

| PivotTable | Purpose |
|---|---|
| Sales by Category | Compare sales across Furniture, Office Supplies and Technology |
| Profit by Category | Compare profitability across the three product categories |
| Sales by Region | Identify regional sales differences |
| Profit by Region | Compare regional profitability |
| Monthly Sales and Profit | Examine performance throughout the year |
| Profit and Average Discount by Sub-Category | Investigate differences in sub-category profitability and discount rates |

These summaries formed the basis of the charts and dashboard.

### 5. Data Visualisation

I created charts from the PivotTable results to make the comparisons easier to interpret.

The visualisations included:

- Sales by Category
- Profit by Category
- Monthly Sales Trend
- Monthly Profit Trend
- Sales by Region
- Profit by Region
- Average Discount by Sub-Category
- Profit by Sub-Category

I used separate charts for monthly sales and monthly profit because the two measures have different numerical scales. Horizontal bar charts helped compare sub-categories and made negative profit values easier to identify.

### 6. Dashboard Development

I assembled the charts into an Excel dashboard titled **Retail Sales Dashboard**.

The dashboard includes four KPI cards:

- **Total Sales:** 2,326,534
- **Total Profit:** 292,297
- **Top Sales Category:** Technology
- **Top Sales Region:** West

I applied a consistent blue colour scheme and arranged the KPI cards and charts into a single dashboard view. The aim was to present the main performance indicators alongside the detailed comparisons.

## Dashboard Preview

The dashboard brings together category performance, monthly trends, regional comparisons and sub-category analysis.

*To display the dashboard screenshot here, save an image of your completed dashboard in the repository as `images/retail-sales-dashboard.png`, then add the following Markdown:*

`![Retail Sales Dashboard](images/retail-sales-dashboard.png)`

## Key Findings

The PivotTable analysis produced the following findings.

### Category Performance

- **Technology** recorded the highest sales, at approximately 839,893, and the highest profit, at approximately 146,543.
- Furniture recorded approximately 754,748 in sales and 19,730 in profit.
- Office Supplies recorded approximately 731,893 in sales and 126,023 in profit.

### Regional Performance

- **The West region** recorded the highest sales, at approximately 739,814, and the highest profit, at approximately 110,799.
- The South region recorded the lowest sales, at approximately 391,722, and the lowest profit, at approximately 46,749.

### Monthly Performance

- **December** recorded the highest monthly sales and profit, at approximately 330,218 and 44,230, respectively.
- Monthly summaries showed variations in both sales and profit throughout the year.

### Sub-Category Profitability

- **Copiers** recorded the highest sub-category profit, at approximately 56,094.
- **Tables** recorded a negative profit of approximately 17,753.
- **Bookcases** also recorded a negative profit of approximately 3,632.

### Discount and Profitability

- **Binders** had the highest average discount rate, at approximately 36.91%, while still generating positive profit of approximately 31,426.
- Machines had an average discount rate of approximately 30.43% and generated positive profit of approximately 3,462.
- Tables had an average discount rate of approximately 25.81% and recorded a negative profit of approximately 17,753.

These results suggest that discount rates and profitability vary across sub-categories. However, average discount alone does not explain whether a sub-category is profitable or loss-making.

## Recommendations

Based on the findings, the following areas warrant further investigation:

1. **Investigate Tables and Bookcases:** Examine product-level sales, discounts, costs and transaction patterns to understand their negative profits.
2. **Review high-discount sub-categories:** Investigate Binders and Machines to understand how their discounting patterns relate to profit.
3. **Examine regional differences:** Explore why the West performs strongly and why the South records lower sales and profit.
4. **Review monthly performance:** Investigate the factors associated with stronger sales and profit in December.
5. **Explore category opportunities:** Examine the performance of Technology and Office Supplies to understand which products and transactions contribute most to profitability.

These are proposed areas for further analysis, not conclusions about the causes of performance differences.

## Limitations

- The dataset is fictional sample retail data and does not represent an actual company's financial performance.
- The analysis focused on the Orders sheet; the People and Returns sheets were excluded.
- Postal code entries flagged as potentially incomplete were retained because their correct values could not be verified.
- The analysis describes patterns in the data and does not establish causation.
- The discount investigation compared average discount rates with total profit by sub-category. It did not isolate the effect of discounts or test statistical significance.
- The dashboard uses rounded figures for readability.

## Conclusion

This project demonstrates how Microsoft Excel can be used to inspect data quality, summarise retail transactions, compare sales and profitability, investigate discount patterns and build a visual dashboard.

PivotTables helped structure the analysis, while charts and KPI cards made the findings easier to communicate. The results highlighted Technology and the West region as leading performers and identified Tables and Bookcases as sub-categories requiring further investigation.

The project represents a practical application of Excel for exploratory data analysis and business performance reporting.

## Skills Demonstrated

- Data inspection and quality assessment
- Data summarisation using PivotTables
- Sales and profit analysis
- Data visualisation
- KPI selection and dashboard design
- Interpretation of business performance patterns
- Communicating findings and analytical limitations
