# 📈 Stock Market Forecasting Using Time Series Analysis

A Python-based time-series forecasting project that analyzes historical stock market data and predicts future stock prices using **Auto ARIMA**. The project explores historical trends, feature engineering, data preprocessing, forecasting, and model evaluation to understand stock price movements.

🔗 **GitHub Repository:** https://github.com/parthvarute09/Stock-Market-Forecasting

## 📌 Project Overview

Stock market forecasting uses historical market data to identify patterns and estimate future price movements. This project applies time-series analysis techniques to historical Bajaj Finance stock data, focusing on the **Volume Weighted Average Price (VWAP)** as the target variable.

The notebook develops lag-based features and uses an Auto ARIMA model to generate forecasts, which are compared against actual values.

## 🎯 Objectives

- Analyze historical stock market data and price trends.
- Explore time-series patterns and potential seasonality.
- Perform data preprocessing and feature engineering.
- Create lag-based features using historical observations.
- Build a forecasting model using Auto ARIMA.
- Compare predicted and actual VWAP values.
- Evaluate model performance using regression error metrics.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Environment:** Jupyter Notebook
- **Libraries:** Pandas, NumPy, Matplotlib
- **Time-Series Forecasting:** Auto ARIMA, pmdarima
- **Model Evaluation:** Scikit-learn
- **Data Processing:** Data cleaning and lag-feature engineering

## 📂 Project Structure

```text
Stock-Market-Forecasting/
│
├── Time_Series_Nifty_Bajaj_deploy.ipynb
├── BAJFINANCE.csv
└── README.md
```

*Note: Include `BAJFINANCE.csv` in the repository only if you have permission to redistribute the dataset. Adjust the notebook filename or folder structure if your actual repository differs.*

## 🔍 Project Workflow

### 1. Data Collection and Loading
Load historical Bajaj Finance stock market data into a Pandas DataFrame.

### 2. Exploratory Data Analysis
- Inspect the dataset and its structure.
- Examine missing values.
- Plot VWAP over time to explore trends and possible seasonality.

### 3. Data Preprocessing
- Set the date column as the index.
- Check and handle missing values.
- Prepare the data for time-series modeling.

### 4. Feature Engineering
Create lag-based features using historical numeric observations, including previous-day, 7-day, and 30-day lookbacks. These features help represent recent price behavior without relying on unavailable future information.

### 5. Model Development
Use `pmdarima.auto_arima` to identify a suitable ARIMA configuration. Fit the model on training data using VWAP as the target and the engineered features as exogenous inputs.

### 6. Stock Price Forecasting
Generate forecasts for the test period and compare the predicted VWAP against actual values using a time-series plot.

### 7. Model Evaluation
Evaluate forecast errors using:

- **Root Mean Squared Error (RMSE):** Measures the square root of the average squared prediction errors.
- **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted values.

## 📊 Key Outcomes

- Explored historical VWAP trends and potential seasonality.
- Applied lag-based feature engineering to historical stock data.
- Implemented Auto ARIMA forecasting with exogenous features.
- Visualized actual and predicted VWAP values.
- Evaluated forecasting performance using RMSE and MAE.

*Actual model performance should be reported using the final results produced by the notebook. Forecasts are estimates, not guarantees of future market movements.*

## ⚙️ Installation and Setup

### Prerequisites
Install Python and Jupyter Notebook, then install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn pmdarima jupyter
```

### Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/parthvarute09/Stock-Market-Forecasting.git
   ```

2. Open the project directory:

   ```bash
   cd Stock-Market-Forecasting
   ```

3. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open the project notebook and update the dataset path to match your local environment.

5. Run the notebook cells sequentially to perform the analysis, train the forecasting model, generate predictions, and evaluate the results.

## 🚀 Future Improvements

- Compare Auto ARIMA with other forecasting approaches.
- Evaluate performance across different forecasting horizons.
- Add additional technical indicators and relevant market features.
- Improve visualizations and build an interactive dashboard.
- Develop a web application for displaying forecasts.
- Test the model on additional stocks and different market conditions.

## 👨‍💻 Author

**Parth Prakash Varute**

Aspiring Data Analyst | Python | SQL | Power BI | Data Science

- GitHub: https://github.com/parthvarute09
- LinkedIn: https://linkedin.com/in/parth-varute-49516a332

## ⚠️ Disclaimer

This project is intended for educational and analytical purposes only. Stock market forecasts are uncertain and should not be treated as financial advice or as a recommendation to buy or sell securities.

---

⭐ If you find this project useful, consider starring the repository!

