# -Retail_Sales_Predication_ML
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. My work includes various plots and graphs , visualizations , feature engineering , ensemble techniques , different ML algorithms with their respective parameter tuning , analysis and trends .

The goal is to predict the Sales of a given store on a given day.

The dataset consists of two csv files: store and Rosmann Data

Data Files:

Rosmann Data holds info about each store. store.csv holds the sales info per day for each store.

Business Problem. Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

Steps for solving the business problem:

a) Collecting Data- That will involved upload the .csv file, thoroughly check the independent and dependent variable by using .head() , .info() , .describe() etc.

b) Preparing the Data- Cleaning the data to remove unwanted data, missing values, rows, and columns, duplicate values, data type conversion, etc. Visualize the data to understand how it is structured and understand the relationship between independent variables and dependent variable. Splitting the cleaned data into two sets - a training set and a testing set. The training set is used to teach the model to recognize patterns and relationships in the data and to optimize its parameters to minimize the error on the training set. A testing set is used to check the accuracy of model after training.

c) Choosing and training the model. d) Hyparameter Tuning. e) Making Predictions.

Conclusion We saw that Sales column contains 172817 rows with 0 sale. So we created a new dataframe in which we removed 0 sales rows and tried to train our model. We used various algorithms and got accuracy score around 74%.

We were also curious about the total dataset(including Sales = 0 rows). So we trained another model using various algorithms and we got accuracy near about 98% which is far better than previous model.

So we came to conclusion that removing sales=0 rows actually removes lot of information from dataset as it has 172817 rows which is quite large and therefore we decided not to remove those values.We got our best rmpse score from Random Forest model,Graident boosting technique like adaboost ,Xgboost,we tried taking an optimum parameter so that our model doesnt overfit.

