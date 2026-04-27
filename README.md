# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import necessary libraries (numpy, matplotlib, sklearn.linear_model).
2. Create a LinearRegression model object.
3. Accept user input (x_input) for hours studied.
4. Generate predicted values (Y_pred) for the dataset.

## Program:
```python
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Naresh J
RegisterNumber: 212225230195
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

# Sample data

X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])

# Create model
model = LinearRegression()

# Train model
model.fit(X, Y)

# Get slope and intercept
m = model.coef_[0]
b = model.intercept_

print("Slope (m):", m)
print("Intercept (b):", b)

# ---- Prediction ----
x_input = float(input("Enter hours studied: "))
predicted_marks = model.predict([[x_input]])
print("Predicted Marks:", predicted_marks[0])

# ---- Plot ----
Y_pred = model.predict(X)

plt.scatter(X, Y, label="Actual Data")
plt.plot(X, Y_pred, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression (Using sklearn)")
plt.legend()
plt.show() 
*/
```

## Output:
<img width="973" height="668" alt="image" src="https://github.com/user-attachments/assets/23fc5013-03db-4780-be6b-04a8d148e2d1" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
