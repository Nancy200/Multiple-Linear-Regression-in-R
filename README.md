# Multiple-Linear-Regression-in-R
Predicting Boston Housing Prices. The file BostonHousing.csv contains information collected by the US Bureau of the Census concerning housing in the area of
Boston, Massachusetts. The dataset includes information on 506 census housing tracts
in the Boston area. The goal is to predict the median house price in new tracts based
on information such as crime rate, pollution, and number of rooms. The dataset contains 13 predictors, and the response is the median house price (MEDV).

a. Why should the data be partitioned into training and validation sets? What will the
training set be used for? What will the validation set be used for?
Ans - The data should be partitioned into training and validation sets to train the model and check the performance of the model using different sets of data. Training set is the sample of data used to fit and train the model whereas validation dataset is the sample of data used for giving an unbiased evaluation of a model developed. In all, the training set will be used to estimate the model, and the validation or holdout set will be used to assess this model’s predictive performance on new, unobserved data.

b. Fit a multiple linear regression model to the median house price (MEDV) as a
function of CRIM, CHAS, and RM. Write the equation for predicting the median
house price from the predictors in the model.

c. Using the estimated regression model, what median house price is predicted for a
tract in the Boston area that does not bound the Charles River, has a crime rate of
0.1, and where the average number of rooms per house is 6? What is the prediction
error?

d. Reduce the number of predictors:
i. Which predictors are likely to be measuring the same thing among the 13
predictors? Discuss the relationships among INDUS, NOX, and TAX.
ii. Compute the correlation table for the 12 numerical predictors and search for
highly correlated pairs. These have potential redundancy and can cause multicollinearity. Choose which ones to remove based on this table.
iii. Use stepwise regression with the three options (backward, forward, both) to reduce
the remaining predictors as follows: Run stepwise on the training set. Choose
the top model from each stepwise run. Then use each of these models separately
to predict the validation set. Compare RMSE, MAPE, and mean error, as well
as lift charts. Finally, describe the best model
