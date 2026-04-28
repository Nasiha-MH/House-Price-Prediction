# House Price Prediction | End-to-End Machine Learning Project

## Project Summary
A machine learning project that predicts residential house sale prices using scikit-learn and the Kaggle House Prices dataset. Built with Linear Regression on six core features, with clean preprocessing and clear evaluation metrics.


## Business Problem

Accurately estimating house prices is critical for:

* Real estate platforms (price recommendations)
* Buyers & sellers (fair valuation)
* Financial institutions (loan risk assessment)

**Goal:** Predict `SalePrice` using property features and evaluate model reliability.

---

## Dataset

* Source: Kaggle
* Dataset: House Prices - Advanced Regression Techniques
* ~1,400+ records, 80+ features (mixed numeric + categorical)

---

## Key Features Used

Focused on high-signal variables:

* **GrLivArea** – Living area (sqft)
* **OverallQual** – Construction & finish quality
* **LotArea** – Land size
* **YearBuilt** – Property age
* **BedroomAbvGr**, **FullBath**

*(Extended version can include GarageArea, TotalBsmtSF, Neighborhood)*

---

## Tech Stack

* Python, Pandas, NumPy
* Matplotlib
* Scikit-learn


## Methodology

### 1) Data Preparation

* Selected high-impact features
* Handled missing values (median imputation)
* Applied **feature scaling** (StandardScaler)

### 2) Modelling

* **Baseline:** Linear Regression
* **Improved:** Gradient Boosting Regressor *(captures non-linearity)*

### 3) Evaluation

* **MAE** (Mean Absolute Error)
* **RMSE** (Root Mean Squared Error)
* Visual validation using **Actual vs Predicted scatter plot**

---

## Results & Insights

* Model captures **overall price trends effectively**
* **Mid-range properties** predicted with good accuracy
* **High-value homes** show larger error → indicates non-linear effects & missing features
* Gradient Boosting improves performance over Linear Regression

> Insight: Property quality and living area have stronger influence than basic counts (bedrooms/bathrooms).

---

## Limitations

* Limited feature set (not using full dataset)
* Minimal categorical encoding
* No hyperparameter tuning
* External factors (location demand, market trends) not included

---

## Future Improvements

* Add **categorical encoding** (e.g., Neighborhood)
* Apply **log transformation** to handle skewed prices
* Perform **hyperparameter tuning**
* Experiment with **Random Forest / XGBoost**
* Deploy model via **Flask / Streamlit**

---

## Skills Demonstrated

* Data Cleaning & Preprocessing
* Feature Selection & Scaling
* Regression Modelling
* Model Evaluation (MAE, RMSE)
* Data Visualization & Insight Extraction

---

## Sample Output

Actual vs Predicted Prices.png

---

## How to Run

```bash
pip install -r requirements.txt
python main.py
```

---


BS Computer Science | Aspiring Data Scientist
📌 Open to internships & entry-level roles in Data Science / ML
