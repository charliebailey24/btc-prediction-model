# Bitcoin Price Prediction using Deep Learning

A comparative analysis of LSTM and GRU architectures for Bitcoin price prediction, with systematic hyperparameter optimization that achieves better-than-baseline performance.

## Project Overview

This project implements and compares different deep learning approaches for cryptocurrency price prediction against a naive persistence baseline, specifically:
* Long Short-Term Memory (LSTM) networks
* Gated Recurrent Units (GRU)

## Key Features

* Custom implementation of both LSTM and GRU architectures
* Rigorous baseline comparison against naive persistence model
* Systematic hyperparameter optimization
* GPU-accelerated training using TensorFlow on M3 Max
* Comprehensive model evaluation using multiple metrics (MAE, RMSE)
* Time series data preprocessing and visualization
* Detailed performance analysis and architecture comparison

## Technical Highlights

* Successfully beat persistence baseline RMSE (1299.10) with optimized GRU model (1294.84)
* Demonstrated that simpler GRU architecture outperforms LSTM for this task
* Implemented efficient GPU training pipeline
* Thorough analysis of model behavior and performance patterns

## Tools & Technologies

* TensorFlow 2.16.2 with GPU acceleration
* Python data science stack (NumPy, Pandas, Matplotlib)
* Apple M3 Max GPU optimization
* Time series analysis and forecasting techniques

## Key Findings

* GRU architecture outperformed LSTM for BTC price prediction
* Model achieved better-than-baseline performance after optimization
* Longer look-back windows (lag=45) improved prediction accuracy
* Smaller batch sizes led to better model performance

## Future Improvements

* Implement multi-step predictions for 30-day forecasting
* Extend beyond test data for real-time predictions
* Add additional market indicators as features
* Implement automated trading strategies based on predictions

## Results

Final Model Performance:
* MAE: 817.14
* RMSE: 1294.84 (beating persistence baseline of 1299.10)
