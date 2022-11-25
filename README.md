# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard libraries. 
2.Upload the dataset and check for any null values using .isnull() function. 
3.Import LabelEncoder and encode the dataset. 
4.Import DecisionTreeClassifier from sklearn and apply the model on the dataset. 
5.Predict the values of array. 
6.Import metrics from sklearn and calculate the accuracy of the model on the dataset. 
7.Predict the values of array. 
8.Apply to new unknown values.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: VASANTHAN 
RegisterNumber: 212220220052


import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)

y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![ss1](https://user-images.githubusercontent.com/115924983/203999566-26fd458e-2671-4ab0-a75b-0f8c87bd2335.png)

![ss2](https://user-images.githubusercontent.com/115924983/203999587-bc804e18-b5ce-4245-a33e-b52941002fd0.png)

![ss3](https://user-images.githubusercontent.com/115924983/203999625-6a522fa5-a3c7-41d5-b7da-eb92013c8fae.png)

![ss4](https://user-images.githubusercontent.com/115924983/203999647-e0cb47f8-735e-4185-968b-6397ef410184.png)

![ss5](https://user-images.githubusercontent.com/115924983/203999665-a17900f5-12d1-4a46-bbb2-bb2f13623237.png)

![ss6](https://user-images.githubusercontent.com/115924983/203999678-67910e35-8c2c-4a3b-aaca-3b6be59f88f8.png)

![ss7](https://user-images.githubusercontent.com/115924983/203999693-0d39e0b6-785d-4bc9-ba31-cf8b51c719b6.png)

![ss8](https://user-images.githubusercontent.com/115924983/203999719-526ead30-243e-40ad-870a-8fef2d4bd832.png)

![ss9](https://user-images.githubusercontent.com/115924983/203999764-beebe4fa-14fa-4e14-8beb-2b22563ef697.png)

![ss10](https://user-images.githubusercontent.com/115924983/203999791-1b1872e7-6c1b-4788-b33e-cbefb357c754.png)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
