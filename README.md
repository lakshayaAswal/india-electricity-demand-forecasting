# India Hourly Electricity Demand Forecasting System

## Overview

This project uses historical electricity demand data from India to analyze consumption patterns and forecast future hourly demand. It combines time-series feature engineering, machine learning, and an interactive Streamlit dashboard to make electricity demand data easier to explore and understand.

The goal is to build a practical forecasting tool that demonstrates how historical data can be used to identify demand patterns and estimate future electricity requirements.

## Features

- **Hourly demand forecasting:** Generate predictions for future electricity demand.
- **Time-series feature engineering:** Use time-based features and historical demand values to capture recurring patterns.
- **Machine learning:** Train a Ridge Regression model with cross-validation to select model parameters.
- **Interactive dashboard:** Explore historical demand, forecasts, and model performance through a Streamlit interface.
- **Data exploration:** Examine demand trends and patterns across different time periods.
- **Model evaluation:** Compare predicted demand with actual values using regression evaluation metrics.

## Technologies Used

- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib
- Streamlit

## Dataset

The project uses historical hourly electricity demand data for India, covering multiple years.

The data includes timestamps and national electricity demand measurements. These records are processed to create features such as hour, day, month, day of the week, and lagged demand values for model training.

**Dataset source:** Add the original dataset source and attribution link here.

## Model and Evaluation

The forecasting model uses Ridge Regression, a regularized linear regression algorithm. Time-based features and previous demand observations are used to predict future electricity demand.

Model performance is evaluated using metrics such as:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Mean Absolute Percentage Error (MAPE)

The data is split chronologically for evaluation so that earlier observations are used to train the model and later observations are used to test its predictions.

Actual performance may vary depending on the forecasting period and the data available to the model.

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/india-electricity-demand-forecasting.git
cd india-electricity-demand-forecasting
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Install the dependencies

```bash
pip install -r requirements.txt
```

### 3. Start the dashboard

```bash
streamlit run app.py
```

Once the application starts, open the local URL displayed in your terminal.

## Limitations

The forecasts are based primarily on historical demand patterns and time-based features. The current model does not directly account for factors such as weather conditions, public holidays, electricity prices, or real-time grid conditions.

The predictions should therefore be treated as estimates for analytical and learning purposes, rather than operational recommendations for electricity grid management.

## What I Learned

Through this project, I worked on:

- Cleaning and preparing time-series data.
- Creating features from timestamps and historical observations.
- Training and evaluating a machine learning regression model.
- Using chronological train-test splits for forecasting evaluation.
- Building an interactive data application with Streamlit.
- Presenting model results through visualizations and performance metrics.

## Future Improvements

- Incorporate weather and holiday data to improve forecasts.
- Compare Ridge Regression with other time-series forecasting approaches.
- Add prediction intervals to communicate uncertainty.
- Evaluate performance across different forecast horizons.
- Deploy the dashboard so that it can be accessed online.

## Author

**Lakshaya Aswal**

GitHub: https://github.com/lakshayaAswal
