
# ✈️ Flight Price Prediction (India → GBP Conversion)

## Overview
This project analyzes a dataset of **~300,000 domestic flight records** from India.  
The main goal is to **explore flight pricing patterns** and **predict flight prices** using machine learning.

All prices have been converted from **INR → GBP** for international relevance.  

The project demonstrates a complete **data science workflow** in a single notebook, including:

- Data cleaning and preprocessing  
- Currency conversion  
- Exploratory Data Analysis (EDA)  
- Predictive modeling using Random Forest Regression  
- Evaluation and interpretation of results  

---

## Dataset
- **Rows:** ~300,000 flight entries  
- **Columns include:**
    - `airline`: Airline name  
    - `flight`: Flight number  
    - `source_city` / `destination_city`  
    - `departure_time` / `arrival_time`  
    - `stops`: Number of stops (0,1,2+)  
    - `class`: Economy, Business, etc.  
    - `duration`: Flight duration (hours)  
    - `days_left`: Days until departure  
    - `price`: Original INR price  

**Data Cleaning & Preprocessing:**  
- Converted categorical times (`departure_time` / `arrival_time`) to ordered numeric values  
- Encoded categorical variables for modeling  
- Removed invalid rows (zero duration or price)  
- Converted prices from INR → GBP using ExchangeRate-API  

---

## Exploratory Data Analysis (EDA)
Key insights from the dataset:

- **Price Distribution:** Most flights are mid-range, with some high-priced outliers  
- **Class Impact:** Business/First class flights are significantly more expensive than Economy  
- **Stops:** More stops generally lead to higher prices and longer durations  
- **Airline Variation:** Some airlines are consistently cheaper or more expensive  
- **Booking Timing:** Flights booked closer to departure tend to cost more  
- **Departure/Arrival Times:** Evening/night flights are slightly more expensive  

Visualizations such as histograms, boxplots, and scatterplots are included in the notebook.

---

## Predictive Modeling

**Model Used:** Random Forest Regressor  

**Features Used:**
- Airline, source/destination city, stops, class, duration, days_left  
- Departure and arrival times (numeric encoding)

**Training:** 80% train / 20% test split  

**Performance Metrics:**
- **R² = 0.979** → 97.9% of variance explained  
- **RMSE = £27.55** → ~16% of mean ticket price (£173.95)  
- **MAPE = 8.88%** → Predictions are within ~9% of actual prices on average  

**Feature Importance:**  
- Most important features: duration, stops, class, airline, and days_left  

---

## Tech Stack
- Python libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Plotly, Requests  
- Environment: Google Colab / Jupyter Notebook  
- API: ExchangeRate-API for INR → GBP conversion  

---

## How to Run

1. Open the notebook file:
