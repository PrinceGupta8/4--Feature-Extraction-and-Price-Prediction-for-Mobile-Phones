# 📱 Mobile Phone Price Prediction & Feature Insights

Predicting mobile phone prices using machine learning and extracting key business insights from device features. Built as a part of **NextHikes’ Project 4** for a Data Science & AI portfolio.

---

## 🚀 Objective

Develop a machine learning model to estimate mobile phone prices based on technical specifications and extract high-impact features influencing pricing. Deliver actionable business recommendations through EDA, ML modeling, and Tableau visualizations.

---

## 🧠 Workflow Overview

### 1. 📊 Data Exploration
- Load data from Google Sheets.
- Inspect data types, missing values, feature distributions.
- Understand class imbalance and outliers.

### 2. 🧹 Data Preprocessing
- Handle missing values via imputation.
- Detect/treat outliers using IQR/z-score.
- Convert categorical features:
  - One-hot encoding (for nominal)
  - Label encoding (for ordinal)
- Normalize features using `StandardScaler`.

### 3. 🧬 Feature Engineering
- Derive new variables (e.g., price segments).
- Use:
  - Correlation heatmap
  - Mutual Information scores
  - Feature importance from Random Forest
  - Optional: PCA or `SelectKBest`

### 4. 🤖 Model Building
- Split data into train/test sets (e.g., 80/20).
- Algorithms tried:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor ✅
  - Gradient Boosting
- Hyperparameter tuning with `GridSearchCV`.

### 5. 📈 Model Evaluation
- Metrics used:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
  - R² (Coefficient of Determination)
- Cross-validation to ensure robustness.

### 6. 🔍 Feature Importance Analysis
- Visualize top contributing features.
- Business mapping (e.g., RAM, Battery life as major price drivers).

---

## 📊 Tableau Dashboard

> Includes interactive charts for business decision-making:

- Price Segment Distribution
- Feature vs Price Plots
- Brand-wise Pricing Analysis
- Correlation Heatmap
- Model Predictions vs Actuals

📎 **(Optional)** [Link to Tableau Public Dashboard](#)

---

## ✅ Business Insights & Recommendations

- 📌 **Key Drivers:** RAM, Rear Camera, Battery, Brand
- 🎯 **Recommendation 1:** Focus pricing strategy around top features.
- 🎯 **Recommendation 2:** Bundle RAM + Storage + Battery for mid-range models.
- 🎯 **Recommendation 3:** Use feature differentiation for competitive positioning.

---

## 🧾 Repo Contents

| File/Folder             | Description                                               |
|-------------------------|-----------------------------------------------------------|
| `Mobile_Price_Prediction.ipynb` | Jupyter Notebook with EDA, modeling & visualizations |
| `requirements.txt`      | Python dependencies                                       |
| `README.md`             | Project summary and documentation                         |
| `data/mobile_phones.csv`| Cleaned dataset used for training                         |
| `Tableau_Screenshots/`  | Exported plots from Tableau dashboard                     |
| `models/`               | Trained model files (`.pkl`)                              |

---

## 🛠️ Technologies Used

- **Python:** pandas, numpy, seaborn, matplotlib, scikit-learn
- **Visualization:** Tableau Public
- **Modeling:** Random Forest, Regression, GridSearchCV
- **Optional:** Streamlit for app-based demo

---

## 📌 How to Run

```bash
git clone https://github.com/yourusername/mobile-price-prediction.git
cd mobile-price-prediction
pip install -r requirements.txt
jupyter notebook
