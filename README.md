# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas

2.Import Decision tree classifier

3.Fit the data in the model

4.Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: PARANTHAMAN S
RegisterNumber: 212224040232
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
print(data.head())
x=data[["Position","Level"]]
print(x.head())
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print(y_pred)
from sklearn import metrics
r2=metrics.r2_score(y_test,y_pred)
print(r2)
dt.predict([[5,6]])
*/
```

## Output:
![Screenshot 2025-04-23 230331](https://github.com/user-attachments/assets/f5856558-8f90-4e56-9d6c-e9380477de90)

![Screenshot 2025-04-23 230339](https://github.com/user-attachments/assets/2bf6c7ac-29ec-4dd4-adca-332c5f16cb60)

![Screenshot 2025-04-23 230346](https://github.com/user-attachments/assets/ab4d45e2-a389-40a1-93bd-3788e282605f)

![Screenshot 2025-04-23 230404](https://github.com/user-attachments/assets/66bdb428-582b-445d-a42b-9c77776ced89)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
