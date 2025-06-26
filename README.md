# Gold Price Prediction with Linear Regression

This project predicts future gold prices using a simple Linear Regression model.

## Overview

- The model uses the past 5 days' closing prices to predict the next day's price.
- The script predicts gold prices for the next 300 business days.
- This is a basic time-series forecasting example and does not consider external factors.

## Requirements

- Python 3.x
- numpy
- pandas
- scikit-learn


pip install numpy pandas scikit-learn


---

## 📊 Dataset

The dataset was retrieved using the `yfinance` library, using the Yahoo Finance ticker `GC=F` (Gold Futures).  
We used the `Close` prices for modeling. The CSV file is stored in the `data/` folder.

---

## 🧪 Methodology

1. Fetch historical gold prices from 2010 to 2024
2. Perform exploratory data analysis (EDA)
3. Train-test split of the dataset
4. Apply Linear Regression for prediction
5. Evaluate the model using R² Score and RMSE
6. Visualize predicted vs actual prices

---

## 🛠 Technologies Used

- Python 3.10  
- Pandas, NumPy  
- Scikit-learn  
- yfinance  
- Matplotlib, Seaborn

---

## ⚙️ How to Run

1. Install dependencies:

```bash
pip install -r requirements.txt


## Usage

1. Prepare your historical gold price data as a CSV file with a 'Close' column.
2. Load your data in the script.
3. Run the prediction script:



python predict_gold.py

The script will print the predicted prices day by day.

## Notes

- The model assumes prices depend linearly on the previous 5 days.
- Predictions are cumulative; each predicted price is used to predict the next.
- Results may diverge over long-term forecasts.
