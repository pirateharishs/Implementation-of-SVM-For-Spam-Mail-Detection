# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import the necessary python packages using import statements.

2.Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().

3.Split the dataset using train_test_split.

4.Calculate Y_Pred and accuracy.

5.Print all the outputs.

6.End the Program.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: HARISH S
RegisterNumber: 212223230071

import pandas as pd

data = pd.read_csv("/content/spam.csv",encoding = 'windows - 1252')

from sklearn.model_selection import train_test_split

data.shape

x=data['v2'].values

y=data['v1'].values

x.shape

y.shape

x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.35,random_state=0)

x_train

x_train.shape

from sklearn.feature_extraction.text import CountVectorizer

cv = CountVectorizer()

x_train = cv.fit_transform(x_train)

x_test = cv.transform(x_test)

from sklearn.svm import SVC

svc=SVC()

svc.fit(x_train,y_train)

y_pred=svc.predict(x_test)

acc = accuracy_score(y_test,y_pred)

acc

con=confusion_matrix(y_test,y_pred)

print(con)

cl=classification_report(y_test,y_pred)

print(cl)


*/
```

## Output:

## Head():

![image](https://github.com/user-attachments/assets/3d3a89fb-d7ac-45fc-b130-829187a0c33c)

## Info():

![image](https://github.com/user-attachments/assets/a4bd2764-9c5f-420a-a067-6c8107f74120)

## Prediction of y:

![image](https://github.com/user-attachments/assets/9f74f111-dceb-43a9-b55f-30d8b1711e66)

## Accuracy:

![image](https://github.com/user-attachments/assets/632098b0-174f-430d-bc7b-89f9410e8fd3)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
