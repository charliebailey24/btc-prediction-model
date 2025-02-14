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
* Analysis of model behavior and performance patterns

## Tools & Technologies

* TensorFlow 2.16.2 with GPU acceleration
* Python data science stack (NumPy, Pandas, Matplotlib)
* Apple M3 Max GPU optimization

## Key Findings

* GRU architecture outperformed LSTM for BTC price prediction
* Model achieved better-than-baseline performance after optimization
* Longer look-back windows (lag=45) improved prediction accuracy
* Smaller batch sizes led to better model performance

## Results

Final Model Performance:
* MAE: 817.14
* RMSE: 1294.84 (beating persistence baseline of 1299.10)

## Getting Setup to View Project

For a quick view, you can check out the [BTC_prediction.pdf](BTC_prediction.pdf) doc. If you would like to see the full setup and run the Deep Neural Network locally, please follow the instructions below.

Note: This project was originally developed on Apple Silicon. If you're running on Windows/Linux/Intel Macs, GPU access will need to be configured differently. If GPU access is not enabled, the code will default to run on the CPU, which may result in significantly longer training times.

### Prerequisites

Python 3.10.x (Tensorflow Requirement)

### Instructions

1. Clone down the repository

    `git clone https://github.com/charliebailey24/btc-prediction-model.git`

2. Navigate into the project directory

    `cd btc-prediction-model`

3. Create and activate a virtual environment

    `python -m venv .venv`

    `source venv/bin/activate`

4. Install dependencies

    Apple Silicon:
    `pip install -r requirements-macos.txt`

    Windows/Linux/Intel Macs:
    `pip install -r requirements.txt`

5. Launch Jupyter and open the notebook

    `jupyter notebook BTC_prediction.ipynb`

## Future Improvements

* Implement multi-step predictions for 30-day forecasting
* Extend beyond test data for real-time predictions
* Add additional market indicators as features
* Implement automated trading strategies based on predictions