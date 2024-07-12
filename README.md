# CSINTSY-MCO3

This group project was completed in partial fulfillment of the course requirements for CSINTSY.

### LINEAR REGRESSION
This model aims to establish a linear relationship and predict the value of the dependent, output variable (in this case, the “close” stock prices) based on the independent, input variable (the “open” stock prices).

This algorithm fits a linear equation of the form, y = mx + b wherein m is the line’s slope and b is the y-intercept. This linear equation is used to train the model with the data being split into subsets for training and testing sets. The linear equation will be continuously adjusted in order to minimize the difference between the predicted and the actual values on the training subset, and therefore finding the best fit for the line.

Consequently, evaluation of the trained model will include assessing its performance on the testing subset through the R² (R-squared) score. R² provides a measure of how well the linear regression model explains the variability in “close stock prices” based on “open stock prices”.

### RIDGE REGRESSION
Ridge Regression is a model tuning method that is used to analyze data that suffers multicollinearity. This model follows the usual linear regression formula which is y = mx + b but with the addition of the L2 regularization method which is the penalty term where in it gets the minimum sum of the squared residuals plus the multiple of the alpha (or lambda) value and the squared slope. Its purpose is to make the results of the regression become less affected by the variations of the independent variable making the resulting plot be more horizontally inclined. It also makes the model less prone to overfitting (learning too much from the training dataset) leading to a better generalization of the pattern behind the data and better performance on newer, unseen data.

The input of this regression are the independent variables of the given data set. In this case, the independent variable of the plot would be the “Open stock prices”. Here we assume that this piece of data has a linear relationship with the dependent variable “Closed stock prices.”

At the end of the processing of the data in the regression model, The R² value will be used to compare with the linear regression model. The R² value represents how close the predicted values generated by the model are to the actual values. The closer the R² value is to 1, the more accurate the model is.

## Linear vs. Ridge Regression:

After training both models, based on their respective resulting R²  scores, which show how well the data fit the regression model, it can be observed that both models' results are very close to each other. In evaluating R² scores, the larger the value (the closer to 100% or 1.0), the better. Linear Regression has an R²  score of 0.9977876704303842, while Ridge Regression has an R² score of 0.9977875953364784. This indicates that both models are a good fit. The only difference between the two scores lies in their decimal values, indicating that Linear Regression is a slightly better-fitting model.

Another reason why using Linear Regression is better is because the model only uses one dependent variable (in this case, the “close” stock prices) and one independent variable (the “open” stock prices). Ridge regression is more beneficial when there are multiple independent variables, as its primary purpose is to mitigate multicollinearity issues. A simple Linear Regression might perform equally well or even better as it can already adequately describe the connection between the single dependent and independent variables in the model, making the additional complexity Ridge regression offers unnecessary.

