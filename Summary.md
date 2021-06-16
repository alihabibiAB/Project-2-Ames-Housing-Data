Project 2 - Ames Housing Data and Kaggle Challenge
==================================================

Objective:
==========

The Ames Housing dataset is a detailed dataset provided for data
analysis. This data set has 80 columns. Each column describes one
feature of houses. In this project, the price of house at sale should be
predicted using three regression models. These models work based on the
linear least square function.

Models used in this project:

1.  Linear Regression
2.  Ridge
3.  Lasso

Workflow of the project
=======================

-   Importing dataset.
-   Cleaning dataset.
-   Feature engineering
-   Modelling with data.
-   Evaluating models.
-   Predicting the sale price
-   Conclusions

Cleaning the trainig dataset
============================

-   Columns with more than 1000 null cells are deleted (Pool QC','Misc
    Feature','Alley','Fence','Fireplace Qu’).
-   Columns are divided into numerical and categorical columns.
-   Null cells in numerical columns are replaced with median or mean
    values of those columns.
-   Null cells in categorical columns are replaced with most common
    feature in those columns.
-   Significant categorical columns are dummified to be considered as
    features.
-   Columns are added to the feature list when absolute value of Pearson
    coefficient is greater than 0.3.

Model preparation and evaluation
================================

Linear regression, ridge, and lasso are used.\
R squared values for linear regression, lasso, and ridge models based on
cross validation process are 0.818, 0.805, and 0.806, respectively. R
squared values for linear regression, lasso, and ridge models for
training set are 0.843, 0.838, and 0.839, respectively. R squared values
for linear regression, lasso, and ridge models for test set are 0.884,
0.881, and 0.885, respectively. All these model underfit the data sets
and need to be revised.

Significant parameters
======================

significant parameters are evaluted based on statmodel (when P is less
than 0.05) and plotting coefficients. Among all parameters, Lot Frontage
has the highest coefficient value among all coefficients.

Conclusions
===========

-   All three models can successfully fit the sale price for Ames House
    datasets.

-   Linear regression has the highest R squared Among models for train
    and test section.

-   Statmodel library is used to determine the significant parameters on
    the sale price.


