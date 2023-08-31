# Prediction-of-Product-Sales
## Analyzing Sales Data for Food Items Sold at Various Stores

**Author**: Ismaa-eel Hendricks

### Business problem:

The purpose of this analysis is to help the retailers understand the properties of products and outlets that play crucial roles in increasing sales in their stores.


### Data:
Data Source: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

For this dataset, there were 8523 rows and 12 columns.

## Methods
### Data Dictionary



## To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis
For the exploratory data analysis, the following was conducted:

    - Histograms to view the distributions of numerical features
    - Boxplots to view statistical summaries of numerical features
    - Countplots to view the frequency of each class of categorical features
    - Heatmap to view the correlation between features

#### Maximum Retail Price ($)
![image](https://github.com/FiyonaK/Prediction-of-Product-Sales/assets/138833676/e434c63f-cf63-4bfe-ab70-b68bf5c63f4c)

This histogram shows that the majority of items have a maximum retail price of between $100 and $200 with a slight dip just under the $150 mark.

#### Explanatory Data Analysis
For the explanatory data analysis, the following was conducted:

    - Categorical features were plotted against the target feature using a combination of a seaborn barplot and stripplot to visualize the spread of data
    - Numerical features were visualized against the target feature using a seaborn regplot

#### Outlet Size vs Outlet Sales
![image](https://github.com/FiyonaK/Prediction-of-Product-Sales/assets/138833676/16a1bb76-4adf-4d79-9c06-2e158bcdb2b3)

According to the above visual, the average sales seem to be highest in the medium sized stores.

### Outlet Type vs Outlet Sales
![image](https://github.com/FiyonaK/Prediction-of-Product-Sales/assets/138833676/c56b0090-a9db-4ffb-b17d-b21b61f501a6)

This visual shows Supermarket Type 3 has the highest average number of sales than the rest of the categories.


## Machine Learning Models:

The following models were used:

    Linear Regression Model
    Random Forest Regressor Model
    Tuned Random Forest Regressor Model

## Models Evaluated & Results

- Linear Regression Model (Testing Set):
    - MAE = 805.312
    - MSE = 1,197,758.824
    - RMSE = 1,094.422
    - R^2 = 0.566
 - Random Forest Regressor Model (Testing Set)
    - MAE = 808.704
    - MSE = 1,348,429.998
    - RMSE = 1,161.219
    - R^2 = 0.511 
 - Tuned Random Forest Regressor Model (Testing Set):
    - MAE = 733.329
    - MSE = 1,105,544.306
    - RMSE = 1,051.449
    - R^2 = 0.599

 - The final model chosen was the Random Forest Regressor Model with the following tuned parameters:
   
       - max_depth = 10
       - min_samples_leaf = 30
       - n_estimators = 350
  - For the chosen model, the Mean Absolute Error was off by about $733.33
  - The Mean Squared Error was $1,105,544.31
  - The Root Mean Squared Error had a calculation of $1,051.45
  - The model can explain 60% of the variation in the target

    Even though this was the best performing model of the two, I would not consider it very reliable in making accurate predictions on our target, due to the low R^2 score and high MSE.

## Recommendations:

There are many factors that can influence a feature like "Sales" in a retail establishment.
Our analysis has shown that the majority of features analysed here have a direct influence on the sales per outlet, from types of products sold, item visibility within the store to outlet size and type. The maximum retail price also has an influence on the sales numbers.
This information could be very useful to store owners in how they price their items, how efficiently the stores are laid out, as well as the types and categories of items sold in each store to assist in increasing sales.


## Limitations & Next Steps

With the unfavourable metric scores and low confidence in the ability of the model to make accurate predictions, I would recommend meeting with the stakeholders to understand what data to add/remove in order achieve a better working dataset as a base for better predictive modeling.


### For further information


For any additional questions, please contact:
  - Ismaa-eel Hendricks
  - Ihendricks.studies2023@gmail.com
