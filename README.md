## Date:
# Exp-10: Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
The first step is to Import Pandas library.

### Step2
The second step is to Import Linear_model from sklearn.

### Step3
Then Read the csv file using pandas library.

### Step4
Enter the parameters of the linear function.

### Step5
Print the parameters of the linear function.

## Program:
```

#Program to implement multivariate linear regression and predict the output.
#Developed by: SURIYA M
#Reg no : 212223110055

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
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

### Insert your output
![image](https://github.com/user-attachments/assets/45d621db-68cd-4f8e-bd8a-ec4f6a08df91)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
