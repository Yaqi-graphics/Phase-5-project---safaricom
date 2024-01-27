# Phase 5 Project: Unlocking Safaricom’s Future: Predicting the Stock Price of Kenya's telecom giant

<img width="424" alt="Capture" src="https://github.com/Yaqi-graphics/Phase-5-project---safaricom/assets/137016696/148fe71e-b13d-415d-8aa5-7777b33881d5">

### Group 8 Members.
Jackline Njuguna
Vitelis Siocha
Angel Atungire
Elsie Ochieng
Flavine Atieno
Evans Machua

## About Safaricom
Safaricom is a telecommunications service provider incorporated in Kenya as a limited liability company. Safaricom was formed in 1997 as a fully owned subsidiary of Telkom Kenya. In May 2000, Vodafone Group PLC of the United Kingdom acquired a 40% stake and management responsibility for the company. In 2008, the government offered 25% of its shares to the public through the Nairobi Securities Exchange.

## Safaricom Stocks.
The current share price of Safaricom Plc (SCOM) is KES 13.90. SCOM closed its last trading day (Monday, January 15, 2024) at 13.90 KES per share on the Nairobi Securities Exchange (NSE). Safaricom is the #1 most traded stock on the Nairobi Securities Exchange over the past three months (Oct 11, 2023 - Jan 15, 2024) therefore our project will help people discover the future value of the stock and gain significant profits.

## Project Overview

### 1. Introduction:
Our project revolves around leveraging time-series analysis to predict Safaricom's stock prices. Using advanced analytics on historical market data and key macroeconomic factors, we aim to extract crucial insights and build a robust predictive model for future stock prices.

### 2. Problem Statement
The challenge lies in the inherent unpredictability of Safaricom's stock movements. Our focus is on constructing a robust predictive model through advanced time-series analysis to unravel critical patterns in Safaricom's historical data. This predictive model aims to offer a reliable forecast of future stock prices, aiding stakeholders in navigating the complex and uncertain financial markets.

### 3. Objectives
Main Objectives
Develop a robust time-series forecasting model for Safaricom's stock prices.

## Specific Objectives
To Identify opportune times to buy and sell Safaricom stocks to maximize returns by analyzing historical data, market trends and economic indicators to pinpoint optimal entry and exit points for various project stakeholders.

To conduct sensitivity analysis to assess how inflation rate variations, interest rate, and GDP affect the model's predictions. This can be achieved by simulating different economic scenarios above and understanding how these changes affect stock price forecasts.

## Data Understanding
This analysis/modelling uses several datasets, which can be found in the data folder in this assignment's GitHub repository. Below are our understanding of the datasets.

### I. Historical Prices
This dataset provides daily historical stock prices and volumes for each stock for a given period of time. The historical price trends are used to indicate the future direction of a stock.

### II. Kenya gdp growth rate
This data set expresses the difference between GDP values from one period to the next as a proportion of the GDP from the earlier period in percentage form and showing the dates.

### III. Central bank interest rates
This dataset shows the interest rate at which Kenya's central bank charges other domestic banks to borrow funds. This rates changes based on the economic changes of our country. 

### IV. Dividend Yield
This data set shows the financial ratio that tells us the percentage of Safaricom shares price that it pays out in dividends each year. 

### V. Mobile Payments
This dataset shows the monthly data on the number of active agents, registered mobile money accounts, and agent cash in and out transactions. The most common one at Safaricom is M-Pesa.

## The Merged data set columns
1. Open price is the first price at which stock trades during market hours
2. The high and low prices reflect the highest and lowest prices the stock reaches
3. The Close price is the closing price during the previous market day.
4. Volume is the number of shares traded in a given period.
5. GDP Growth Rate shows the annual average rate of change of the gross domestic product (GDP) at market prices based on constant local currency, for a given national economy, during a specified period of time.
6. Annual average inflation is the percentage change in the annual average consumer price index (CPI) of the corresponding months.
7. Central Bank Rate shows the interest rate at which a central bank lends money to domestic banks, often in the form of very short-term loans.
8. Dividend Yield shows the measures the annual value of dividends received relative to the market value per share.

## Exploratory Data Analysis
Using the merged dataset we checked the relationship between the columns and visualized the correlation.
![correlation](https://github.com/Yaqi-graphics/Phase-5-project---safaricom/assets/137016696/26fcaf40-27e9-4623-b1b2-8be6d06895d8)

Findings
The 'Close' price demonstrates a strong positive correlation with 'Dividend Yield' (0.81) and a negative correlation with 'GDP Growth Rate' (-0.52). 'Annual Average Inflation' and 'Central Bank Rate' exhibit a significant positive correlation (0.83), while 'RSI' and 'MACD' show a moderate positive correlation (0.58). These insights provide valuable information for understanding potential interdependencies and trends within the dataset.

## Modeling and Regression Results.
### 1. Vector Autoregression
We used the close dataset to work on this model. We started by spliting the data into training and testing sets, then we trained our VAR Model in order to make predictions. After making predictions on the test set. We extracted the predicted values and visualized the same. This model gave us a rmse of 2.5715913248554116.
![vector autoregression](https://github.com/Yaqi-graphics/Phase-5-project---safaricom/assets/137016696/ab770e07-4d91-4456-b612-e68af0595ef7)

### 2. Recurrent Neural Network (RNN)
We started by converting the dataset into sequences. We started by spliting the data into training and testing sets, then we trained our RNN Model in order to make predictions. After making predictions on the test set. We extracted the predicted values and visualized the same. This model gave us a rmse of 0.04060818256430719.
![rnn](https://github.com/Yaqi-graphics/Phase-5-project---safaricom/assets/137016696/5c97007f-9a14-4a0b-9a4b-90ff9edda5b5)









