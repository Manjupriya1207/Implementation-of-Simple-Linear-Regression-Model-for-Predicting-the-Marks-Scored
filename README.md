# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. Read the given dataset

2. Assign values for x and y and plot them

3. Split the dataset into train and test data

4. Import linear regression and train the data

5. find Y predict

6. Plot train and test data

7. Calculate mse,mae and rmse

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by:S.SRIMATHI
RegisterNumber:212220040160 

import numpy as np

import pandas as pd

dataset=pd.read_csv('/content/student_scores.csv')

dataset.head()

dataset.tail()

#assingning hrs to x and scores to y

x=dataset.iloc[:,:-1].values

y=dataset.iloc[:,1].values

print(x)

print(y)

x=dataset.iloc[:,:-1].values

y=dataset.iloc[:,1].values

print(x)

print(y)

import matplotlib.pyplot as plt

from sklearn.metrics import mean_absolute_error, mean_squared_error

plt.scatter(x_train,y_train,color='grey')

plt.plot(x_train,reg.predict(x_train),color='magenta')

plt.title('Training set(H vs S)')

plt.xlabel('Hours')

plt.ylabel('Scores')

plt.show()

plt.scatter(x_test,y_test,color='magenta')

plt.plot(x_test,reg.predict(x_test),color='grey')

plt.title('Test set(H vs S)')

plt.xlabel('Hours')

plt.ylabel('Scores')

plt.show()

print(y_predict)

print(y_test)

mse=mean_squared_error(y_test,y_predict)

print('MSE = ',mse)

mae=mean_absolute_error(y_test,y_predict)

print('MAE = ',mae)

import numpy as np

np. sqrt(3)

rmse=np.sqrt(mse)

print('RMSE = ',rmse)

*/
```

## Output:
## DATA.HEAD():
![image](https://github.com/srimathi-25/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/114581999/73e87bd4-5ce9-4203-9441-ba67159c65a2)
## DATA.TAIL():
![image](https://user-images.githubusercontent.com/114581999/229363874-f3545eb0-472c-495f-8b3c-705a02d9b2a0.png)

## ARRAY VALUES OF X AND Y:

![image](https://user-images.githubusercontent.com/114581999/229363192-17c58540-64bf-4894-a659-633deaaa0bd2.png)

## TRAINING SET GRAPH:
![image](https://user-images.githubusercontent.com/114581999/229363231-3407e72d-c662-4cef-ab4b-cb7c969ad38d.png)

## TEST SET GRAPH:
![image](https://user-images.githubusercontent.com/114581999/229363252-584735c8-88db-4b30-aeb4-54b8d8dda0bb.png)

## VALUES OF Y PREDICTION:

![image](https://user-images.githubusercontent.com/114581999/229363279-e0e382bd-af26-4b5d-9459-bb3376f08101.png)

## ARRAY VALUES OF Y TEST:

![image](https://user-images.githubusercontent.com/114581999/229363310-2c16ecbc-e308-4f95-b9e4-5019cfe760bc.png)

## VALUES OF MSE,MAE AND RMSE:

![image](https://user-images.githubusercontent.com/114581999/229363534-ef9f24d3-b73a-4e03-9464-c567b2d8f07c.png)






## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
