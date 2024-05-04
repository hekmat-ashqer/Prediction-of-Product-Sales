
# Sales Impact Analysis of Product Features and Store Characteristics
## Predictive Modeling to Enhance Retail Decisions

**Author**: Hikmat Ashqar

## Analyzing Product Categories & Sales Performance in Retail
In the dynamic landscape of retail sales, understanding the intricate relationships between products, their placement in outlets, and the resulting sales figures is paramount. The 'Prediction_of_Product_Sales' project is tailored to unravel these complexities and offer actionable insights into what drives sales in a retail environment

### Business Problem:
This project focuses on predicting sales of food items sold at various retail outlets. The goal is to assist retailers in understanding how product attributes and store characteristics influence sales volumes, enabling them to optimize marketing and product placement strategies effectively.

### Data:
The dataset comprises several features related to products and stores, such as product type, store size, and location. It includes historical sales data, which serves as the target variable for our predictive modeling.
Big Mart Sales Prediction
https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/
For this dataset, there were 8523 rows and 12 columns.

### Data Dictionary
<img width="297" alt="Data Dictionary" src="https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/e17e2556-d17b-4969-b580-cc6286974132">


## Methods
- **Data Preparation**: We cleaned the dataset to handle missing values, corrected anomalies, and engineered features to improve model performance.
- **Exploratory Data Analysis (EDA)**: Performed to identify significant patterns and relationships that informed the subsequent modeling phase.

- During the exploratory data analysis, a boxplot and histogram was visualized for each numeric datatype column. 
- Also, a barplot was visualized for each categorical column. 
- This gave a good baseline for all of the numeric and categorical columns for univariate EDA.

![Distribution of Sales of the product](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/45f53f40-d6b6-426e-b1cb-33e09b7b72ef)

The histogram illustrates how the sales are distributed across different ranges, showing us that most of the product sales are concentrated within the lower range of the scale, indicating that a large number of products have lower sales figures


## Results

### Sales Trends by Store Type
![Sales Trends by Store Type](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/0654a1f4-8eb8-414f-8003-8636124d0b7b)

> This chart illustrates the distribution of total sales across different store types, providing insights into which store formats achieve higher sales volumes. it show that supermarkets tend to have higher average sales per item compared to grocery stores, indicating that outlet type is a strong predictor of sales.

### Price Elasticity of Products
![Price Elasticity of Products](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/price_elasticity.png)

> This scatter plot demonstrates the relationship between the Maximum Retail Price (MRP) of products and their sales volumes across various outlets. The correlation coefficient r=0.57 indicates a moderate positive correlation, suggesting that as the MRP increases, sales volumes tend to increase as well. This highlights a certain degree of price sensitivity, where higher-priced items still enjoy substantial sales, possibly due to perceived value or brand loyalty.


### Scatter Plot of Item Visibility versus Item Sales

![Scatter Plot of Item Visibility versus Item Sales](https://github.com/hekmat-ashqer/Prediction-of-Product-Sales/assets/12829449/e40dbf37-0699-474a-b759-055bc7c2b4f1)

> The scatter plot suggests a nuanced relationship between item visibility and sales; despite a cluster of products with lower visibility achieving varied sales figures, there is not a clear linear trend to indicate that increased visibility straightforwardly leads to higher sales. This could imply that factors beyond visibility play significant roles in determining sales outcomes.


## Model
### Recommended Model: Tuned Random Forest
Our comprehensive analysis and rigorous tuning process have led us to select the Tuned Random Forest model as the optimal choice for predicting sales of food items across various retail outlets. 

#### Model Evaluation Metrics:
- **Mean Absolute Error (MAE)**: Shows how far the predictions are from the actual results on average.
  - Train: 755.249
  - Test: 728.708
- **Mean Squared Error (MSE)**: Indicates the average squared difference between the estimated values and actual value.
  - Train: 1,152,451.050
  - Test: 1,096,964.685
- **Root Mean Squared Error (RMSE)**: Provides the standard deviation of the residuals, which measure how far from the regression line data points are.
  - Train: 1,073.523
  - Test: 1,047.361
- **R² (R-squared)**: Represents the proportion of the variance for a dependent variable that's explained by an independent variable or variables in a regression model.
  - Test: 0.602

#### Why the Tuned Random Forest Model Rocks:
- **High Prediction Accuracy**: The model exhibits strong performance, particularly in its ability to forecast sales for unseen data, with an RMSE on the test set of approximately 1,047.361. This means our sales predictions could be off by around $1,047 on average, which is robust for our use case.
- **Effective Learning Capability**: With an R² of 0.602 on the test set, the model effectively captures about 60% of the variability in sales data, making it a reliable choice for our predictions.
- **Balanced Learning**: The model has been tuned to prevent overfitting, ensuring it generalizes well on new, unseen data, which is crucial for adapting to varying market conditions and store characteristics.

### Conclusion
Opting for the Tuned Random Forest in our sales prediction project positions us to leverage a model that not only understands our existing data deeply but is also skilled at adapting to new scenarios. This makes it akin to having a sales prediction expert capable of accurately estimating sales outcomes for diverse products and outlets.


## Recommendations:
- **Dynamic Pricing Strategy**: Implement dynamic pricing strategies informed by the model’s insights into price sensitivity, adjusting prices in real-time based on demand and inventory levels.
- **Inventory Optimization**: Use the model's predictions to optimize inventory levels across stores, ensuring high-demand products are adequately stocked in locations where they sell well.

## Limitations & Next Steps
- **Enhanced Feature Engineering**: Although the model performs well, further improvement could be achieved by exploring more sophisticated feature engineering techniques, possibly incorporating external data sources such as weather patterns or economic indicators.
- **Model Deployment and Monitoring**: Deploy the model into a real-time analytics framework to continuously monitor its performance and tweak as necessary to adapt to changing market conditions or consumer behaviors.
