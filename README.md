# UWFinTechModule12: Supervised Learning

## Overview of the Analysis

The purpose of this analysis is to use different machine learning models in order to determine which model will be most efficient in determining risky loans. Due to the high ratio of healthy loans to risky loans, this may be a challenge to machine learning in predicting which case is a risky loan. Within the dataset there are various variables such as loan size, interest rate, debt to income ratio, number of accounts, total dept and status of loan. The machine learning models will take in these variables to understand the traits of these loan in order to know when to classify a loan as a risky loan. In this analysis we will focus on two models, one model using the original dataset and the other using a random oversampling module. The main difference between these two models is that the random oversampling will use many, smaller, random sets within the original dataset to train itself. In theory, because of the low amount of risky loans may not be enough for the model to train and predict accurately, the random oversampling will allow more instances of risky loans to be reiterate in the training model to obtain a better understanding of it. After prepping the data for both models and training it, the performances of these two model will be compared to determine which is more efficient for the purpose of the data. Specifically we will be looking at precision, balance accuracy score, and recall.


## Results


 Machine Learning Model 1:

![LRM_original_data](https://user-images.githubusercontent.com/61864923/196864994-de032bda-1d02-4642-8b51-8aff9fcab382.JPG)

  * Balance accuracy score of 0.95, which is relatively high.
  * In predicting the '0' or healthy loan, the model was 100% accurate with a precision of 1.
  * In predicting the '1' or high-risk loan, this model with a precision of 0.85 shows that it was 85% accurate.
  * It had a recall of 0.91, meaning that it is 91% likely to predict a high-risk loan correctly.





 Machine Learning Model 2:

![RandomOverSampler](https://user-images.githubusercontent.com/61864923/196865001-fc4e3e5c-c3ec-48e9-b95e-dd404399be9a.jpg)

  * Balance accuracy score of 0.99, which is higher than model 1.
  * Model 2 was again 100% accurate or has a precision of 1 in determining the '0' or healthy loans.
  * The precision of this model(2) is similar to model 1 in that the precision in predictiong a '1' or high risk loan with a precision of 0.84 or 84% accuracy.
  * However, despite similar precision in the prediction of '1', this model has a recall of 0.99, meaning that this model would be 99% likely to predict a high-risk loan correctly.
  
  
## Summary

In conclusion, we can see that the machine learning model (2) that uses oversampling is more efficient than the machine learning model that uses just the original data. The balance accuracy score of the oversampling model was higher at 0.99 and has a better recall value of 0.99, compared to model 1's 91%. When it comes down to the purpose of this analysis, it is important to accurately determine which cases has a high-risk loan and in this situation the oversampling model will perform better. Although oversampling performs better in this data, it is not always the case in other data sets thus I would recommend trying out different learning models to figure out which model performs best to solve the problem that is being focused on.
