# Credit Card Fraud Detection  

## 📌 Project Overview  
Machine learning model to detect fraudulent credit card transactions using imbalanced data techniques. Achieved **84% recall** with **<1% false positives** on highly skewed data (492 frauds in 284,807 transactions).

## 🔍 Dataset  
- **Source**: European cardholders (September 2013)  
- **Size**: 284,807 transactions (0.172% fraud)  
- **Features**:  
  - V1-V28: PCA-transformed numerical features  
  - `Time`: Seconds elapsed since first transaction  
  - `Amount`: Transaction amount  
  - `Class`: Target variable (1=Fraud, 0=Legitimate)  

## 🛠️ Key Techniques  
- **Data imbalance**: SMOTETomek resampling  
- **Feature scaling**: RobustScaler  
- **Models**: Random Forest, XGBoost, LightGBM  
- **Optimization**: Hyperparameter tuning (GridSearchCV/RandomizedSearchCV)  

## 📊 Results  
| Metric          | Score  |
|-----------------|--------|
| Recall          | 84%    |
| AUC-ROC         | 0.97   |
| F1-Score        | 0.84   |
| False Positives | 11     |
