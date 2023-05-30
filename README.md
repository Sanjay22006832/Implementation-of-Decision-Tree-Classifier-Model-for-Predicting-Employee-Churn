# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.
2.Read the data set.
3.Apply label encoder to the non-numerical column inoreder to convert into numerical values.
4.Determine training and test data set.
5.Apply decision tree Classifier and get the values of accuracy and data prediction.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: M Sanjay
RegisterNumber: 212222240090
import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull()
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
![Screenshot 2023-05-16 214111](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/154c9eb8-8333-48c5-8d8f-62db90a413d7)

![Screenshot 2023-05-16 214122](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/144e7cf4-e430-4dc3-942f-eb76b34c34cc)

![Screenshot 2023-05-16 214132](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/ee05ccb1-ef92-444f-9f69-951c2e39ed1f)

![Screenshot 2023-05-16 214140](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/122ec72c-2e10-4daa-9d95-0209a6e05f3f)

![Screenshot 2023-05-16 214146](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/1aa77bf5-e021-44a4-872e-f2f720cfd7e3)

![Screenshot 2023-05-16 214202](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/1ec4ed71-2bf4-4b25-8771-a0a973e33090)

![Screenshot 2023-05-16 214208](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/b84b598e-c83e-4df8-a8d4-2aa717469988)

![Screenshot 2023-05-16 214220](https://github.com/Sanjay22006832/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119830477/72a9badb-3d81-455f-ab62-301b74f547e4)




## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
