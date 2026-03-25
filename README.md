# ✈️ Air Freight Demand Forecasting using ANN

## 🧠 Overview
This project focuses on forecasting air freight demand using historical time-series data and an Artificial Neural Network (ANN).  
The model is trained on real-world freight data (2017–2023) to predict future demand patterns and support logistics decision-making.

---

## 🎯 Problem Statement
Air freight plays a critical role in global trade, with demand influenced by seasonality, economic conditions, and unexpected disruptions such as pandemics.

Traditional forecasting methods often fail to capture complex patterns in demand.  
This project aims to build a machine learning model that can accurately predict future air freight demand using historical data.

---

## 📊 Dataset
- Time Range: 2017 – 2023  
- Records: **3,104 rows, 6 columns**  
- Type: Daily time-series data  
- Domain: Air freight data across Indian airports

---

## ⚙️ Tech Stack
- Python  
- Pandas, NumPy  
- TensorFlow / Keras  
- Scikit-learn  
- Matplotlib  

---

## 🔄 Project Workflow
1. Data Cleaning & Preprocessing  
2. Feature Engineering  
   - Extracted year, month, day  
   - Lag features (previous day demand)  
   - Rolling mean (3-day average)  
3. Data Scaling (StandardScaler)  
4. Model Building (ANN)  
5. Model Evaluation (MAE, RMSE)  
6. Forecasting  

---

## 🧠 Model Details
- Model: Artificial Neural Network (ANN)  
- Architecture:
  - Dense (64, ReLU) + Dropout (0.2)  
  - Dense (32)  
  - Output layer (1 neuron)  
- Optimizer: Adam  
- Loss Function: Mean Squared Error (MSE)  
- Epochs: 100 | Batch Size: 16 

---

## 📊 Results
- **MAE:** 6,510.72  
- **RMSE:** 9,541.02 

👉 Actual freight volume range: 150,000 – 200,000  
👉 Prediction error: ~3–6% 

The model successfully captured:
- Seasonal trends  
- Short-term fluctuations  
- Demand patterns over time  

---

## 📈 Visual Output
(Add your graph here)

Example:
![Actual vs Predicted](outputs/forecast.png)

👉 The model predictions closely follow actual demand trends, showing strong generalization ability. :contentReference[oaicite:3]{index=3}  

---

## 💡 Business Impact

### Before:
- Limited visibility into future freight demand  
- Reactive decision-making  
- Risk of over/under-utilization of logistics resources  

### After:
- Data-driven demand forecasting  
- Improved capacity planning for airlines and airports  
- Better resource allocation (fleet, storage, operations)  
- Reduced operational inefficiencies  

### Key Value:
- Supports **strategic planning and cost optimization**  
- Helps companies prepare for demand fluctuations  
- Enables **proactive logistics management** :contentReference[oaicite:4]{index=4}  

---

## 🚀 Future Improvements
- Use LSTM / advanced deep learning models  
- Add external factors (weather, economic indicators)  
- Deploy model using Flask API  
- Integrate real-time forecasting  

---

## 📚 Key Learnings
- Time-series forecasting using ANN  
- Feature engineering for sequential data  
- Model evaluation using MAE and RMSE  
- Understanding real-world logistics problems  

---

## 📌 Conclusion
The ANN model demonstrated strong performance in forecasting air freight demand.  
It provides a reliable and scalable approach for improving decision-making in logistics and transportation systems.
