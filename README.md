# Sales Prediction Analysis

## Overview
This project aims to predict sales using two different machine learning models: Linear Regression and Decision Tree. The analysis involves evaluating the performance of each model and comparing their predictive capabilities.


### Data:
Data Science Big Market Sales Prediction: https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets
Sales data for 1559 products across 10 stores in different cities

### **Data Dictionary:**

**Attribute** | **Description**  
--- | ---
Item_Identifer | Unique product id
Item_Weight | Weight of Product
Item_Fat_Content | Whether the product is low fat or regular 
Item_Visibility  | Percentage of total display area of all products in a store allocated in the particlar product
Item_Type | The cateogry to which the product belongs
Item_MRP | Maximum Retail Price of the product
Outlet_Identifier | Unique store id
Outlet_Establishment_Year | The year in whch store was established
Outlet_Size | The size of the store in terms of ground area covered
Outlet_location_type | The type of area in which the storoe is located
Outlet_Type | Whether the outlet is a grocery store or some sort of supermarket
Item_Outlet_Sales | Sales of the product in the particular store. This is the target variable to be predicted. 

## Exploratory Data Analysis
- This histogram shows the frequency distribution of the Item Fat Content.
  
<img width="409" alt="Screen Shot 2024-03-06 at 1 15 05 PM" src="https://github.com/rimchristian/sales-prediction/assets/74616874/28da7dc4-342e-491f-91b9-bc1974bd6688">

Item Type: Different types of products
- Even from this graph, the food dominates than the drinks. 'Food and Vegetables' and 'Snack Foods' had the most. 

<img width="519" alt="Screen Shot 2024-03-06 at 1 16 18 PM" src="https://github.com/rimchristian/sales-prediction/assets/74616874/b048d184-85b8-4705-a1fb-8684dfaba963">


Outlet Type: Different types of supermarket outlets
- Looking at the graph, the supermarket type 1 has a lot of count.
  
<img width="665" alt="Screen Shot 2024-03-06 at 1 16 46 PM" src="https://github.com/rimchristian/sales-prediction/assets/74616874/7d11383f-c85d-46ed-bcc6-df386f639e9b">


## Results Interpretation
### Linear Regression Model:
- **Training Scores:**
  - \(R^2\): 0.5606
  - MAE: 848.9872
  - MSE: 1,300,271.1535
  - RMSE: 1,140.2943

- **Test Scores:**
  - \(R^2\): 0.5658
  - MAE: 808.0322
  - MSE: 1,197,957.7117
  - RMSE: 1,094.5125
    
### Decision Tree Model:

- **Training Scores:**
  - \(R^2\): 0.6039
  - MAE: 762.6551
  - MSE: 1,172,151.6518
  - RMSE: 1,082.6595

- **Test Scores:**
  - \(R^2\): 0.5947
  - MAE: 738.6501
  - MSE: 1,118,238.0927
  - RMSE: 1,057.4678


### Key Findings:

- The Decision Tree model outperformed the Linear Regression model across all evaluation metrics.
- Decision Tree model demonstrated better generalization performance, indicating its suitability for real-world sales prediction.
- Both models showed moderate predictive power with \(R^2\) scores ranging from 0.5606 to 0.6039.

### Implications and Alignment with Objectives:

- Model Selection: Decision Tree model is recommended for predicting sales due to its superior performance.
- Generalization Performance: Decision Tree model's ability to generalize well to unseen data is advantageous for accurate sales predictions.
- Model Improvement: Further optimization of hyperparameters or exploration of ensemble methods could enhance the Decision Tree model's predictive performance.
- Business Insights: Insights derived from these models can aid businesses in optimizing inventory management and making data-driven strategic decisions.

## Conclusion

This analysis provides valuable insights into sales prediction modeling, enabling businesses to make informed decisions and maximize revenue and profitability.
