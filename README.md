# Energy Consumption Forecasting

This project focuses on predicting future energy consumption using supervised machine learning techniques combined with time series analysis. The goal is to model energy usage trends and generate accurate forecasts using four different algorithms: **Support Vector Machine (SVM)**, **Random Forest**, **Linear Regression**, and **Decision Tree Regression**.

---

## Objective

To analyze and forecast future energy consumption based on historical data using various regression models and time series techniques. The project helps in identifying usage patterns and making data-driven predictions for efficient energy planning and resource optimization.

---

## Tech Stack

- **Python 3.x**
- **Pandas**, **NumPy** for data handling
- **Matplotlib**, **Seaborn** for data visualization
- **scikit-learn** for machine learning models
- **Statsmodels** for time series preprocessing and analysis

---

## Machine Learning Models Used

| Model                 | Description |
|----------------------|-------------|
| **Linear Regression** | A baseline model for capturing linear trends in energy data |
| **Decision Tree**     | Captures non-linear relationships and patterns |
| **Random Forest**     | An ensemble model for reducing overfitting and improving accuracy |
| **Support Vector Machine (SVM)** | Provides robust regression by maximizing the margin |

Each model was trained and evaluated independently on the same preprocessed dataset.

---

## Time Series Analysis

- Used lag features, rolling statistics, and time-based decomposition
- Analyzed seasonality, trend, and residuals
- Feature engineering based on **hour, day, week, month**, and **holidays/weekends**

---

## Features Considered

- Timestamp (converted to datetime)
- Hourly/daily energy consumption
- Weather conditions (optional)
- Lagged energy usage values
- Rolling means (e.g., 3-hour, 6-hour, 24-hour)

---

## Evaluation Metrics

| Metric           | Description                            |
|------------------|----------------------------------------|
| **MAE**          | Mean Absolute Error                    |
| **RMSE**         | Root Mean Square Error                 |
| **R² Score**     | Coefficient of determination           |

Models were evaluated using both **train-test split** and **cross-validation**.

---

## Project Workflow

1. **Data Preprocessing**:
   - Handled missing values and outliers
   - Extracted time-based features
   - Normalized input variables

2. **Exploratory Data Analysis (EDA)**:
   - Plotted seasonal and trend components
   - Visualized consumption patterns by day/week

3. **Model Training**:
   - Trained each model using historical data
   - Performed hyperparameter tuning (GridSearchCV where applicable)

4. **Forecasting**:
   - Predicted short-term consumption (e.g., next 24-72 hours)
   - Compared actual vs predicted values for each model

---

## ⚙️ How to Run

### Requirements:
- Python 3.7+
- Libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
