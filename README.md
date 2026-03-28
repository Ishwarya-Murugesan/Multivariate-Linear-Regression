# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Data Preparation

### Step2
Define the Hypothesis Function

### Step3
Cost Function

### Step4
Optimization (Gradient Descent / Normal Equation)

### Step5
Model Evaluation & Prediction

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
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


<img width="832" height="379" alt="Screenshot 2026-03-28 142816" src="https://github.com/user-attachments/assets/dae3729c-79a2-4fbd-b907-56e22604b4ec" />
<img width="861" height="480" alt="Screenshot 2026-03-28 142832" src="https://github.com/user-attachments/assets/8adb17da-6724-4eb4-920d-093eadccdce2" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
