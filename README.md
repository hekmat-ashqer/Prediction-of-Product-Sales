# Prediction of Product Sales

by Hikmat Ashqar

## Analyzing Product Categories & Sales Performance in Retail
In the dynamic landscape of retail sales, understanding the intricate relationships between products, their placement in outlets, and the resulting sales figures is paramount. The 'Prediction_of_Product_Sales' project is tailored to unravel these complexities and offer actionable insights into what drives sales in a retail environment

### Data Source:
Big Mart Sales Prediction
https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/
For this dataset, there were 8523 rows and 12 columns.

### Data Dictionary
<img width="297" alt="Data Dictionary" src="https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/e17e2556-d17b-4969-b580-cc6286974132">

## Project 1 - Parts 1 & 2

## To prepare this data, the data was cleaned, and the following processes were performed:

## Exploratory Data Analysis

- During the exploratory data analysis, a boxplot and histogram was visualized for each numeric datatype column. 
- Also, a barplot was visualized for each categorical column. 
- This gave a good baseline for all of the numeric and categorical columns for univariate EDA.

![Distribution of Sales of the product](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/45f53f40-d6b6-426e-b1cb-33e09b7b72ef)

The histogram illustrates how the sales are distributed across different ranges, showing us that most of the product sales are concentrated within the lower range of the scale, indicating that a large number of products have lower sales figures




## Explanatory Visuals

Bar Chart of Average Sales by Outlet Type
![Bar Chart of Average Sales by Outlet Type](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/0654a1f4-8eb8-414f-8003-8636124d0b7b)

 This bar chart show that supermarkets tend to have higher average sales per item compared to grocery stores, indicating that outlet type is a strong predictor of sales.


Scatter Plot of Item Visibility versus Item Sales

![Scatter Plot of Item Visibility versus Item Sales](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/e40dbf37-0699-474a-b759-055bc7c2b4f1)

The scatter plot suggests a nuanced relationship between item visibility and sales; despite a cluster of products with lower visibility achieving varied sales figures, there is not a clear linear trend to indicate that increased visibility straightforwardly leads to higher sales. This could imply that factors beyond visibility play significant roles in determining sales outcomes.
