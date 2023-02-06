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


### Before data modeling, the data was cleaned, and the following processes were performed:


### Exploratory Data Analysis
- This histogram shows the frequency distribution of the Item Fat Content.  

![image](https://user-images.githubusercontent.com/74616874/216893168-1b8e8740-da89-46a7-aa77-dbdf2b8ecb4e.png)

Item Category or Product Category (Food, Drink, Non-Consumable)
- There are more food categories that has been sold than other product categories. 

![image](https://user-images.githubusercontent.com/74616874/216893892-e5d2996a-4b85-47ab-b964-a053fd276715.png)


Item Type: Different types of products
- Even from this graph, the food dominates than the drinks. 'Food and Vegetables' and 'Snack Foods' had the most. 

![image](https://user-images.githubusercontent.com/74616874/216894271-67f099a8-fc99-4939-a3b2-6c995fcc744f.png)


Outlet Type: Different types of supermarket outlets
- Looking at the graph, the supermarket type 1 has a lot of count. 

![image](https://user-images.githubusercontent.com/74616874/216894757-aa8cb43f-2e0d-4323-a7b4-229a906cd1aa.png)



Scatter Plot: Correlation Coefficient
![image](https://user-images.githubusercontent.com/74616874/216895650-8c19b281-39df-4cdf-8250-3041cd243e9b.png)

### Models Evaluated & Results
       
Linear Regression Test Scores:
MAE: 803.6604 
MSE: 1,192,130.7291 
RMSE: 1,091.8474 
R2: 0.5679

Decision Tree Regressor Testing Model (Max_Depth = 9)
MAE: 783.5367 
MSE: 1,270,111.0932 
RMSE: 1,126.9921 
R2: 0.5396

Tuned Decision Tree Regressor Testing Model (Max_Depth = 5)
MAE: 738.0686 
MSE: 1,115,223.9035 
RMSE: 1,056.0416 
R2: 0.5958


- The Final Model chosen was a Decision Regression Tree Model with the max_depth tuned to 5. 
- The Mean Absolute Error was off by about $738.10
- The Mean Squared Error was $1,115,223.90
- The Root Mean Squared Error had a calculation of 1,056.0416

We can use this model to predict sales for the various stores.  
