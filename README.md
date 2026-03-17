# iris-classification-project

## 📌 Overview
This project focuses on building a machine learning model to classify iris flowers into three different species based on their physical features. It is a classic classification problem in machine learning.

---

## 📊 Dataset
The dataset contains 150 samples with the following features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

Target Variable:
- Species (Setosa, Versicolor, Virginica)

---

## 🔍 Exploratory Data Analysis (EDA)
- Checked dataset structure using `head()`, `info()`, and `describe()`
- Identified missing values (none found)
- Visualized data using:
  - Pairplot
  - Histogram
  - Boxplot
  - Scatter Plot

---

## 🧹 Data Preprocessing
- Encoded categorical target variable (`species`) using LabelEncoder
- Split dataset into training and testing sets (80:20 ratio)

---

## 🤖 Models Used
The following machine learning models were trained and compared:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier

---

## 📈 Model Evaluation
Models were evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

Best performing model: **Decision Tree / KNN (based on accuracy)**

---

## 💾 Model Saving
The best model was saved using `joblib`:
```python
import joblib
joblib.dump(model, "iris_model.pkl")
