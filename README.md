# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import necessary libraries such as NumPy, Pandas, and Scikit-learn for data handling and model building.

### Step2
<br>
Read the dataset, separate independent variables (X) and dependent variable (y), and split the data into training and testing sets.

### Step3
<br>
Create a Linear Regression model and fit it using the training data to learn the relationship between variables.
 
 ### Step4
<br>
Use the trained model to predict outputs for test data and display the predicted results.
 
 ### Step5
<br>
Check the performance of the model using metrics like accuracy, Mean Squared Error (MSE), or R² score to determine how well the model predicts the output.
 
 ## Program:
```
#Developed By:Kamali V 
#Ref no :212225240066


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

![image](https://github.com/kamaliv-1602/Multivariate-Linear-Regression/blob/master/Screenshot%202026-03-26%20101653.png?raw=true)


### Insert your output


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
