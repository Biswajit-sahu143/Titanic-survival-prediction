# 🚢 Titanic Survival Prediction

A beginner-friendly Machine Learning project that predicts whether a passenger on the Titanic survived or not.

This project uses the Titanic dataset and a **Random Forest Classifier** to predict passenger survival based on features such as passenger class, gender, age, family size, fare, and embarkation port.

---

## 📌 Project Objective

The main objective of this project is to build a Machine Learning classification model that can predict whether a Titanic passenger survived or not.

- `0` → Did Not Survive
- `1` → Survived

This is a **Binary Classification** problem.

---

## 📊 Dataset

The Titanic dataset contains information about individual passengers, including:

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

The following preprocessing steps were performed:

- Missing values in the `Age` column were replaced with the median age.
- Missing values in the `Embarked` column were replaced with the most frequent value.
- Unnecessary columns such as `PassengerId`, `Name`, and `Ticket` were removed.
- Categorical columns such as `Sex` and `Embarked` were converted into numerical values using `LabelEncoder`.

---

## 🤖 Machine Learning Model

The project uses the **Random Forest Classifier**.

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees to make accurate predictions.

### Model Code

```python
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier(random_state=42)

model.fit(X_train, y_train)

y_pred = model.predict(X_test)
```

---

## 📈 Model Evaluation

The model is evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report
- Feature Importance

### Accuracy

```python
from sklearn.metrics import accuracy_score

accuracy = accuracy_score(y_test, y_pred)

print("Accuracy:", accuracy)
```

The model typically achieves around **80–85% accuracy**, depending on the dataset split and preprocessing.

---

## 📁 Project Structure

```text
Titanic-Survival-Prediction/
│
├── Titanic-Dataset.csv
├── Titanic-Survival-Prediction.ipynb
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Titanic-Survival-Prediction.git
```

### 2. Open the Notebook

Open:

```text
Titanic-Survival-Prediction.ipynb
```

You can run the notebook using:

- Google Colab
- Jupyter Notebook
- JupyterLab

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 4. Run the Notebook

Run all the cells from top to bottom.

---

## 🎯 Results

The Random Forest model successfully learns patterns from the Titanic passenger data and predicts whether passengers survived or not.

The model uses features such as:

- Gender
- Passenger Class
- Age
- Fare
- Family information

---

## 📚 Learning Outcomes

Through this project, I learned:

- Data loading and exploration
- Data cleaning
- Handling missing values
- Data preprocessing
- Encoding categorical variables
- Train-test splitting
- Machine Learning model training
- Classification
- Model evaluation
- Feature importance analysis

---

## 🚀 Future Improvements

Possible improvements for this project include:

- Trying Logistic Regression
- Trying Decision Tree Classifier
- Comparing multiple Machine Learning models
- Performing hyperparameter tuning
- Improving feature engineering
- Creating a user interface for survival prediction

---

## 👨‍💻 Author

**Biswajit Sahu**

This project was created as a beginner Machine Learning project to understand the complete workflow of a classification problem.

---

⭐ If you found this project useful, feel free to star the repository!
