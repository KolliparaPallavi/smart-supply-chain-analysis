# smart-supply-chain-analysis
### Overview
This project performs a statistical analysis of the DataCo Smart Supply Chain Dataset with a focus on Australian orders. The goal is to understand factors influencing delivery performance and order financials. Key analyses include descriptive statistics, outlier detection, chi-square tests, and linear regression.
### Project Objectives
Examine the association between shipping modes and delivery status.<br>
Investigate the relationship between Benefit per Order and Order Item Total using linear regression.<br>
Summarize Order Item Total across Australian states and identify trends or outliers.<br>
Perform data cleaning and preprocessing to ensure consistency. 
### Dataset
The dataset is sourced from Kaggle: DataCo Smart Supply Chain Dataset.
### Key Variables:
<table>
  <tr>
    <th>Variable</th><th>Type</th><th>Description</th>
  </tr>
  <tr>
    <td>Order State</td><td>Character</td><td>Australian state of the order</td>
  </tr>
  <tr>
    <td>Product Price</td><td>Numeric</td><td>Price of individual product</td>
  </tr>
  <tr>
    <td>Product Name</td><td>Character</td><td>Name of the product</td>
  </tr>
  <tr>
    <td>Order Item Discount</td><td>Numeric</td><td>Discount applied per order item</td>
  </tr>
  <tr>
    <td>Order Item Quantity</td><td>Numeric</td><td>Quantity ordered</td>
  </tr>
  <tr>
    <td>Order Item Total</td><td>Numeric</td><td>Total cost per order item</td>
  </tr>
  <tr>
    <td>Benefit per Order</td><td>Numeric</td><td>Profit/benefit per order</td>
  </tr>
  <tr>
    <td>Delivery Status</td><td>Factor</td><td>Delivery outcome (On time, Late, etc.)</td>
  </tr>
  <tr>
    <td>Shipping Mode</td><td>Character</td><td>Mode of shipping used</td>
  </tr>
</table>

### Methodology
#### Data Preprocessing:
Filtered dataset to only include Australian orders.<br>
Standardized state names and converted delivery status to an ordered factor.<br>
Selected relevant columns for analysis.<br>
#### Descriptive Statistics & Visualization:
Computed summary statistics of Order Item Total grouped by state.<br>
Visualized data with boxplots and scatterplots to detect trends and outliers.
#### Chi-square Test:
Tested association between Shipping Mode and Delivery Status.
#### Linear Regression:
Explored the relationship between Benefit per Order and Order Item Total.<br>
Checked assumptions: linearity, normality, homoscedasticity, and influential points.
### Key Findings
No significant association between shipping mode and delivery status (Chi-square p = 0.9898). <br>
Positive but weak relationship between benefit per order and total order value (R² = 0.0059). <br>
New South Wales had the highest average sales per customer (~$183.35). <br>
No major outliers detected in Order Item Total across states.
### Tools & Libraries
Language: R <br>
Libraries: dplyr, ggplot2, RColorBrewer, readr
