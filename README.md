# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
1.Import the required libraries and load the California Housing dataset.
2.Define the feature matrix X and target vector y.
3.Split the dataset into training and testing sets using train_test_split().
4.Create and train the Linear Regression model using the training data.
5.Predict the output, calculate the variance score, and plot the residual errors.
```
## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:
![alt text](image.png)
### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.