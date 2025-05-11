# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step1:Import panda
## Step2:Import linear model from sklearn
## Step3:Read the file cars.csv
## Step4:Assign the values for x and y as required
## Step5: Create the linearRegression model and predict the output
## Program:

```
Implementation of Multivariate Linear Regression
Developed by: Sanchita Sandeep
RegisterNumber: 212224240142

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)





```
## Output:

![WhatsApp Image 2025-05-10 at 14 12 48_18626837](https://github.com/user-attachments/assets/584f7b83-d849-46f6-a5f7-4f90e7834099)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
