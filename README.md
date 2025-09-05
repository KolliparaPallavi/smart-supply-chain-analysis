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
<th> Variable </th>	<th> Type	</th> <th> Description </th>
Order State	Character	Australian state of the order<br>
Product Price	Numeric	Price of individual product
Product Name	Character	Name of the product
Order Item Discount	Numeric	Discount applied per order item
Order Item Quantity	Numeric	Quantity ordered
Order Item Total	Numeric	Total cost per order item
Benefit per Order	Numeric	Profit/benefit per order
Delivery Status	Factor	Delivery outcome (On time, Late, etc.)
Shipping Mode	Character	Mode of shipping used
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
