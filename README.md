# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
~~~
1. Import the required packages.
2.Import the dataset to operate on.
3.Split the dataset.
4.Predict the required output.
5.End the program
~~~

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Manoj M
RegisterNumber:  212221240027
import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extractiaon.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
Data Head:

![a1](https://user-images.githubusercontent.com/94588708/173184075-a5448220-b822-4e4a-8406-268387bde344.png)


Data Info:


![a2](https://user-images.githubusercontent.com/94588708/173184086-f6c7cbf3-6593-4924-87cd-3f8c7b73ca19.png)



Data isnull():


![a3](https://user-images.githubusercontent.com/94588708/173184094-29abdaa7-e86a-4b7c-bf23-7ac78533672f.png)



y_pred:


![a4](https://user-images.githubusercontent.com/94588708/173184111-fd905f3d-8039-429c-b9af-761e6b2f18d8.png)



Accuracy:



![a5](https://user-images.githubusercontent.com/94588708/173184122-47c59aa7-86b2-4a41-b672-efe4985fa0d5.png)







## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
