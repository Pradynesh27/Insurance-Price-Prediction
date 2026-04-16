# Insurance-Price-Prediction
# Health Insurance Price Prediction

This project aims to predict the medical insurance costs of individuals based on several factors such as age, BMI, smoking status, and more. By leveraging machine learning regression techniques, we can provide accurate cost estimates for both providers and consumers.

##  Key Results
* **Best Model:** Tuned XGBoost Regressor
* **Accuracy ($R^2$ Score):** 0.8599
* **Mean Absolute Error (MAE):** 2590.49
* **Key Findings:** Smoking status and BMI were the most significant predictors of insurance charges.

##  Dataset Features
The dataset contains 1,338 records with the following attributes:
- **Age:** Age of the primary beneficiary.
- **Sex:** Insurance contractor gender (female/male).
- **BMI:** Body Mass Index ($kg/m^2$).
- **Children:** Number of children covered by health insurance.
- **Smoker:** Smoking status (yes/no).
- **Region:** The beneficiary's residential area in the US.
- **Charges:** Individual medical costs billed by health insurance (Target).

##  Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn, XGBoost
- **Optimization:** RandomizedSearchCV, Cross-Validation

##  Project Workflow
1. **Exploratory Data Analysis (EDA):** Visualized feature distributions and correlations.
2. **Data Preprocessing:** - Handled categorical variables using Label Encoding.
   - Standardized features using `StandardScaler`.
   - Addressed outliers in BMI and Charges.
3. **Model Development:** Evaluated multiple models including:
   - Linear Regression
   - Decision Tree Regressor
   - Random Forest Regressor
   - XGBoost Regressor
4. **Hyperparameter Tuning:** Optimized XGBoost and Random Forest using `RandomizedSearchCV` (5-fold cross-validation) to prevent overfitting.
5. **Evaluation:** Compared models using MAE, MSE, RMSE, and $R^2$ scores.

## 🏁 Conclusion
The Tuned XGBoost model outperformed other algorithms, demonstrating its ability to handle non-linear relationships and complex feature interactions effectively.
