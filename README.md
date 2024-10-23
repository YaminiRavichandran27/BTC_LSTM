

# Bitcoin Price Prediction using LSTM

## Overview
This project aims to predict Bitcoin prices using historical data and a Long Short-Term Memory (LSTM) neural network. LSTM is a type of recurrent neural network (RNN) that is well-suited for time series forecasting, making it ideal for this task.

## Features
- Data Preprocessing: Cleaned and prepared the Bitcoin price dataset.
- Feature Engineering: Added features like date breakdown (year, month, day) for better analysis.
- Model Building: Used LSTM for predicting future Bitcoin prices based on historical data.
- Visualization: Plotted actual vs predicted prices to compare performance.
  
## Dataset
The dataset contains historical Bitcoin prices, including the following features:
- **Date**: Date of the record
- **Open**: Opening price of Bitcoin
- **High**: Highest price during the day
- **Low**: Lowest price during the day
- **Close**: Closing price of Bitcoin
- **Volume**: Number of Bitcoins traded during the day

## Installation and Requirements
To run this project, you'll need to install the following dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
```

## Steps to Run the Project

1. **Data Preprocessing**
   - Load the dataset and inspect the data.
   - Drop unnecessary columns like 'Adj Close.'
   - Handle missing values if any.
   - Scale the data for LSTM input.

2. **Model Development**
   - Prepare the data into sequences for time series forecasting.
   - Build and compile the LSTM model using TensorFlow/Keras.
   - Train the model on the dataset and validate its performance.

3. **Visualization**
   - Plot the actual vs predicted Bitcoin prices over time to evaluate the model.

## Results
The LSTM model provides predictions for future Bitcoin prices with reasonable accuracy.

## Usage
You can tweak the hyperparameters, such as the number of epochs, batch size, and the structure of the LSTM layers, to improve model performance.

## Future Enhancements
- Add more features such as moving averages, trading volume trends, or external financial indicators.
- Explore other time series models such as ARIMA or GRU for comparison.
- Implement real-time Bitcoin price prediction using live data.

