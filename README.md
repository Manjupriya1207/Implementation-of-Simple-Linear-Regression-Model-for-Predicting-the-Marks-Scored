# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Manjupriya P
RegisterNumber:  212220220024
*/
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

data=pd.read_csv('/content/student_scores.csv')

data.head()

data.tail()

x=data.iloc[:,:-1].values  
y=data.iloc[:,1].values

print(x)
print(y)

from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split

x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=1/3,random_state=0 )

regressor=LinearRegression() 
regressor.fit(x_train,y_train)

y_pred=regressor.predict(x_test) 
print(y_pred)

print(y_test)

#for train values
plt.scatter(x_train,y_train) 
plt.plot(x_train,regressor.predict(x_train),color='black') 
plt.title("Hours Vs Score(Training set)") 
plt.xlabel("Hours")
plt.ylabel("Score")
plt.show()

#for test values
y_pred=regressor.predict(x_test) 
plt.scatter(x_test,y_test) 
plt.plot(x_test,regressor.predict(x_test),color='black') 
plt.title("Hours Vs Score(Test set)") 
plt.xlabel("Hours")
plt.ylabel("Score")
plt.show()

import sklearn.metrics as metrics

mae = metrics.mean_absolute_error(x, y)
mse = metrics.mean_squared_error(x, y)
rmse = np.sqrt(mse)  

print("MAE:",mae)
print("MSE:", mse)
print("RMSE:", rmse)
```

## Output:
![simple linear regression model for predicting the marks scored](<img width="576" alt="ex_2 op2" src="https://user-images.githubusercontent.com/113583090/230037000-7676c828-f63a-4839-9001-0839ee8a732b.png"><img width="576" alt="exp_2 op1" src="https://user-images.githubusercontent.com/113583090/230037101-629901be-9200-45df-ae17-14d79308c704.png"><img width="409" alt="exp_2 op" src="https://user-images.githubusercontent.com/113583090/230037188-ed1db472-94ca-47e9-930b-af1d96a2a2ff.png">
![Uploading exp_2 op1.png…]()![Uploading exp_2 op.png…]())


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
