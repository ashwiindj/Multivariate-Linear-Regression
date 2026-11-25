# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step 1: Import Pandas and the required module from Scikit-learn.   
Step 2: Read the carsemission.csv dataset.  
Step 3: Select Weight and Volume as independent variables.  
Step 4: Select CO2 as the dependent variable.  
Step 5: Create and train a Multivariate Linear Regression model.  
Step 6: Display the regression coefficients and intercept.  
Step 7: Predict the CO₂ emission for: Weight = 3300 Volume = 1300  
Step 8: Display the predicted CO₂ emission.  

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
<img width="737" height="390" alt="image" src="https://github.com/user-attachments/assets/846c84e8-4028-4850-bc6f-b23cfb0d7574" />  
<img width="681" height="75" alt="image" src="https://github.com/user-attachments/assets/b213877d-6259-47cf-937e-911f0baa64d1" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
