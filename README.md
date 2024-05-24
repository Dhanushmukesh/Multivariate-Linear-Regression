# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
Step1:import pandas as pd.
Step2:Read the csv file.
Step3:Get the value of X and y variables
Step4:Create the linear regression model and fit.
Step5:Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
```
## Program:
```
#Program to find Multivariate Linear Regression
#Developed by Dhanush.G
#REG NO : 2305002006
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
X=df[['Weight', 'Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print("Coefficient:", regr.coef_)
print("Intercept: ", regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume", predictedCO2)
```
## Output:
![Screenshot 2024-05-24 114427](https://github.com/Dhanushmukesh/Multivariate-Linear-Regression/assets/155508176/2b35200f-7c40-4a19-b92b-c376f4871fbd)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
