# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:
1. Load the dataset containing employee information
2. encoding categorical variables, and splitting the dataset into training and testing sets.
3. Choose a splitting criterion such as gini index or entropy and select the best feature to split on based on the chosen criterion.
4. Recursively split the dataset based on the selected feature until the feature has no impurity.
5. Find the accuracy of the model and predict the required values by importing the required module from sklearn.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SARAVANA KUMAR
RegisterNumber: 212222230133 
*/
```
```
import pandas as pd
from sklearn.tree import DecisionTreeClassifier,plot_tree
from sklearn.preprocessing import LabelEncoder
import matplotlib.pyplot as plt
df=pd.read_csv('/content/Employee_EX6.csv')
df.head()
df.info()
df.isnull().sum()
df["left"].value_counts()
le=LabelEncoder()
df['salary']=le.fit_transform(df['salary'])
df.head()
x=df.drop(['Departments','left'],axis=1)
y=df['left']
from sklearn.model_selection import train_test_split as t
x_train,x_test,y_train,y_test=t(x,y,test_size=0.2,random_state=100)
dt=DecisionTreeClassifier(criterion='entropy')
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics as m
accuracy=m.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
```

## Output:
## Head
![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/aacf3ca2-fbb1-4295-9e30-960e96316209)
## Accuracy
![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/f3511641-8e10-4102-a0ce-5adba612018a)
## Predicted value
![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/0900bb07-379b-462d-b0e5-b56b1e6c90b0)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
