# Diwali Sales Data Analysis

## Project Overview

This project explores Diwali sales data using Python to understand customer demographics, order patterns, and sales performance. The analysis uses data cleaning, descriptive statistics, grouping, aggregation, and visualizations to examine gender, age groups, state-wise orders and sales, marital status, occupation, product categories, and frequently recorded product IDs.

## Project Objectives

- Inspect the dataset structure, data types, and summary statistics.
- Identify missing values and prepare the data for analysis.
- Explore the distribution of purchase amounts and handle missing values.
- Compare customer counts and recorded sales across gender and age groups.
- Analyze order counts and sales amounts by state.
- Explore customer distribution by marital status and occupation.
- Compare product-category counts and recorded sales amounts.
- Identify the 10 most frequently recorded Product IDs.

## Dataset

The notebook's saved output shows **11,251 records and 15 original columns**. The dataset includes customer and product identifiers, gender, age group, age, marital status, state, zone, occupation, product category, order count, and purchase amount.

During preparation, the notebook removes the `Status` and `unnamed1` columns because they contain no usable values in the inspected data. It fills 12 missing values in `Amount` with the median value (`8109`) and converts `Amount` to an integer. After removing the two columns, the working DataFrame has 13 columns.

> **Dataset note:** Add the CSV to the repository only if you have permission to redistribute it. Otherwise, document the dataset source and explain how readers can obtain it.

## Tools and Libraries

- **Python** — analysis workflow
- **Pandas** — data loading, cleaning, grouping, and aggregation
- **NumPy** — numerical operations
- **Matplotlib** — visualizations
- **Seaborn** — statistical charts
- **Jupyter Notebook** — interactive analysis

## Analysis Workflow

### 1. Data Loading and Inspection
The notebook loads the CSV into a Pandas DataFrame and examines its dimensions, columns, sample records, data types, missing values, and descriptive statistics.

### 2. Data Cleaning
- Checks missing-value counts and percentages.
- Removes `Status` and `unnamed1`.
- Uses a boxplot to inspect the `Amount` distribution.
- Fills missing `Amount` values with the median.
- Converts `Amount` to an integer type.

### 3. Exploratory Data Analysis (EDA)
- **Gender:** customer counts and total recorded sales by gender.
- **Age group:** customer counts split by gender and total recorded sales by age group.
- **State:** total orders and total recorded sales by state.
- **Marital status:** customer counts by marital status and gender.
- **Occupation:** customer counts by occupation.
- **Product category:** record counts and total recorded sales by category.
- **Product IDs:** the 10 most frequently recorded Product IDs.

## Key Findings from the Notebook

- **Gender:** The saved aggregation reports total recorded sales of **74,416,943 for female customers** and **31,929,494 for male customers**. This compares total sales, not average spending per customer.
- **State-wise performance:** Uttar Pradesh ranks first in the saved results for both total orders (**4,813**) and total recorded sales (**19,391,186**). Maharashtra and Karnataka follow in both measures.
- **Customer segments:** The notebook explores customer counts across age groups, marital status, gender, and occupation.
- **Product analysis:** The notebook compares product-category counts with total recorded sales and charts the 10 most frequently recorded Product IDs.

The exact rankings for age groups, occupations, and product categories should be confirmed from the relevant chart data or group-by tables before reporting specific leaders. Product ID frequency does not necessarily mean highest revenue or profit.

## Business Questions

1. Which gender contributes the most to total recorded sales?
2. Which age groups contribute most to customer activity and recorded sales?
3. Which states have the highest total orders and recorded sales?
4. How are customers distributed by marital status and gender?
5. Which occupations have the highest customer counts?
6. Which product categories have the highest record counts and total recorded sales?
7. Which Product IDs appear most frequently in the dataset?
8. What customer and regional patterns could be explored further for marketing and inventory planning?

## Conclusion

This exploratory analysis uses Python to examine customer characteristics and sales patterns in the Diwali sales dataset. The saved results show higher total recorded sales for female customers than male customers, and identify Uttar Pradesh as the leading state by both total orders and recorded sales. The notebook also explores age groups, marital status, occupations, product categories, and frequently recorded Product IDs.

These findings can help guide further investigation into customer segmentation, regional performance, and product demand. However, customer counts and total sales alone do not prove individual purchasing power, profitability, or the effectiveness of a marketing strategy. Additional analysis would be required to validate those conclusions.

## How to Run

1. Download or clone this repository.
2. Make the dataset CSV available in the project folder, if you are permitted to share it.
3. Open `Diwali_sales_analysis.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
4. Update the notebook's CSV path to match your local setup.
5. Install the required libraries if needed:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

6. Run the notebook cells from top to bottom.

## Repository Structure

```text
Diwali-Sales-Analysis/
├── Diwali_sales_analysis.ipynb
├── README.md
└── Diwali Sales Data.csv   # Include only if redistribution is permitted
```
