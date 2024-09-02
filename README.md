# Stock Price Prediction using Deep Learning Models

This repository contains the implementation and analysis of various deep learning models used for stock price prediction. The models evaluated in this project include Long Short-Term Memory (LSTM), Gated Recurrent Unit (GRU), and Generative Adversarial Network (GAN). This project is part of the QF634 – Applied Quantitative Research Methods course for the MSc in Quantitative Finance.

### Project Overview

#### 1. Introduction
The project aims to apply deep learning techniques to predict stock prices for three companies: Apple Inc. (AAPL), eBay Inc. (EBAY), and Starbucks Corporation (SBUX). The study compares the predictive performance of three models—LSTM, GRU, and GAN—on the historical stock prices of these companies.

#### 2. Models Implemented
Long Short-Term Memory (LSTM): A type of Recurrent Neural Network (RNN) that is capable of learning long-term dependencies and is widely used in time-series prediction tasks.
Gated Recurrent Unit (GRU): A variant of LSTM that has fewer parameters and can be trained faster while maintaining comparable performance.
Generative Adversarial Network (GAN): A framework that consists of two neural networks, a generator and a discriminator, which compete against each other to improve the accuracy of the generated outputs.

#### 3. Dataset and Features
The dataset includes daily closing prices of AAPL, EBAY, and SBUX from January 1, 2013, to December 31, 2022.
A total of 15 features, including basic stock data, technical indicators, and fundamental indicators, were used for model training.

#### 4. Methodology
Data preprocessing involved normalization and splitting the dataset into training and testing sets.
The GAN model utilized GRU as the generator and Convolutional Neural Network (CNN) as the discriminator.
The models were trained and evaluated using performance metrics such as RMSE, MAE, MAPE, MSLE, and R².

#### 5. Experimental Results
The GAN model demonstrated superior accuracy in the testing phase across all stocks compared to LSTM and GRU.
GRU showed competitive performance during the training phase but was outperformed by GAN in testing.
LSTM, while effective, lagged behind both GRU and GAN in terms of predictive accuracy.

#### 6. Conclusion
The GAN framework excels in capturing time-series patterns and offers superior accuracy compared to traditional LSTM and GRU models. However, the complexity of GANs necessitates extensive hyperparameter tuning. Future studies could explore more efficient hyperparameter tuning strategies and the application of other generative models to further enhance prediction accuracy.

#### Repository Structure
QF634 - Deep Learning Models for Stock Prices Prediction.ipynb: The Jupyter notebook containing the implementation of LSTM, GRU, and GAN models, along with data preprocessing and results analysis.
Fundamental_data.csv: This CSV file contains the fundamental data of the stocks used in the project. It includes key financial metrics and ratios that are considered in the analysis and model building process.
FED_interest_rate.csv: This CSV file contains data on the Federal Reserve's interest rates, which is used as an external factor influencing stock prices. This data is integrated into the models to analyze its impact on stock price predictions.

#### Acknowledgments
This project was developed as part of the QF634 – Applied Quantitative Research Methods course at Singapore Management University.
