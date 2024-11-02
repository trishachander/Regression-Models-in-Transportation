# 🚌 Bus Arrival Delay Prediction using XGBoost

## 📚 Course Information
- **Course**: AH2179
- **Module**: 2
- **Project**: XGBoost Regression Model for Bus Arrival Delay Prediction

## 🎯 Project Overview
This project implements an XGBoost regression model to predict bus arrival delays, utilizing GridSearchCV for hyperparameter optimization and comprehensive feature engineering techniques.

## 🏗️ Model Architecture
### Data Preprocessing
- **Dropped Features**: 'Arrival_time', 'Stop_id', 'Bus_id', 'Line_id'
- **Feature Scaling**: StandardScaler implementation
- **Data Split**: 80% training, 20% testing
- **Cross-Validation**: 5-fold KFold

### 🔧 Hyperparameter Search Space
GridSearchCV explored the following parameters:
- min_child_weight
- gamma
- subsample
- colsample_bytree
- max_depth
- objective functions:
  - reg:squarederror
  - reg:squaredlogerror
  - reg:logistic

## ⭐ Best Model Configuration
Optimized XGBoost parameters:
- **colsample_bytree**: 1
- **gamma**: 1.5
- **max_depth**: 15
- **min_child_weight**: 1
- **objective**: 'reg:squarederror'
- **subsample**: 0.6

## 📊 Model Performance
- **Mean Absolute Error**: 9.1804
- **Mean Squared Error**: 12.9618
- **R-squared Score**: 0.9932

  ![image](https://github.com/user-attachments/assets/024e2c56-8a33-4436-a6d7-49de26c77fe3)


## 💡 Key Findings
- XGBoost's ensemble approach proved highly effective for delay prediction
- GridSearchCV significantly streamlined hyperparameter optimization
- Model showed strong resistance to overfitting
- Sequential tree predictions enhanced accuracy

## 🔮 Applications & Future Work
The model architecture can be adapted for various transportation scenarios:
- 🔌 EV charging station selection (classification)
- 🚗 Traffic congestion prediction
- 🛑 Route optimization
- 📱 Real-time delay notifications

## 🛠️ Dependencies
- XGBoost
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

---
*Note: This project was completed as part of the AH2179 course, Module 2.* 🎓
