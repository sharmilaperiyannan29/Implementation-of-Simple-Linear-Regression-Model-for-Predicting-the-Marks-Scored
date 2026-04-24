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
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Sharmila P
RegisterNumber: 212225230261
*/
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
denom=0
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-m*x_mean
print(m,b)
y_predicted=m*x+b
print(y_predicted)
plt.scatter(x,y)
plt.plot(x,y_predicted,color='red')
plt.show()

```

## Output:
<img width="640" height="618" alt="image" src="https://github.com/user-attachments/assets/de592954-3432-4af5-8d4b-919e4a8a42c7" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
