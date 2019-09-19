# Housing Price Prediction
**[Johnny Yiu](https://github.com/johnnyyiu)**

<a href="https://www.kaggle.com/c/house-prices-advanced-regression-techniques"><img src="https://i.imgur.com/C0qJ5Kv.jpg" title="
House Prices: Advanced Regression Techniques" /></a>

## Goal
The goal is to predict the sales price for each house. With 79 explanatory variables describing almost every aspect of residential homes in Ames, Iowa, we hope to accurately predict the sales price with creative feature engineering and advanced regression techniques.

## Data
The Ames Housing dataset was compiled by [Dean De Cock](http://jse.amstat.org/v19n3/decock.pdf), which is an alternative to the often cited Boston Housing dataset. 

## Model
We evaluate the performance of 9 different models (lasso, elasticnet, ridge, svr, gradient boosting, random forest, xgboost, lightgbm, catboost regressors) by their Root-Mean-Squared-Error (RMSE) using a 10-fold cross validation. We then trained a meta StackingCVRegressor with 8 of the models (excluding random forest) and optimized using lasso. The final prediction will be an ensembled predictions from the models to prevent overfitting. Our final score is an good RMSE of 0.11525.

## Inspiration
* [Comprehensive data exploration with Python](https://www.kaggle.com/pmarcelino/comprehensive-data-exploration-with-python)

* [How I made top 0.3% on a Kaggle competition](https://www.kaggle.com/lavanyashukla01/how-i-made-top-0-3-on-a-kaggle-competition)

* [#1 House Prices Solution [top 1%]](https://www.kaggle.com/jesucristo/1-house-prices-solution-top-1)
