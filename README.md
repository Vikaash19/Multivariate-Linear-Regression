# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
Import pandas
### Step2:
Import linear model from sklearn
### Step3:
Read the file cars.csv
### Step4:
Assign the values for x and y as required
### Step5: 
Create the linearRegression model and predict the output

## Program:
```
'''
Program to implement multivariate linear regression
Developed by:Vikaash K S
Register no: 23013426
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)
```
## Output:
![Multivariate LR](https://github.com/Vikaash19/Multivariate-Linear-Regression/assets/148514589/a6557837-6226-4afb-a28d-abe9f212fd36)
## Result:
Thus the multivariate linear regression is implemented and predicted the output using python program.
