# 🚢 Titanic Survival Prediction

A beginner-friendly Machine Learning project that predicts whether a passenger on the Titanic survived or not.

This project uses the Titanic dataset and a **Random Forest Classifier** to predict passenger survival based on features such as passenger class, gender, age, family size, fare, and embarkation port.

---

## 📌 Project Objective

The main objective of this project is to build a Machine Learning classification model that can predict:

- `0` → Did Not Survive
- `1` → Survived

This is a **Binary Classification** problem.

---

## 📊 Dataset

The dataset contains information about Titanic passengers, including:

- Passenger Class (`Pclass`)
- Gender (`Sex`)
- Age (`Age`)
- Number of Siblings/Spouses (`SibSp`)
- Number of Parents/Children (`Parch`)
- Ticket Fare (`Fare`)
- Port of Embarkation (`Embarked`)
- Survival Status (`Survived`)

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

---

## 🔄 Project Workflow

The project follows these steps:

1. Load the Titanic dataset
2. Explore and understand the dataset
3. Check for missing values
4. Handle missing values
5. Remove unnecessary columns
6. Convert categorical data into numerical values
7. Separate features and target variable
8. Split the dataset into training and testing data
9. Train a Random Forest Classifier
10. Make predictions
11. Evaluate the model
12. Analyze feature importance

---

## 🧹 Data Preprocessing

Missing values in the `Age` column are handled using the median value.

Missing values in the `Embarked` column are handled using the most frequent value.

The following unnecessary columns are removed:

- PassengerId
- Name
- Ticket

Categorical columns such as `Sex` and `Embarked` are converted into numerical values using `LabelEncoder`.

---

## 🤖 Machine Learning Model

The project uses the **Random Forest Classifier**.

Random Forest is an ensemble learning algorithm that combines multiple decision trees to make better predictions.

```python
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier(random_state=42)

model.fit(X_train, y_train)

y_pred = model.predict(X_test)
