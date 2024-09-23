# MSc-Project

This repository contains the code, experiments, and analyses referenced in my MSc dissertation. Rather than overloading the dissertation itself with code, this repository serves as an appendix where you can explore some of the exploratory work and final model implementations. All coding was done using Jupyter Notebooks.

## Structure of the Repository
1. Archive

The "Archive" folder contains various experiments from the exploratory phase. This section was primarily used to test different approaches and methodologies, and is somewhat disorganised. However, it demonstrates some of the time and effort spent during the exploratory process.

    actual+predicted: This folder contains notebooks where I examined the actual vs. predicted results when experimenting with log differencing. I closely inspected the actual vs predicted values to investigate why DA wass consistly <50% before discovering that predictions could simply be inversed to make them useful.

    lstm1-6: Testing various LSTM configurations including:
        Binary classification (e.g., lstm5)
        Log differencing
        Multi-layer architectures
        Early stopping
        Different activation functions and optimizers

    ETH: Contains experiments using ETH (Ethereum, another cryptocurrency) instead of Bitcoin data sourced from Binance.

    longterm: These files are from attempts to predict beyond just the next time step (t+1) by using more granular datasets.

2. Preprocessing and Datasets

This folder includes scripts for data preprocessing. The main dataset was downloaded from Kaggle at https://www.kaggle.com/datasets/jkraak/bitcoin-price-dataset and is too large to be included in this repository. However, by placing the kaggle dataset in the same folder and then following the numbered scripts (1-4), the necessary preprocessed datasets can be generated.

3. Results

The "Results" folder contains the results generated from the Daily dataset. Due to file size limitations on GitHub, only the results from the Daily are listed.

4. Main Files

The main directory contains the final versions of the models used in the dissertation, including:

    ARIMA: Final experiment using ARIMA .
    GRU: Final experiment using GRU.
    LSTM: Final experiment using LSTM.
    trading_simulations_arima: Trading simulation using the ARIMA model's results.
    trading_simulations_gru: Trading simulation using the GRU model's results.
    trading_simulations_lstmb: Trading simulation using the LSTM model's results.

Notes

    The code in the exploratory phase was not optimised for readability and may contain redundant or unfinished elements, as it served the purpose of exploring different methods and approaches.
