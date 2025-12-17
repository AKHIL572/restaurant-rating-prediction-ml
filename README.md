# 🍽️ Restaurant Rating Prediction – End-to-End Machine Learning Project

## 📌 Project Overview
This project builds an **end-to-end machine learning system** to predict **restaurant aggregate ratings** based on operational, location, pricing, and service-related features.

The project follows **industry-standard data science practices**, covering:
- Data cleaning & preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training & comparison
- Cross-validation & hyperparameter tuning
- Model interpretation & business insights

The final solution uses a **tuned Gradient Boosting Regressor**, achieving strong predictive performance and interpretable insights.

---

## 🎯 Business Objective
Restaurant ratings influence:
- Customer trust
- Online visibility
- Revenue & conversions

**Goal:**  
Predict restaurant ratings and identify **key factors that drive higher ratings**, enabling data-driven business decisions.

---

## 🛠️ Tech Stack
- **Programming:** Python  
- **Libraries:**  
  - Data Handling: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Machine Learning: `scikit-learn`  
  - Model Persistence: `joblib`  

---

## 📁 Project Structure

Restaurant-Rating-Prediction/
│
├── data/
│ ├── Res_dataset.csv
│ ├── Cleaned_dataset.csv
│ └── Updates_dataset.csv
│
├── notebooks/
│ ├── 01_data_cleaning.ipynb
│ ├── 02_eda_outliers.ipynb
│ ├── 03_modeling.ipynb
│ └── 04_business_insights.ipynb
│
├── models/
│ └── final_gradient_boosting_model.pkl
│
├── README.md
└── .gitignore


---

## 🔄 Project Workflow

### 1️⃣ Data Cleaning & Preprocessing
- Removed duplicates
- Handled missing values
- Converted categorical Yes/No columns into numerical format
- Saved cleaned dataset for reproducibility

### 2️⃣ Exploratory Data Analysis (EDA)
- Rating distribution analysis
- City & country-wise restaurant distribution
- Cuisine popularity analysis
- Outlier detection using IQR
- Correlation analysis

### 3️⃣ Feature Engineering
- Cuisine count per restaurant
- Cost category derived from price range
- One-hot encoding for categorical variables
- Leakage prevention (excluded target-derived features)

### 4️⃣ Model Building & Evaluation
Models evaluated:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

Evaluation metrics:
- MSE
- MAE
- RMSE
- R² Score

---

## 📊 Model Performance (Cross-Validation)

| Model | Mean CV R² | Std CV R² |
|------|------------|-----------|
| Linear Regression | 0.38 | 0.26 |
| Decision Tree | 0.91 | 0.01 |
| Random Forest | 0.95 | 0.00 |
| Gradient Boosting | 0.95 | 0.00 |

📌 **Insight:**  
Tree-based models significantly outperform linear regression, indicating **strong non-linear relationships** in the data.

---

## 🔧 Hyperparameter Tuning
- Used **RandomizedSearchCV** on Gradient Boosting
- Optimized parameters:
  - `n_estimators`
  - `learning_rate`
  - `max_depth`
  - `subsample`

### ✅ Final Model
- **Model:** Tuned Gradient Boosting Regressor
- **Final R² Score:** ~0.95
- Model saved using `joblib`

---

## 🔍 Model Interpretability
- Feature importance analysis
- Identified key drivers influencing restaurant ratings
- Grouped feature importance for high-level insights

---

## 📈 Business Insights
- Restaurants offering **online delivery** tend to have higher ratings
- **Table booking availability** correlates with better customer ratings
- Higher **price ranges** generally receive higher and more consistent ratings
- Cuisine diversity and customer votes strongly influence ratings

---

## 🚀 Key Takeaways
- End-to-end ML pipeline following industry best practices
- Strong model performance with cross-validation
- Clear business-focused insights, not just predictions
- Reproducible and production-ready workflow

---

## 📌 Future Improvements
- Deploy model using Flask / FastAPI
- Create an interactive dashboard (Power BI / Tableau)
- Integrate SHAP for deeper explainability
- Add real-time prediction interface

---

## 👤 Author
**Akhil T V**  
Aspiring Data Scientist  
📫 *Open to Data Science & Machine Learning roles*

---

⭐ If you find this project useful, feel free to star the repository!
