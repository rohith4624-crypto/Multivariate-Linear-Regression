# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.Import pandas as pd

2.read the csv file

3.find the value of X and Y variables

4.Create the linear regression model and fit

5.Predict the CO2 emission of car where the weight of 2300kg, and the volume is 1300cm cube.
## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)





```
## Output:

<img width="690" height="96" alt="image" src="https://github.com/user-attachments/assets/963d273a-d206-461b-acf9-da350801f58e" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
