# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries.
2.Upload the csv file and read the dataset.
3.Check for any null values using the isnull() function.
4.From sklearn.tree inport DecisionTreeRegressor.
5.Import metrics and calculate the Mean squared error.
6.Apply metrics to the dataset, and predict the output.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: BALA MURUGAN 
RegisterNumber:  212222230017

import pandas as pd
data=pd.read_csv("/content/Salary(1).csv")
print('data.head():')
data.head()
print('data.info():')
data.info()
print('isnull() and sum():')
data.isnull()
print('data.head() for salary:')
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
print('MSE value:')
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
print('r2 value:')
r2 = metrics.r2_score(y_test,y_pred)
r2
print('data prediction:')
dt.predict([[5,6]])


*/
```

## Output:
![Decision Tree Regressor Model for Predicting the Salary of the Employee](sam.png)

![240625208-852c50c9-64bb-4412-b661-8f6b55feb5a0](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/72af6bca-e2f6-47ae-b286-fcb1242b9ec2)

![240625274-9ddf7ade-efec-4780-ba6c-2fdad008f207](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/a7ae6323-3981-4ef9-acad-071c26d6bfba)

![240625422-6ab42b5a-c402-44b4-aac4-eccf4a329d6f](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/de88c425-90d9-430b-bb6c-fb6ab91a58ed)

![240625547-06a63650-48a7-4742-bc37-417a56767409](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/385ba55f-e4f5-47b0-a814-b829ffab5418)


![240625613-f21aa42f-96be-4ed8-8432-8278c0e6429f](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/cfaa34d9-cca6-41e8-a3ea-d3dc35d9397d)

![240625661-d2d35478-e397-49a0-8530-6db4aabd85f0](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/b016fa72-b3ca-4020-8f21-7808ce6c031a)

![240625836-a11b4bf4-fc84-4214-8595-9865efa559bb](https://github.com/Bala1511/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118680410/0d71bb6a-e0fd-4b50-a606-3c9c2cf569a3)
## RESULT:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
