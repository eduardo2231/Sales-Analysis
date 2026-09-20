# Sales Analysis

## Overview

This repository includes the notebook `SalesAnalysis.ipynb`, which performs an exploratory analysis of a retail sales dataset. The objective is to identify relevant sales patterns, profitability drivers, customer behavior, and payment preferences through clear visual analysis.

## File Scope

- `SalesAnalysis.ipynb`: main notebook for the sales analysis
- `assets/Sales Dataset.csv`: source dataset used in the notebook

## Analysis Objectives

The notebook is structured around the following business questions:

1. Which sub-categories sell the most within each product category?
2. Which states generate the highest total profit?
3. How do sales evolve over time?
4. Which customers purchase the most and generate the highest profit?
5. Which payment method is used most frequently?

## Dataset Summary

The dataset contains **1,194 rows** and the following fields:

- `Order ID`
- `Amount`
- `Profit`
- `Quantity`
- `Category`
- `Sub-Category`
- `PaymentMode`
- `Order Date`
- `CustomerName`
- `State`
- `City`
- `Year-Month`

## Tools and Libraries

The analysis uses the following Python libraries:

- `pandas`
- `matplotlib`
- `seaborn`
- `numpy`

## Methodology

The notebook follows a direct exploratory workflow:

1. Import the required libraries.
2. Load the sales dataset.
3. Adjust date-related fields to datetime format.
4. Aggregate and visualize information by category, state, time, customer, and payment method.
5. Interpret the results through charts and summary tables.

## Visual Outputs

The notebook generates charts such as:

- Pie charts for sales distribution by sub-category and payment method
- Horizontal bar chart for profit by state
- Line chart for sales volume over time
- Bar charts for customer purchase volume and generated profit

## Execution

To run the notebook locally:

1. Open `SalesAnalysis.ipynb` in Jupyter Notebook or VS Code.
2. Ensure the dataset is accessible from the notebook environment.
3. Install the required libraries if necessary:

```bash
pip install pandas matplotlib seaborn numpy
```

## Important Note

The notebook currently loads the dataset using:

```python
pd.read_csv("Sales Dataset.csv")
```

If the file is executed from the project root, the dataset path may need to be updated to:

```python
pd.read_csv("assets/Sales Dataset.csv")
```

## Conclusion

This notebook provides a concise and structured view of sales performance, customer activity, profitability by region, and payment behavior. It is suitable as an introductory business intelligence exercise and as a foundation for more advanced data analysis projects.
