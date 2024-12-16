# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas libraryband linear_model from sklean using import statement

### Step2
Read the give csv file using read_csv()method

### Step3
Create teo array,independent array x with two classes and dependent array y with one class.find regression of x and y using linear_model.linearRegression() method and fit x and y using.fit()method.

### Step4
Find the coefficients using.coef_and intercept using.intercept_
### Step5
Predict the linear regression using regr.predict()method and display the result
## Program:
```
import pandas as pd 
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.linearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.Intercept_)
predicitedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predicitedCO2)


```
## Output:

### Insert your output

![Screenshot 2024-12-15 005658](https://github.com/user-attachments/assets/1ac25d54-7657-42f4-a38c-068404576c21)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
