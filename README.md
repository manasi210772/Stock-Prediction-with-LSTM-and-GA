# Stock Price Prediction using LSTM and Genetic Algorithm

## Overview
This project predicts next-day stock prices for selected company using historical market data fetched via the `yfinance` library. The prediction is performed using Long Short-Term Memory (LSTM) neural networks, with an optional Genetic Algorithm (GA) optimization step to improve model performance. The project provides three modes of operation: default LSTM, GA-optimized LSTM, and a comparison mode.

## Prediction Modes
1. **Default LSTM:** Uses standard LSTM architecture with default hyperparameters for quick prediction.  
2. **GA-Optimized LSTM:** Employs a Genetic Algorithm to identify optimal hyperparameters and retrains the model using these values.  
3. **Comparison Mode:** Runs both methods and compares results using evaluation metrics and visualizations.

## Workflow
1. User enters a valid company ticker symbol (e.g., AAPL, TSLA).  
2. User selects the prediction mode.  
3. The system fetches historical price data using `yfinance`.  
4. Data is scaled and preprocessed for LSTM input.  
5. The model is trained and used to predict the next-day stock price.  
6. If GA optimization is selected, hyperparameters such as sequence length, hidden size, number of layers, learning rate, dropout and epochs are optimized using the Genetic Algorithm.  
7. The program displays prediction results and evaluation metrics such as RMSE and R² score.

## Technologies Used
- **Programming Language:** Python  
- **Development Environment:** Jupyter Notebook (`.ipynb`)  
- **Data Source:** Yahoo Finance API (`yfinance`)  
- **Machine Learning:** Built LSTM model from scratch using Pytorch  
- **Optimization:** Genetic Algorithm  
- **Libraries:** NumPy, Pandas, Scikit-learn, Matplotlib

## Installation and Execution
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/StockPricePrediction-GA-LSTM.git
   cd StockPricePrediction-GA-LSTM
