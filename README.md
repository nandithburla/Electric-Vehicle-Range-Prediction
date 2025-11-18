# 🚗⚡ Electric Vehicle Range Prediction  
_End-to-End Machine Learning & Power BI Project_

![Python](https://img.shields.io/badge/Python-3.x-blue)
![PowerBI](https://img.shields.io/badge/Power%20BI-Analytics-yellow)
![Machine Learning](https://img.shields.io/badge/ML-Regression-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## 📌 Overview
This project builds a complete **Electric Vehicle Range Prediction** pipeline using Python and Power BI.  
It includes data preprocessing, in-depth EDA, feature engineering, and a **Random Forest Regressor (R² = 0.978)** to accurately predict EV driving range.  
A Power BI dashboard visualizes results, trends, and model insights.

---

## 🎯 Objectives
- Predict the **electric vehicle driving range** using machine learning.
- Perform **EDA** to identify the key factors affecting EV range.
- Clean and preprocess **100K+ EV data records**.
- Build an interactive **Power BI dashboard** for insights.
- Export prediction results for BI tools.

---

## 🧰 Tech Stack

### Languages & Tools
- Python  
- Jupyter Notebook  
- Power BI  
- Excel / CSV

### Python Libraries
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 📂 Project Structure
```bash
📦 Electric-Vehicle-Range-Prediction/
│
├── EV_Range_Prediction_Final_Workflow.ipynb     # Main ML workflow
├── ElectricVehicle.ipynb                        # Additional EDA
├── cleanedprojectdataset.xlsx                   # Cleaned dataset
├── EV_Range_Predictions_For_PowerBI.csv         # Predictions for BI
├── REPORT.pdf                                   # Detailed project report
├── README.md                                    # Documentation
└── PowerBI Dashboard/                           # PBIX or screenshots
````

---

## 🔍 Exploratory Data Analysis (EDA)

Performed using Python with visualizations such as:

* EV type distribution
* Base MSRP vs Range
* City-level EV density
* Correlation heatmap
* Boxplots & outlier removal using **IQR**
* Manufacturer-level insights

---

## 🤖 Machine Learning Workflow

### 1️⃣ Data Preprocessing

* Cleaned missing values
* Removed outliers
* Label encoding + One-hot encoding
* Created **Vehicle Age** feature
* Combined City & State into a **location** attribute

### 2️⃣ Model Used

**Random Forest Regressor**

### 3️⃣ Train-Test Split

```python
X_train, X_test, y_train, y_test = train_test_split(
    X_encoded, y, test_size=0.2, random_state=42
)
```

### 4️⃣ Model Training

```python
model = RandomForestRegressor(random_state=42)
model.fit(X_train, y_train)
```

### 5️⃣ Evaluation

* **R² Score:** 0.978
* **Mean Absolute Error (MAE)** printed in notebook

### 6️⃣ Export Predictions

```python
df_results = X_test.copy()
df_results['Actual Range'] = y_test
df_results['Predicted Range'] = y_pred
df_results.to_csv("EV_Range_Predictions_For_PowerBI.csv", index=False)
```

---

## 📊 Power BI Dashboard

The Power BI dashboard includes:

* EV range distribution
* Actual vs Predicted comparison
* Insights across Make, Model, EV Type
* City & State level trends
* Interactive slicers

---

## 📈 Results

* Achieved **0.978 R² score** using Random Forest
* Improved accuracy using outlier removal
* Identified top features impacting EV range
* Delivered a visually rich Power BI dashboard

---

## 📬 Author

**Nandith Burla**
B.Tech — Data Science & Engineering
#### GitHub: [https://github.com/nandithburla](https://github.com/nandithburla)
#### LinkedIn: [https://www.linkedin.com/in/nandithburla/](https://www.linkedin.com/in/nandithburla/)

---


