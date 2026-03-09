# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import required libraries
2. Load the dataset
3. Preprocess the data (handle categorical values)
4. Split data into training and testing sets
5. Train the Decision Tree model
6. Predict the results
7. Evaluate the model accuracy

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Hari Ramesh
RegisterNumber:212225100016
# Import required libraries
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score

# Sample Employee Dataset
data = {
    'Age': [25, 30, 45, 35, 22, 40, 50, 29],
    'Salary': [30000, 50000, 80000, 60000, 25000, 70000, 90000, 48000],
    'Years_at_Company': [1, 3, 10, 5, 1, 7, 12, 4],
    'Churn': [1, 0, 0, 0, 1, 0, 0, 1]   # 1 = Leave, 0 = Stay
}

df = pd.DataFrame(data)

# Features and Target
X = df[['Age', 'Salary', 'Years_at_Company']]
y = df['Churn']

# Split dataset
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42)

# Create Decision Tree model
model = DecisionTreeClassifier()

# Train the model
model.fit(X_train, y_train)

# Predict
y_pred = model.predict(X_test)

# Accuracy
accuracy = accuracy_score(y_test, y_pred)

print("Predicted Values:", y_pred)
print("Actual Values:", y_test.values)
print("Model Accuracy:", accuracy)  
*/
```

## Output:

<img width="329" height="83" alt="Screenshot 2026-03-09 110240" src="https://github.com/user-attachments/assets/4bad31ba-545d-47fe-a7d8-bc9febef886a" />


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
