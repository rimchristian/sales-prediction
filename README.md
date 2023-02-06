# Sales Predictions for Big Mart Outlets

## **Aim is to build a predictive model and predict the sales of each product at a particular outlet.**

### Data:
Data Science Big Market Sales Prediction: https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets
Sales data for 1559 products across 10 stores in different cities

### Methods:
- Load the Data
- Inspect the Data
- Clean the Data
- Data Preprocessing
-   ColumnSelector
-   ColumnTransformer
- Data Modeling
- Linear Regresssion Model
-   R-Squared
-   Root Mean Squared Error
- Regression Tree Model
-   R-Squared
-   Root Mean Squared Error
- Model Comparison

### Results 
- Create a default model
- High Bias Version and High Variance Version 
- Create best version of the model

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
