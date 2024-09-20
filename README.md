# Sentiment Analysis for Stock Price Prediction

## Overview

This repository contains the code and research for a project aimed at enhancing sentiment analysis models to improve stock price prediction accuracy. By utilizing real-time data from Twitter and Reddit, the project integrates diverse, organic sentiment signals instead of relying on pre-classified sentiment scores. The approach allows the models to be continuously refined over time, enhancing their performance as they process live data.

## Models Used

- **Support Vector Machine (SVM)**
- **Long Short-Term Memory (LSTM)**
- **Bidirectional Encoder Representations from Transformers (BERT)**
- **Support Vector Regression (SVR)** for stock price predictions

## Datasets

The project combines datasets from Twitter and Reddit, ensuring a variety of opinions and expressions, which helps in reducing overfitting and increasing the accuracy of sentiment analysis.

## Methodology

1. **Sentiment Analysis**:  
   SVM, LSTM, and BERT models were trained on individual and combined datasets and evaluated using:
   - Classification Reports
   - ROC Curves
   - Confusion Matrices
   - Accuracy and Validation Loss Curves
   
2. **Stock Price Prediction**:  
   The generated sentiment scores were used to train an SVR model to predict stock prices for the final month of the dataset. The predictions were cross-validated with actual stock price shifts.

## Key Findings

- The combination of Twitter and Reddit datasets improved model performance, particularly with the **BERT model**, which achieved 98.1% accuracy in the validation set.
- Stock price predictions based solely on public sentiment from Twitter showed limitations, indicating the need for additional factors such as economic reports.
- A secondary analysis with the BERT model explored investor sentiment during significant global events, revealing unexpected patterns of positive sentiment.

## Future Work

- Integration of macroeconomic indicators to complement sentiment data.
- Further exploration of political, social, and economic events in shaping investor sentiment.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/username/repository-name.git
   ```
2. Navigate to the project directory:
   ```bash
   cd repository-name
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook containing the models:
   ```bash
   jupyter notebook ML_and_DL_Models.ipynb
   ```

## Contact
You can contact me via danforrester4270@gmail.com if you have any enquiries regarding this work.
