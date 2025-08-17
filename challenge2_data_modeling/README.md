# Challenge 2: Data Modeling – Airbnb Price Prediction & Investment Strategy

## 🎯 Objective
Build a predictive model using **tidymodels + XGBoost** to estimate Airbnb listing prices, evaluate performance, and design a **real estate investment strategy** with a €3M budget.

---

## 🛠️ Modeling Workflow
1. **Data Preparation**
   - Clean column names  
   - Train/test split (75/25)  
   - 10-fold cross-validation (stratified by neighborhood)  

2. **Preprocessing Recipe**
   - One-hot encoding for categorical variables  
   - Boolean conversion for features like `host_is_superhost`  
   - Median/mode imputation for missing values  
   - Remove near-zero variance & correlated predictors  

3. **Model**
   - Algorithm: XGBoost regression  
   - Hyperparameters tuned (trees, learning rate, depth, min_n, sample size)  
   - Evaluation metrics: RMSE, MAE, R², MAPE  

4. **Evaluation**
   - Predictions align well for mid-range prices  
   - Higher variance for expensive listings  
   - Leaflet map shows mostly low errors (green markers), with localized anomalies  

---

## 📊 Business Insights
- **Prediction Accuracy**: Strong model performance for most listings.  
- **Neighborhood Variance**: Higher errors in Gracia, Eixample, and Nou Barris.  
- **Investment ROI**:  
  - **Best ROI neighborhoods**: Sants-Montjuïc (7.2%), Nou Barris (6.6%).  
  - **Worst ROI neighborhoods**: Sarria-Sant Gervasi, Les Corts (<2.5%).  

---

## 💰 Investment Strategy (with €3M budget)
### Risky Portfolio (Diversified)
- Spread across **Sants-Montjuïc, Nou Barris, Sant Andreu, Eixample, Ciutat Vella**  
- Higher risk but better upside due to diversification.  

### Less Risky Portfolio (Focused)
- Concentrated in **Sants-Montjuïc & Nou Barris**  
- Stable returns, faster payback (~14–15 years).  
