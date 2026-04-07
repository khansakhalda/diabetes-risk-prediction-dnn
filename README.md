# 🩺 Diabetes Risk Prediction using Deep Neural Network

This project focuses on predicting diabetes risk using a Deep Neural Network (DNN) based on patient clinical data such as age, BMI, blood glucose level, and other health indicators.

Diabetes is a serious chronic disease that requires early detection. This project aims to support preventive healthcare by providing an accurate and data-driven prediction model.

---

## 📌 Background

Diabetes is one of the most common chronic diseases worldwide and can lead to severe complications if not detected early. Many patients remain undiagnosed until the condition becomes critical.

With the availability of healthcare data, machine learning and deep learning techniques can be applied to identify patterns and predict the likelihood of diabetes, enabling early screening and better decision-making.

---

## 🎯 Objectives

This project aims to:

* Predict whether a patient is at risk of diabetes (classification task)
* Develop a Deep Neural Network model for accurate prediction
* Handle class imbalance to improve detection of diabetes cases
* Analyze feature importance to understand key influencing factors

---

## ⚙️ Process

### 1. Data Collection

* Dataset: Diabetes Prediction Dataset
* Source: Kaggle
* Total data: **100,000 records**

---

### 2. Data Preprocessing

* Handling missing values
* Normalizing column names
* Encoding categorical variables:

  * Gender → binary encoding
  * Smoking history → one-hot encoding
* Removing inconsistencies and ensuring clean dataset

---

### 3. Feature Engineering

* Conversion of categorical variables into numerical format
* Feature scaling using **StandardScaler**
* Selection of relevant clinical features

---

### 4. Exploratory Data Analysis (EDA)

* Analysis of data distribution
* Class imbalance identification

📌 Insight:

* **91.5% non-diabetes vs 8.5% diabetes** → highly imbalanced dataset

---

## 🤖 Model Development

### 🔹 Deep Neural Network (DNN)

Architecture:

* Dense (128) + ReLU + Dropout (0.4)
* Dense (64) + ReLU + Dropout (0.3)
* Dense (32) + ReLU + Dropout (0.2)
* Output layer (Sigmoid)

Techniques used:

* **Class Weighting** → handle imbalance
* **Early Stopping** → prevent overfitting
* Optimizer: Adam

---

## 📊 Model Evaluation

### ✅ Model Performance:

* **Accuracy: ~91%**
* **Recall (Diabetes): ~90%**
* **Precision (Diabetes): ~47%**
* **ROC-AUC Score: 0.976**

📌 Key Point:

* Model has **high recall**, meaning it successfully detects most diabetes cases
* Suitable for **medical screening**, where missing a positive case is critical

---

## 📊 Final Results & Insights

* The DNN model successfully learns patterns from clinical data
* Strong performance in distinguishing diabetes vs non-diabetes
* Class weighting significantly improves minority class detection
* The model is more sensitive to detecting diabetes cases than standard models

📌 Example Insight:

* High blood glucose and HbA1c levels strongly indicate diabetes risk

---

## 💡 Key Insights

* **Blood glucose level and HbA1c** are the most influential features
* Age and BMI also contribute significantly to prediction
* Deep learning improves performance compared to traditional methods
* Handling imbalance is crucial in medical datasets

---

## 🔍 Model Interpretability (SHAP)

SHAP analysis was used to interpret the model predictions:

* High **HbA1c_level** → increases probability of diabetes
* High **blood_glucose_level** → strong predictor
* Moderate influence: Age & BMI
* Low influence: Gender, smoking history

This improves trust and transparency in model decisions.

---

## 🛠️ Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib
* SHAP

---

## 👩‍💻 Author

**Khansa Khalda**  
Data Science Project<br>
Jenderal Soedirman University
