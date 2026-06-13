Based on your notebook, your project is a **Sales Prediction using Advertising Data** project that uses **Linear Regression** to predict sales from advertising spending on TV, Radio, and Newspaper.

You can use the following README.md content:

# 📊 Advertising Sales Prediction

## 📌 Project Overview

This project predicts product sales based on advertising expenditure across different marketing channels such as TV, Radio, and Newspaper. The objective is to analyze the relationship between advertising budgets and sales and build a machine learning model that can accurately forecast future sales.

## 🎯 Objective

* Analyze advertising data.
* Identify the impact of TV, Radio, and Newspaper advertisements on sales.
* Build a predictive model using Machine Learning.
* Predict future sales based on advertising budgets.

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Joblib

## 📂 Dataset Features

| Feature   | Description                           |
| --------- | ------------------------------------- |
| TV        | Advertising budget spent on TV        |
| Radio     | Advertising budget spent on Radio     |
| Newspaper | Advertising budget spent on Newspaper |
| Sales     | Product sales (Target Variable)       |

## 📈 Exploratory Data Analysis (EDA)

The following analyses were performed:

* Data loading and inspection
* Missing value checking
* Duplicate value checking
* Statistical summary of dataset
* Correlation analysis
* Heatmap visualization

### Correlation Heatmap

A heatmap was generated to understand the relationship between advertising channels and sales.

## 🤖 Machine Learning Model

### Algorithm Used

* Linear Regression

### Data Splitting

* Training Data: 80%
* Testing Data: 20%

```python
train_test_split(test_size=0.2, random_state=42)
```

## 🔄 Model Training

The Linear Regression model was trained using:

```python
model = LinearRegression()
model.fit(X_train, y_train)
```

## 📊 Model Evaluation

The model performance was evaluated using:

### R² Score

```python
from sklearn.metrics import r2_score
r2 = r2_score(y_test, y_predict)
```

R² Score measures how well the model explains the variance in sales.

## 💾 Model Saving

The trained model was saved using Joblib.

```python
joblib.dump(model, 'evebatch.pkl')
```

## 🔮 Prediction Example

```python
loaded_model.predict([[22.3, 32.3, 22.4]])
```

### Input

* TV Budget = 22.3
* Radio Budget = 32.3
* Newspaper Budget = 22.4

### Output

Predicted Sales Value

## 📁 Project Structure

```text
Advertising-Sales-Prediction/
│
├── advertise_sales.csv
├── advertise_sales.ipynb
├── evebatch.pkl
├── README.md

```

## 🚀 Future Improvements

* Use multiple regression techniques.
* Compare different machine learning algorithms.
* Hyperparameter tuning.
* Deploy the model using Flask or Streamlit.
* Create an interactive dashboard.

## 📚 Learning Outcomes

Through this project, I learned:

* Data preprocessing techniques
* Exploratory Data Analysis (EDA)
* Correlation analysis
* Linear Regression implementation
* Model evaluation using R² Score
* Model serialization using Joblib
* Sales forecasting using Machine Learning

## 📌 Conclusion

This project demonstrates how machine learning can be used to predict sales based on advertising expenditures. The Linear Regression model successfully identifies the relationship between marketing investments and sales performance, helping businesses make data-driven advertising decisions.

---

**Author:** Suganya Ganesan
**Project:** Advertising Sales Prediction Using Machine Learning 🚀📈
