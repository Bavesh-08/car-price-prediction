### 🚗 Car Price Prediction 

## 📌 Project Overview
This project applies Machine Learning regression models to predict the **price of cars** based on various technical specifications and features (e.g., horsepower, engine size, fuel type, car body). 

## 📊 Dataset Description
* **Total Samples:** 205 cars 
* **Features:** 26 features (mix of numerical and categorical data)
* **Target Variable:** `price` (Continuous variable)
* **Data Quality:** Clean dataset with **0 missing values**.

## 🛠️ Tech Stack & Dependencies
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn` (Linear Regression, Lasso Regression, Random Forest Regressor)
* **Data Preprocessing:** `StandardScaler`, `LabelEncoder`

## 🚀 Workflow Methodology
1. **Data Loading & EDA:** Visualized numerical distributions, detected outliers using boxplots, and plotted a correlation heatmap to find relationships between features.
2. **Data Preprocessing (Encoding):** Converted categorical text data (like fuel type, car body, etc.) into numerical formats using `LabelEncoder`.
3. **Feature Scaling:** Applied `StandardScaler` to normalize the feature set so that no single feature dominates the model due to its scale.
4. **Data Splitting:** Split the data into **90% Training** and **10% Testing** sets.
5. **Model Training & Evaluation:** Trained three regression models and evaluated them using the **R² (R-squared) Score** and Actual vs. Predicted scatter plots.

## 📈 Model Performance & Results
The models were evaluated based on their R² scores (closer to 1.0 is better). 

| Model | Training R² Score | Testing R² Score |
| :--- | :--- | :--- |
| **Linear Regression** | 0.897 | 0.901 |
| **Lasso Regression** | 0.897 | 0.901 |
| **Random Forest** | **0.989** | **0.903** |

🏆 **Conclusion:** All three models performed exceptionally well on the test data, explaining about 90% of the variance in car prices. **Random Forest** performed best overall, though it shows signs of slight overfitting on the training data compared to the linear models.

