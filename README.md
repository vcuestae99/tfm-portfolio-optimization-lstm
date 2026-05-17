# tfm-portfolio-optimization-lstm
# Dynamic Portfolio Optimization with LSTM

This repository contains the code developed for a Master's Thesis on dynamic portfolio allocation using Deep Learning.

The project implements and evaluates an end-to-end LSTM model that generates portfolio weights directly from historical market data. The model is compared against traditional strategies such as Buy & Hold ACWI, Equal Weight allocation and Markowitz Max Sharpe optimization.

## Assets

The investment universe consists of the following ETFs:

- SPY
- VGK
- EWJ
- VWO
- XLK
- XLE
- GLD

The benchmark used is ACWI.

## Methodology

The project uses:

- Weekly historical data obtained with `yfinance`
- Monthly portfolio rebalancing
- Feature engineering based on returns, volatility, RSI, moving averages and VIX
- Walk-forward validation
- Transaction costs
- LSTM end-to-end portfolio weight generation
- Sharpe ratio loss penalized by turnover

## Repository structure

- `notebooks/`: main notebook with the complete implementation
- `src/`: auxiliary Python scripts
- `results/`: generated metrics and figures

## Requirements

The main Python libraries used are:

- numpy
- pandas
- yfinance
- scikit-learn
- tensorflow
- scipy
- matplotlib

## Disclaimer

This project is developed for academic purposes only and does not constitute financial advice.
