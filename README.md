# Machine Learning Assignment
coursera John Hopkins - October 2017

- Data from http://web.archive.org/web/20161224072740/http:/groupware.les.inf.puc-rio.br/har
- Predicting "class" (factor variable A to E) which denotes how the excercise is performed from metrics
- Includes exploratory analysis and combining predictors with PCA
- Final model used is a Random Forest in caret

# Executive Summary

## Results
- Initial pml-training.csv data was randomly partitioned 60%/20%/20% into Training, Testing & Validation for Cross Validation
- Out of Sample Error was X% on Testing and Y% on Validation

## Pre- Processing
- Reduced the columns from 160 to 59 by removing those which had greater than 20% missing values
- Best fit model was found using unstandardised data and removing some variables that were highly correlated with others
- Also tried standardising (centre & scale) and PCA to compress predictors but this actually gave lower Accuracy in the model
