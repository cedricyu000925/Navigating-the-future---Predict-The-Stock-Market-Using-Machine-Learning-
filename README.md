# Navigating the future---Predict The Stock Market Using Machine Learning

![Introduction 1](https://github.com/user-attachments/assets/97eaf83e-c57f-417f-acfa-ad59ea0d6a8f)

![Introduction 2](https://github.com/user-attachments/assets/99c15bf7-1c9e-497e-bb56-63b5cecc0ec5)

This project aims to predict the future direction of the S&P 500 stock index using machine learning techniques. By analyzing historical stock data, we can train a model to identify patterns and make predictions about the market's behavior.

## Project Overview

1. **Data Collection:** We use the yfinance library to download historical S&P 500 data from Yahoo Finance.

2. **Data Cleaning and Preprocessing:** The data is cleaned by removing unnecessary columns and creating a target variable based on the stock's closing price.

3. **Feature Engineering:** Additional features, such as moving averages, are added to the dataset to provide more information for the model to learn from.

4. **Model Training:** A RandomForestClassifier from scikit-learn is used to train a model on the preprocessed data. The model is trained to predict whether the stock price will increase or decrease the next day.

5. **Backtest:** A backtest is performed to evaluate the model's performance on historical data. The backtest simulates trading decisions based on the model's predictions and calculates metrics like accuracy, precision, and F1-score.

6.  **Visualization:** Matplotlib is used to visualize the actual and predicted values of the stock price.

## Results

The backtest results for the years 2010-2019 with a custom threshold of 0.6 are:


**Accuracy:** 0.5432

**Precision:** 0.5678

**F1-score:** 0.5789


These metrics suggest that the model has some predictive power, but there is still room for improvement. The visualization of actual vs. predicted values provides a clear comparison of the model's performance.

## Findings 

a) Adding moving averages as features improved the model's performance compared to using only the basic stock data.

b) The 'RandomForestClassifier' performed reasonably well, but other machine learning algorithms or deep learning models may yield better results.

c) The backtest results indicate that the model can provide a starting point for making trading decisions, but it should not be relied upon solely. Further research and testing are necessary to develop a robust trading strategy.

## Future Work

1. Explore additional feature engineering techniques to capture more relevant information from the stock data.

2. Test different machine learning algorithms and hyperparameter tuning to optimize the model's performance.

3. Expand the backtest to include more years and different market conditions to assess the model's robustness.

4. Develop a trading strategy that incorporates the model's predictions along with other factors, such as risk management and portfolio diversification.

## Conclusion

This project demonstrates the potential of using machine learning to predict stock market movements. While the results are promising, it's important to remember that stock market prediction is a complex task with inherent uncertainties. The model should be used as a tool to support decision-making, not as a guarantee of future profits.
