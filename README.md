# upskillcampus

## 📌 Overview

This repository contains two real-world machine learning projects completed as part of an Industrial Internship conducted by Upskill Campus in collaboration with UniConverge Technologies Pvt. Ltd. (UCT).

The projects focus on solving industrial problems using data-driven approaches, including predictive maintenance and process optimization.

---

## 📂 Project Structure
industrial-ml-internship/
│
├── datasets/
│ ├── turbofan/
│ └── mining_quality/
│
├── notebooks/
│ ├── turbofan_rul.ipynb
│ └── mining_quality.ipynb
│
├── results/
│
└── README.md

---

# 🚀 Project 1: Turbofan Engine RUL Prediction

## 📌 Objective

To predict the Remaining Useful Life (RUL) of turbofan engines using multivariate sensor data.

---

## 📊 Dataset Description

- Time-series sensor data from multiple engines  
- Each engine operates until failure  
- Includes 21 sensor readings and 3 operational settings  

---

## ⚙️ Approach

- Data preprocessing and cleaning  
- Creation of RUL target variable  
- Engine-wise data splitting (to avoid data leakage)  
- Feature scaling using StandardScaler  
- Model training using Random Forest  

---

## 🔑 Key Techniques

- Time-series aware splitting  
- RUL clipping (max = 130 cycles)  
- Feature selection  
- Model evaluation using Mean Squared Error (MSE)  

---

## 📈 Results

| Metric | Value |
|-------|------|
| Train MSE | ~200 |
| Test MSE | ~411 |

---

## 💡 Insights

- Certain sensors significantly impact engine degradation  
- Proper data splitting is crucial in time-series problems  
- Model generalization improved after preventing data leakage  

---

# ⚙️ Project 2: Mining Process Quality Prediction

## 📌 Objective

To predict the percentage of silica (% Silica Concentrate) in a mining flotation process.

---

## 📊 Dataset Description

- Real industrial process data  
- Includes variables such as air flow, pulp levels, and chemical inputs  
- Contains time-based measurements  

---

## ⚙️ Approach

- Data cleaning and preprocessing  
- Handling missing values  
- Removal of non-numeric and irrelevant columns  
- Conversion of string values to numeric  
- Removal of highly correlated features (% Iron Concentrate)  

---

## 🔑 Key Techniques

- Feature scaling  
- Data leakage prevention  
- Random Forest regression  
- Model evaluation using MSE  

---

## 📈 Results

| Metric | Value |
|-------|------|
| Train MSE | ~0.008 |
| Test MSE | ~0.049 |

---

## 💡 Insights

- Certain process variables strongly influence silica levels  
- Removing correlated features improves model reliability  
- Model can assist engineers in real-time decision making  

---

# 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

# 📚 Key Learnings

- Handling real-world industrial datasets  
- Time-series modeling techniques  
- Feature engineering and preprocessing  
- Avoiding data leakage  
- Model evaluation and optimization  

---

# 🔮 Future Work

- Implement deep learning models (LSTM) for time-series prediction  
- Deploy models using Flask or Streamlit  
- Integrate real-time industrial data streams  

---

# 👤 Author

**Sriram S**

---

# 🎯 Conclusion

These projects demonstrate the application of machine learning in industrial environments, focusing on predictive maintenance and process optimization. The solutions developed are scalable and can be extended for real-time deployment.