# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
step 1: start the program

step 2: Get the independent variable X and dependent variable Y.

step 3: Calculate the mean of the X -values and the mean of the Y -values.

step 4: find the slope m of the line of best fit using the formula. 

step 5: Compute the y -intercept of the line by using the formula:\

step 6: Use the slope m and the y -intercept to form the equation of the line.

step 7: Obtain the straight line equation Y=mX+b and plot the scatterplot.

step 8: End the program
## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
## Developed by: Jayasuryaa k
## RegisterNumber: 212222040060

import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='blue')
plt.plot(X,Y_pred,color='yellow') 
plt.show() 
*/
```

## Output:
![Screenshot 2024-08-28 111208](https://github.com/user-attachments/assets/2bdd9862-3070-4adb-b5c4-1c075e7085ed)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
