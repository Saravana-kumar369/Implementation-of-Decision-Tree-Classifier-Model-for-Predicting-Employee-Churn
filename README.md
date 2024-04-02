![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/abc5441c-7b6b-436d-b20a-87c2ea6712ff)# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. select each feature
2.compute  
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SARAVANA KUMAR
RegisterNumber: 212222230133 
*/

import pandas as pd
from sklearn.tree import DecisionTreeClassifier,plot_tree
from sklearn.preprocessing import LabelEncoder
import matplotlib.pyplot as plt
df=pd.read_csv('/content/Employee_EX6.csv')
df.head()
df.info()
df.isnull().sum()
df["left"].value_counts()
```

## Output:
![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/aacf3ca2-fbb1-4295-9e30-960e96316209)

![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/f3511641-8e10-4102-a0ce-5adba612018a)

![image](https://github.com/Saravana-kumar369/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/117925254/0900bb07-379b-462d-b0e5-b56b1e6c90b0)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
