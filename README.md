# ENIAC – Sales & Discount Strategy Analysis

**Data Analytics Portfolio Project | Python | Pandas | Data Cleaning | Business Analysis | Data Visualization**

## Project Overview

This project analyzes historical sales data from ENIAC, an online electronics retailer specializing primarily in Apple products.

The main objective was to evaluate the effectiveness of the company's discount strategy and determine whether offering discounts across the entire product range is a sustainable business approach.

The analysis focuses on sales performance, discount distribution, product categories, price structures, and seasonal trends.

The final goal is to develop data-driven recommendations for a more targeted discount strategy.

## Business Questions

The project addresses the following key questions:

- What proportion of products are sold at a discount?
- What is the average discount percentage compared to the reference product price?
- How are discounts distributed across different product categories?
- Which products and categories generate the highest sales revenue?
- How do seasonal patterns and special shopping events influence sales?
- How does the average discount develop over time?
- How can products be classified into meaningful categories to simplify reporting and business analysis?
- What pricing patterns can be observed across product categories?
- How can the existing discount strategy be improved?

## Dataset

The analysis uses three original datasets:

| Dataset | Description |
|---|---|
| Orders | Order information, dates, payment amounts and order status |
| Orderlines | Individual products included in each order, quantities and selling prices |
| Products | Product information, descriptions, reference prices and product types |

The datasets were combined using order IDs and product SKUs.

**Data period:** January 2017 – March 14, 2018.

## Project Structure

```text
ENIAC-Sales-Discount-Analysis/
│
├── README.md
├── ENIAC_Analysis.ipynb
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── raw/
│   └── processed/
│
├── presentation/
│   ├── ENIAC_Presentation.pdf
│   └── ENIAC_Presentation.pptx
│
└── images/
    ├── sales_overview.png
    ├── discount_analysis.png
    └── category_analysis.png
```

## Methodology

### 1. Data Exploration

Initial exploration of the three datasets using Python and Pandas.

- Dataset structure and dimensions
- Column types and data formats
- Missing values
- Duplicate records
- Initial statistical summaries

### 2. Data Cleaning

The datasets were prepared for further analysis.

- Identification and removal of duplicate records
- Handling missing values
- Correction of date formats
- Identification of corrupted price entries
- Conversion of price columns into numeric values
- Review of order statuses
- Removal of incomplete or inconsistent records where necessary

### 3. Data Integration

The three datasets were merged into one analytical dataset.

- Orders and Orderlines were joined using order IDs.
- Product information was added using product SKUs.
- Orders with missing product information were reviewed and excluded where necessary.

### 4. Data Quality Analysis

Additional checks were performed to evaluate the consistency of order and payment information.

The difference between total order payments and product line payments was analyzed to identify possible shipping charges and unusual values.

### 5. Sales Analysis

Sales performance was evaluated over the available historical period.

- Monthly and quarterly sales development
- Revenue distribution by order status
- Identification of high-performing products
- Analysis of order values
- Identification of unusual sales patterns

### 6. Product Categorization

A custom Python function was developed to classify products based on product names and descriptions.

The resulting categories include:

- iPhone
- iPad
- Apple Devices
- Mac Computers
- Storage
- Memory
- Monitors
- Audio
- Electronic Accessories
- Cases & Protection
- Computer Accessories
- Networking
- Tools & Repair
- Other

This classification simplifies product reporting and allows more structured comparisons between product groups.

### 7. Discount Analysis

Discounts were calculated by comparing the reference product price with the actual selling price.

The analysis includes:

- Discount percentage calculation
- Average and median discount
- Distribution of discount levels
- Comparison across order statuses
- Discount analysis by month
- Comparison of reference prices and selling prices

### 8. Seasonality Analysis

Monthly sales trends were analyzed to identify periods of increased and decreased business activity.

Special attention was given to:

- Black Friday in November
- Christmas shopping in December
- January sales activity
- The weaker period from February to April
- Summer sales in July
- Back-to-School and Back-to-Work demand in August

### 9. Data Visualization

Python visualizations were created to communicate the analytical findings.

The visual analysis includes:

- Monthly revenue trends
- Sales by order status
- Product and category comparisons
- Discount distribution
- Reference price versus actual selling price
- Average order value over time

## Key Findings

The following figures are reported in the project presentation and analytical notebook. They should be interpreted in the context of the selected dataset and calculation method.

- Approximately 7.9 million in total revenue is reported in the presentation.
- The fourth quarter of 2017 is identified as the strongest quarter, with approximately 3 million in revenue.
- The presentation reports that approximately 93% of products were discounted.
- The analytical notebook calculates an average discount of approximately 20.4% across 98,594 product records.
- The product classification resulted in 14 categories.
- iPhone and Storage are among the strongest categories in terms of product revenue.

## Business Recommendations

The analysis supports a more selective and seasonal discount strategy rather than continuous discounts across the entire product range.

The proposed recommendations are:

1. **Targeted seasonal discounts** – focus discount campaigns on selected products during periods of high demand.
2. **Protect Apple hardware pricing** – avoid unnecessary discounts on core hardware products.
3. **Accessory bundles** – offer discounted accessories together with selected devices.
4. **Black Friday campaigns** – reserve larger discounts for specific promotional periods.
5. **Customer loyalty** – introduce loyalty incentives, newsletter vouchers and purchase-based benefits.
6. **Customer service** – strengthen customer relationships through personalized service.

The overall recommendation is to use discounts strategically, considering product category, seasonality and customer demand.

## Tools & Technologies

- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Business Analysis

## Project Files

### Analysis

[Open the complete Python analysis notebook](ENIAC_Analysis.ipynb)

### Presentation

- [View the project presentation (PDF)](presentation/ENIAC_Presentation.pdf)
- [Open the editable PowerPoint presentation](presentation/ENIAC_Presentation.pptx)

### Data

Original datasets are not included in this repository unless redistribution is authorized.

When available, the expected input files are:

- `data/raw/orders.csv`
- `data/raw/orderlines.csv`
- `data/raw/products.csv`

## Limitations

The analysis is based on historical data from January 2017 to March 14, 2018.

The reference product price is not verified as the actual purchase cost of the product. Therefore, the calculated price differences and discounts should not be interpreted as actual profit or profit margin.

Seasonal patterns are observations from the available historical period and do not independently establish causation.

## Conclusion

This project demonstrates how raw transactional data can be transformed into structured business insights.

By combining data cleaning, data integration, product classification, discount analysis, seasonal analysis and visualization, the project provides a foundation for more informed pricing and promotional decisions.

**The key business recommendation: fewer, more targeted and seasonally planned discounts instead of permanent discounts across the entire product range.**

---

**Project:** ENIAC – Sales & Discount Strategy Analysis  
**Created as part of:** Data Analytics & AI Weiterbildung  
**Team:** Majestic PyLots  
**Date:** November 2026
