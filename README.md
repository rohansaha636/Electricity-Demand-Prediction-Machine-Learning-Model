# Electricity Demand Prediction using XGBoost

## Overview

This project predicts electricity demand using the XGBoost Regression algorithm. Historical electricity demand data is analyzed and used to train a machine learning model capable of forecasting future electricity demand with high accuracy.

The project demonstrates the complete machine learning workflow, including data preprocessing, exploratory data analysis, model training, evaluation, visualization, and model serialization.

---

## Features

* Data preprocessing and cleaning
* Exploratory Data Analysis (EDA)
* Feature engineering
* XGBoost Regressor model
* Model evaluation using multiple metrics
* Demand prediction visualization
* Model saving and loading using Joblib
* High prediction accuracy

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost
* Joblib
* Jupyter Notebook

---

## Dataset

The project uses historical electricity demand data stored in:

`Electricity+Demand+Dataset.csv`

The dataset contains electricity demand records and corresponding date-time information used for model training and evaluation.

---

## Model Performance

### XGBoost Regressor Results

| Metric                         | Score  |
| ------------------------------ | ------ |
| R² Score                       | 0.9849 |
| Mean Absolute Error (MAE)      | 123.08 |
| Root Mean Squared Error (RMSE) | 173.44 |

### Interpretation

* The model explains approximately **98.49%** of the variance in electricity demand.
* The average prediction error is approximately **123 units**.
* The model successfully captures seasonal and daily demand patterns.
* Minor deviations occur during sudden extreme demand spikes.

---

## Project Structure

```text
Electricity-Demand-Prediction/
│
├── Electricity_Demand_Prediction_Machine_Learning_Model.ipynb
├── Electricity+Demand+Dataset.csv
├── electricity_xgb_prediction_model.pkl
├── requirements.txt
└── README.md
```

---

## Installation

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

1. Open the Jupyter Notebook:

```text
Electricity_Demand_Prediction_Machine_Learning_Model.ipynb
```

2. Run all notebook cells sequentially.

3. Train the XGBoost model.

4. Evaluate model performance using R², MAE, and RMSE metrics.

5. Generate demand prediction visualizations.

---

## Saved Model

The trained model is stored as:

```text
electricity_xgb_prediction_model.pkl
```

Load the model using:

```python
import joblib

loaded_model = joblib.load("electricity_xgb_prediction_model.pkl")
```

Make predictions:

```python
predictions = loaded_model.predict(X_test)
```

---

## Future Improvements

* Incorporate weather features such as temperature and humidity.
* Add lag-based and rolling-window features.
* Perform hyperparameter tuning using GridSearchCV.
* Compare performance with LSTM and GRU models.
* Deploy the model as a web application using Flask or Streamlit.

---

## Author

**Rohan Saha**

Computer Science Engineering Student

Machine Learning • Data Science • Artificial Intelligence

