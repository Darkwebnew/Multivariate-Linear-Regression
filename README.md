# EX 10 Implementation of Multivariate Linear Regression
## Date: 08.11.2023
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import panda
### Step2
Import linear model from sklearn
### Step3
Read the file cars.csv
### Step4
Assign the values for x and y as required
### Step5
Create the linearRegression model and predict the output
## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predictedd co2 for the corresponding weight and volume", predictedCO2)
```
## Output:
![image](https://github.com/Darkwebnew/Multivariate-Linear-Regression/assets/143114486/667d3480-7db8-4ca8-a8f7-78676fefa43d)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
