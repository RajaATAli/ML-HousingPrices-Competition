# Housing Prices Competition for Kaggle Learn Users

## Overview
This comptetion revolves around the real estate market, where various factors contribute to the price negotiations of residential homes, beyond the commonly considered features like the number of bedrooms or the aesthetics of a white-picket fence.

## Dataset
The dataset comprises 79 explanatory variables describing almost every aspect of residential homes in Ames, Iowa. The challenge is to utilize these variables to predict the final price of each home. The dataset files include:
- `train.csv` - the training set
- `test.csv` - the test set
- `data_description.txt` - full description of each column, lightly edited to match the column names used in this competition
- `sample_submission.csv` - a benchmark submission from a linear regression model

Some key data fields include the property's sale price, area, type and quality of various home features, year built, and more.

## Skills
- Creative feature engineering 
- Employing advanced regression techniques like random forest and gradient boosting

## Evaluation
### Goal
The objective is to predict the sales price for each house in the test set. The predictions should be made for the `SalePrice` variable against each `Id` in the test set.

### Metric
Submissions will be evaluated based on the Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the logarithm of the observed sales price, ensuring equal weighting in error assessment across different price ranges.

### Submission File Format
The submission file should contain a header and have the following format:

```
Id,SalePrice
1461,169000.1
1462,187724.1233
1463,175221
...
```