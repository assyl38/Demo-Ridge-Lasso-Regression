# What is Data Fitting
The procces of plotting a series of data points and drawing the best fit line to understand the relationship between the variables is called "Data Fitting".
It is a linear relationship: the line used to represent the relationship is a straight line that passes through the data points and the variables have a linear relationship.

# Bias and Variance
Bias occurs when an algorithm has limited flexibility to learn from data while the variance defines the algorithm's sensitivity to sepcific sets of data.

![1_2HV_rbv0XEgmOveyMw3X8g](https://user-images.githubusercontent.com/57531658/160246824-7cc50b22-f186-4108-9cf5-29e533748f28.png)
 # Overfitting
 A scenario where the machine learning model tries to learn from the details along with the noise in the data and tries to fit each data point on the curve. </br>
 
Reasons for overfitting : </br>

1/ Data used for training is not cleaned and contains noise (garbage values). </br>
2/ The model has a high variance. </br>
3/Size of training data is not enough. </br>
4/ The model is too complex.</br>

# Underfitting
A scenario where machine learning model can neither learn the relationship between variables in the data nor predict or classify a new datapoint . </br>

Reasons for underfitting : </br> 

1/ Data used for training is not cleaned and contains noise (garbage values). </br>
2/ The model has a high bias.</br>
3/ Size of training data used is not enough. </br>
4/ The model is too simple. </br>

# A good fit
A line or a curve that best fits the data is neither overfitting nor underfitting models but is just right.

![Identify_overfitting_underfitting](https://user-images.githubusercontent.com/57531658/160247090-3b950af4-0d9d-4212-8c6e-aeb73eca9d62.png)

# Regularization
Regularization techniques are used to calibrate the linear regression models in order to minimize the adjusted loss function and prevent overfitting or underfitting.

![ezgif com-gif-maker](https://user-images.githubusercontent.com/57531658/160247467-d72e9c7c-8265-4ba5-8ec0-39eae2c27d37.png)

Lasso and Ridge regression, also known as L1 & L2 respectively, are “regularization” techniques.

![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/57531658/160247551-17b8580c-d14e-47fe-a1c5-2d3f775cbe6f.png)

The goal of regularization is to improve the overall fit by increasing “bias” to reduce “variance”, by adding a penalty that scales with model complexity.

![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/57531658/160247601-6c26f9f2-118b-490f-96b9-47b2d74d0802.png)

![ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/57531658/160247631-c41a2945-3ba2-43df-8b7b-735751ba163f.png)

Applying this to linear regression, we start with a line through our data.

![ezgif com-gif-maker (5)](https://user-images.githubusercontent.com/57531658/160247686-334e2a73-2563-4334-9a63-39cca5552939.png)

We calculate the residuals per usual.

![ezgif com-gif-maker (6)](https://user-images.githubusercontent.com/57531658/160247738-f20b6b2e-942e-4e1b-bee8-79348b91a538.png)

Then the penalty is calculated. For Lasso, the penalty scales with the absolute value of the slope, and for Ridge it scales with the slope squared.

![ezgif com-gif-maker (7)](https://user-images.githubusercontent.com/57531658/160247796-1bb5540b-a839-472c-b0a6-631e9751e912.png)

The penalty is added to our residual, and then the algorithm proceeds via the least-squares method.

![ezgif com-gif-maker (6)](https://user-images.githubusercontent.com/57531658/160247827-91913235-7b01-40f5-9247-316f02a7cfb3.png)

The result is a best-fit line with a smaller slope, that will hopefully fit our test data better.

![ezgif com-gif-maker (9)](https://user-images.githubusercontent.com/57531658/160247866-4dfc9c3e-ed21-451a-902a-550913e20901.png)



