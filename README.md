
## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Developed by: SELVARANI S
## RegisterNumber:  212224040301

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required Python libraries such as Pandas, Matplotlib, and Scikit-learn.
2. Load the student dataset containing hours studied and marks scored.
3. Split the dataset into input variable X (hours studied) and target variable Y (marks scored), and train a Simple Linear Regression model.
4. Predict the marks for a given number of study hours and display the predicted result.

## Program:
```

import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

x=np.array([1,2,3,4,5]).reshape(-1,1)
y=np.array([35,50,65,70,85])

model=LinearRegression()
model.fit(x,y)

x_input = float(input("Enter hours studied: "))
pred_mar = model.predict([[x_input]])
print("Predicted Marks:", pred_mar[0])

y_pred=model.predict(x)
plt.scatter(x, y, label=" Actual Data")
plt.plot(x, y_pred, label="Regression Line")
plt.xlabel("Hours studied")
plt.ylabel("mark scored")
plt.title("simple linear regression using ")
plt.legend()
plt.show()

```

## Output:
<img width="868" height="650" alt="image" src="https://github.com/user-attachments/assets/36e319f9-c4dd-4a45-9fe0-9fc1c498d4bb" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
