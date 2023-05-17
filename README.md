# Credit Risk Classification

## Overview
The purpose of this analysis is to practice training and predicting data using a logistic regression model, as well as getting more experience working with an unbalanced data set.
Part of this analysis is identifying if oversampling the data helps or hinders the overall accuracy of the model.

## Results
### Basic Pipeline
Initially I used the basic pipeline of splitting data to training and predicting with the model. The resulting scores for the healthy loan label (or "0" in this case) were 0.99 precision and 1.00 recall, meaning the model did well with this particular label.
The model did worse with the high-risk laon label (or "1") with a precision score of 0.91 and a recall score of 0.85. This is most likely due to the much smaller data set for this category, resulting in a less well-trained model.
Overall, using this pipeline, the model achieved an accuracy score of 99.18% with a total of 158 data points being incorrectly categorized.

### Oversampling Pipeline
Following the first pipeline, the steps were mostly the same with the addition of oversampling the training data. The resulting scores for the healthy loan label was still the same with 0.99 precision and 1.00 recall, however this time, the precision score for the high-risk loans was higher at 0.99.
On the flip-side, the recall score did go down by 0.01 to 0.84. However, the overall accuracy of the model increased to 99.38% with a total of 120 points being mis-categorized.

## Summary
Overall, this logistic regression model was very accurate with its healthy loan predictions, however due to the smaller dataset for high-risk loans, it is less accurate predicting these. I think this model is usable as long as there are additional failsafes in place regarding loans that were predicted to be high-risk as these make up a smaller portion of predicted values.
