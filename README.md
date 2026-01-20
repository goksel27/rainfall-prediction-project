# Rainfall Prediction Classifier 🌧️☀️

This project builds a **binary classification model** to predict whether it will rain **tomorrow** based on historical Australian weather data.

Repo: https://github.com/goksel27/rainfall-prediction-project

---

## ✅ Project Goal
Predict the target variable:

- **RainToday / RainTomorrow** → **Yes / No**

using weather features such as humidity, pressure, temperature, sunshine, etc.

---

## 🧠 What I Implemented

### 1) Data Preparation
- Converted the `Date` column into a **Season** feature
- Removed unnecessary columns
- Split the dataset with **stratified train/test split**

### 2) Preprocessing Pipeline
Used `ColumnTransformer` to handle mixed feature types:

- **Numerical features** → `StandardScaler`
- **Categorical features** → `OneHotEncoder`

### 3) Model Training
Trained and compared two models:

- **Random Forest Classifier**
- **Logistic Regression**

### 4) Hyperparameter Optimization
For Random Forest, applied:

- `GridSearchCV`
- `StratifiedKFold`

to tune key parameters like:

- `n_estimators`
- `max_depth`
- `min_samples_split`

### 5) Evaluation
Evaluated models using:

- Test set score
- Classification report
- Confusion matrix
- Feature importances (for Random Forest)

---

## 🛠️ Tech Stack
- Python
- Jupyter Notebook
- scikit-learn
- pandas
- matplotlib

---

## 📂 Files
- `FinalProject_AUSWeather.ipynb` → full notebook solution
- `README.md` → project documentation

---

## 🚀 How to Run
1. Clone the repository:
```bash
git clone https://github.com/goksel27/rainfall-prediction-project.git
cd rainfall-prediction-project

Open the notebook:

jupyter notebook


Run all cells in:
FinalProject_AUSWeather.ipynb

📌 Notes

This project was completed as part of an applied Machine Learning lab, focusing on:

real-world preprocessing,

pipeline-based training,

cross-validation tuning,

and model comparison.
