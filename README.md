# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
First,we want to import numpy,then import sys,assume a variable.
### Step2
For gaussian elimination method, we want to make 2nd and 3rd column zero.
### Step3
For that we want to make a range accorting to our program output.
### Step4
Then print the program with correct form then the output will display.
## Program:
```
Develope by:kishore.A
register number:23008675


import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)

```
## Output:

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
