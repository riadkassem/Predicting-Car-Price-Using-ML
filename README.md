# Car Price Prediction with Ridge Regression 🚗💻

This project explores a **machine learning pipeline** to predict car prices using Ridge Regression, with comprehensive data preprocessing, hyperparameter tuning, and model evaluation.

## Key Features
- **Data Preprocessing**: Handles missing values, categorical encoding (OneHotEncoder), and feature scaling.
- **Model Comparison**: Tests Ridge, SVR, and RandomForestRegressor.
- **Hyperparameter Tuning**: Uses `RandomizedSearchCV` to optimize Ridge Regression.
- **Metrics**: Evaluates performance with **R², MAE, and MSE**.

## Results
| Model                | R² Score   | MAE      | MSE          |
|----------------------|------------|----------|--------------|
| Ridge (Baseline)     | 0.2540     | 5,713.82 | 49,950,182.63|
| Ridge (Tuned)        | **0.2557** | -        | -            |
| RandomForest         | 0.2149     | -        | -            |

## How to Use
1. **Install Dependencies**:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn

2. **Run the Notebook**:
    ```bash
    jupyter notebook car_sales.ipynb

# Car Price Prediction Dataset and Future Improvements

## Dataset
- **Columns**: 
  - `Make` 
  - `Colour` 
  - `Odometer (KM)` 
  - `Doors` 
  - `Price`
  
- **Missing Values Handling**:
  - Numeric features: Imputed with median
  - Categorical features: Imputed with constant values

## Future Improvements
1. **Model Enhancements**:
   - Implement non-linear models:
     - Gradient Boosting
     - XGBoost

2. **Feature Engineering**:
   - Create mileage bins (Low/Medium/High)
   - Add brand-country mappings

3. **Deployment**:
   - Develop Flask API for real-time price predictions

## Note
- Replace placeholder file paths (e.g., `data/car_sales.csv`) with your actual dataset location
