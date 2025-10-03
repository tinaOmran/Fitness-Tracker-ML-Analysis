# 🏋️‍♀️ Fitness Tracker Sensor Data Analysis & Modeling

This project focuses on analyzing and modeling sensor data collected from fitness trackers using machine learning techniques. It was developed as part of an Artificial Intelligence course at Amirkabir University of Technology.

---

## 📌 Overview

The dataset contains accelerometer and gyroscope readings from participants performing various exercises. The goal is to preprocess the data, explore hidden patterns, and build predictive models to classify activity types and intensities.

---

## 🧠 Key Steps

### 1️⃣ Data Preprocessing  
- Removed irrelevant features (`epoch`, `participants`)  
- Detected and removed outliers using IQR and box plots  
- Cleaned ~3000 noisy records

### 2️⃣ Exploratory Data Analysis (EDA)  
- Visualized distributions with bar charts and box plots  
- Created 3D scatter plots for movement patterns  
- Generated heatmaps to study feature correlations

### 3️⃣ Model Selection & Training  
- Used `lazypredict` to benchmark multiple classifiers  
- Addressed overfitting by adjusting train-test split and removing highly correlated features  
- Final models: `DecisionTreeClassifier`, `RandomForest`, `LGBMClassifier`

### 4️⃣ Evaluation  
- Accuracy scores:  
  - Decision Tree: 0.98  
  - Random Forest: 0.97  
  - LGBM: 0.97  
- Logistic Regression: 0.86 (test), 0.78 (train)  
- Cross-validation score: 0.85

---

## 📊 Dataset Description

- **Source**: [Kaggle – Fitness Tracker Dataset](https://www.kaggle.com/datasets/krishujeniya/fitness-tracker-accelerometer-and-gyroscope-data)  
- **Features**:  
  - Accelerometer (x, y, z)  
  - Gyroscope (x, y, z)  
  - Activity label, intensity category, set ID  
- **Size**: ~9000 records, 11 features

---

## 🛠 Technologies Used

- Python 3.x  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- scikit-learn  
- lazypredict  
- LightGBM

---
## 📚 References

- [Kaggle: Fitness Tracker Dataset](https://www.kaggle.com/datasets/krishujeniya/fitness-tracker-accelerometer-and-gyroscope-data)  
- [LazyPredict Documentation](https://pypi.org/project/lazypredict/)  
- [GeeksforGeeks: Cross-Validation](https://www.geeksforgeeks.org/cross-validation-machine-learning)  
- [Intro to EDA in Python](https://www.kaggle.com/code/imoore/intro-to-exploratory-data-analysis-eda-in-python)  
- [Logistic Regression Guide](https://cafetadris.com/blog/رگرسیون-لجستیک)
