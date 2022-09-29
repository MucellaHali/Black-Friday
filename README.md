# Black-Friday
# Black-Friday

# Project Introduction
Black Friday is an informal name for the Friday following Thanksgiving Day in the United States. The day after Thanksgiving has been regarded as the beginning of the United States Christmas shopping season since 1952. Many stores offer highly promoted sales on Black Friday. The major challenge for a Retail store or eCommerce business is to choose product price such that they get maximum profit at the end of the sales. Our project deals with determining the product prices based on the historical retail store sales data. After generating the predictions, our model will help the retail store to decide the price of the products to earn more profits.
# Dataset Description
Dataset has 550068 rows (transactions) and 12 columns (features) as described below:

   - **User_ID**: Identity Number of a User. There are a total of 5891 users in the dataset.
   - **Product_ID**: Identity Number of a Product. There are a total of 3623 products in the dataset.
   - **Gender**: Gender of User (M/F).
   - **Age**: Age of the User (in bins).
   - **Occupation**: Occupation Number, already labeled with numbers 0 to 20.
   - **City_Category**: City of a User. Cities are categorized into 3 different categories 'A', 'B' and 'C'.
   - **Stay_In_Current_City_Years**: Number of Years the User has Stayed in their City.
   - **Marital_Status**: is 0 if the user is not married and 1 otherwise.
   - **Product_Category_1 to_3**: Category of the product. All 3 are already labaled with numbers.
   - **Purchase**: Purchase amount.(Target variable)  

Our model will be predicting the purchase amount of the products.

# EDA
Findings;
  -  People of Age group 51-55 have purchased with high amount per person (9600 dollars per person).
  -  40% of total people visited were between Age 26-45.
  -  People from Age group 26-35 collectively have spent more amount.
  -  P00265242 was the product which attratcted most of the adults and P00255842 attracted 0-17 Age group.
  -  Unmarreid Male who are 45% in the dataset have spent 9453 dollars per person.
  -  Even though less no of customers are of Ocuupation 12,15,17 the spend more rougly 9800 dollars per person.
  -  Highest No of customers are from Occupation 0,4 and 7.
  -  High no of customers are of newly settled people but customers who are 2 years residents have spent 9320 dollars per person.
  -  Product P00025442 has got highest total sale amount of about 27.9 million but it is not the highest repeated product in sale P00265242 was highest repeated with 1880 times(1880 customers have bought this).
  -  75% of the number of purchases are made by Male users and rest of the 25% is done by female users. 
  -  People of City of C have purchased with high amount per person (9719 dollars per person)
  -  42% of the number of purchases are made by living in City B users.

# Data Preparation
  - Filled the missing values in the Product_Category_2 and Product_Category_3
  - Used LabelEncoder for encoding the categorical columns Marital_Status,Gender,Age,City_Category and Stay_In_Current_City_Years
# Modeling Phase
  - Splitted dataset into into random train and test subset of ratio 70:30
  - Implemented multiple supervised models.These are Linear Regressor, Ridge, Lasso, ElasticNet, Decision Tree Regressor, Random Forest Regressor and XGBoost.
# Evaluation Metric
Root Mean Square Error (RMSE) is a standard way to measure the error of a model in predicting quantitative data. It’s the square root of the average of squared differences between prediction and actual observation.
# Conclusion
Implanted multiple supervised models such as Linear Regressor,Decision Tree Regressor, Random Forest Regressor and XGBOOST Regressor. Out of these supervised models, based on the RMSE scores XGBRegressor/XGBOOST Regressor was the best performer with a score of 2982.


