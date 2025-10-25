# 🪙 Crypto and Gold Price Analysis with Machine Learning (2015–2025)

### 🎯 Project Overview
This project analyzes the prices of **Bitcoin, Ethereum, Binance Coin, Ripple, Cardano, Dogecoin, Solana**, and **Gold (USD/oz)** between **2015–2025**, applying **machine learning algorithms** to predict short-term price direction (increase or decrease).  
The main objective is to explore whether cryptocurrencies can be regarded as *digital gold* and to evaluate the performance of classical machine learning models on financial time series data.

---

## 📊 Dataset Information
**Source:** [Kaggle – Crypto and Gold Prices Dataset (2015–2025)](https://www.kaggle.com/datasets/muhamedumarjamil/crypto-and-gold-prices-dataset-20152025)

| Feature | Description |
|----------|--------------|
| **Period** | January 2015 – January 2025 |
| **Assets** | Bitcoin, Ethereum, BNB, XRP, ADA, DOGE, SOL, Gold |
| **Frequency** | Daily closing price |
| **Target Variable** | Next day price direction → 1 (Increase), 0 (Decrease) |

---

## 🧠 Applied Machine Learning Models
1. **Logistic Regression**  
2. **K-Nearest Neighbors (KNN)**  
3. **Support Vector Machine (SVM, RBF Kernel)**  
4. **Random Forest Classifier**

All models were trained and tested over the same features and time intervals to ensure a fair comparison.

---

## ⚙️ Feature Engineering
Technical indicators derived from the dataset:

| Feature | Description |
|----------|--------------|
| `ret_1d` | Daily return |
| `ret_7d` | 7-day average return |
| `vol_7d` | 7-day volatility (standard deviation) |
| `ma30_dev` | Deviation from 30-day moving average |
| `mom_10` | 10-day momentum indicator |

These indicators reflect both short-term trend and volatility dynamics, providing predictive signals for market movements.

---

## 🧩 Code Workflow
1. Load and clean the dataset  
2. Generate technical features and binary labels  
3. Split data into Train/Test sets (2015–2021 → Train, 2022–2025 → Test)  
4. Train each model on the same features  
5. Evaluate performance using accuracy and confusion matrix  
6. Visualize results (Heatmap, Feature Importance, Model Comparison)

---

## 📈 Results
| Model | BTC | ETH | GOLD | BNB |
|--------|-----|-----|------|-----|
| Logistic Regression | 0.68 | 0.68 | 0.68 | 0.68 |
| KNN | 0.66 | 0.66 | 0.66 | 0.66 |
| SVM | 0.68 | 0.68 | 0.68 | 0.68 |
| Random Forest | 0.65 | 0.65 | 0.65 | 0.65 |

- **Highest accuracy:** Logistic Regression & SVM (~68%)  
- **Most balanced model:** Random Forest  
- All models perform better on *upward movements* while struggling with *downward predictions.*

---

## 💡 Key Insights
- Compared to gold, cryptocurrencies exhibit **higher volatility** but **greater return potential.**  
- Even with simple features, ML models can successfully capture short-term momentum.  
- Model comparisons help investors better understand the **risk–return balance** between digital and traditional assets.

---

## 🚀 Future Improvements
- Apply **deep learning models** (LSTM, GRU, Prophet) for advanced time-series forecasting  
- Incorporate **macroeconomic variables** (inflation, interest rate, money supply, etc.)  
- Extend to multi-currency comparison (USD, EUR, TRY)

---

## 👨‍💻 Author
**Yunus Ahmet Dokazoğlu**  
📍 Ankara, Türkiye  
🔗 [GitHub Profile](https://github.com/AhmetDokazoglu)  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/ahmet-dokazo%C4%9Flu-9660b2346/)

---

## 📎 Additional Documents  
📄 [Download Full Project Report (Word Version)](https://github.com/AhmetDokazoglu/Crypto-and-Gold-Price-Analysis-ML/raw/refs/heads/main/Kripto%20ve%20Alt%C4%B1n%20Fiyatlar%C4%B1n%C4%B1n%20Analizi%20ve%20Makine%20%C3%96%C4%9Frenmesi%20ile%20%C3%96ng%C3%B6r%C3%BCs%C3%BC.docx)
