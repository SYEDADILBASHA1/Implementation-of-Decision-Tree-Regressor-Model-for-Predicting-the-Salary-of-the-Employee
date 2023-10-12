# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import necessary libraries.
2. Load and preprocess your dataset.
3. Split the data into training and testing sets.
4. Create and train the Decision Tree Regressor.
5. Make predictions on the test set.
6. Evaluate the model.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SYED ADIL BASHA
RegisterNumber:  212221043008

import pandas as pd
data=pd.read_csv("/content/Salary.csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()

x=data[["Position","Level"]]
y=data["Salary"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)

from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse

r2=metrics.r2_score(y_test,y_pred)
r2

dt.predict([[5,6]])


*/
```

## Output:

## 1.data.head():
![Screenshot (123)](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/03fe7e7b-9207-482c-b09c-0e6c126bd0e2)

## 2.data.info():
![Screenshot (127)](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/3cbe9b67-717d-42b7-982d-5b882cfb06ab)

## 3.isnull() & sum() function:
![3](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/f09bf215-6ffc-44b2-8d0f-72965fe61d54)

## 4.data.head() for Position:
![Screenshot (124)](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/6062526b-8d82-4a15-b69d-1923f0686ebd)

## 5.MSE Value:
![Screenshot (125)](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/323eaf73-6bab-46c4-8de7-3c5fffedce97)

## 6.R2 Value:
![Screenshot (12)](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/0b9487f3-60da-40e2-bf40-55fd10a3ee0d)

## 7.Prediction Value:
![Screenshot (128)](https://github.com/SYEDADILBASHA1/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134796157/957fc48e-ef8e-479d-b2a0-a714937877ba)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
