# Phase 2 Project


## Project Overview

This project analyzes 2014-2015 the King County house sales data for a local real estate agency that helps potential homeowners to sell their homes. The analysis will follow Cross-Industry Standard Process for Data Mining (CRISP-DM). Based on the validated model and exploratory analysis, the real estate agency will provide useful advice to their clients about what factors determine the sale price.


### The Data

This project uses the King County House Sales dataset, which can be found in  `kc_house_data.csv` in the data folder in this repo. The description of the column names can be found in `column_names.md` in the same folder. As with most real world data sets, the column names are not perfectly described, so you'll have to do some research or use your best judgment if you have questions about what the data means.

It is up to you to decide what data from this dataset to use and how to use it. If you are feeling overwhelmed or behind, we recommend you ignore some or all of the following features:

* date
* view
* sqft_above
* sqft_basement
* yr_renovated
* zipcode
* lat
* long
* sqft_living15
* sqft_lot15


### Business Problem

Local real estate agents usually face such questions from their clients as: whether home renovations increase the value of houses, and by what amount; whether a view of waterfront increases the house sale price; and etc.

Upon analyzing the King County house sales data, we will help local real estate angency to answer the questions from their clients, i.e. homeowners. We will help figure out what are the key features that determine the sale price of houses, and by what amount.


## Deliverables

There are three deliverables for this project:

* A **GitHub repository**
* A **Jupyter Notebook**
* A **non-technical presentation**


## Methodology

* Check missing values and convert datatypes

* Check Four Assumptions associated with a Linear Regression Model：

Before modeling, we will check the linearity and multicollinearity here.
At the same time, we will investigate the the relationship between our target: price and the predictors by data visualization. We will also remove outliers from the skewed data.

* One-Hot Encoding on Categorical Data

* Modeling:

1. Split Data into Training and Test Sets
2. Build Models with OLS results
3. Check Normality and Homoscedasticity Assumptions
4. Validate Each Model by Calculating RMSE

* Models:

1. Baseline Model
2. Model 1: remove uninfluential features by stepwise selection with p-values
3. Model 2: scale the predictors based on Baseline Model


## Summary

### Results

![Module Results Comparison Table](https://github.com/carlearn/dsc-phase-2-project/blob/main/images/Module%20Results%20Comparison%20Table.png)

![Relationship](https://github.com/carlearn/dsc-phase-2-project/blob/main/images/Relationship.png)


### Conclusion
The top features to determine the value of houses are:
1. Grade: overall grade given to the housing unit, based on King County grading system
2. Square footage of the house and its nearest 15 neighbors
3. Square footage of lot and its nearest 15 neighbors
4. Waterfront: whether the house has a view to a waterfront

### Next Step
1. More sales data:
2. Further analysis on age of the house
3. Further analysis on renovation
4. Analyze the zipcode/location feature
