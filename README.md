# AdEase Case Study: Wikipedia View Count Forecasting

## About AdEase

AdEase is an advertising and marketing technology company that helps businesses maximize user engagement at minimal cost. AdEase provides an end-to-end digital advertising solution through three core AI modules — Design, Dispense, and Decipher — enabling clients to design, deploy, and analyze ad campaigns efficiently.

## Business problem

You are working in the Data Science team at AdEase and are tasked with analyzing daily page view data for Wikipedia pages over a period of 550 days. The objective is to forecast future view counts in order to optimize ad placement strategies for clients.

The dataset contains daily view counts for approximately 145,000 Wikipedia pages across multiple languages and regions. Since AdEase serves a global client base, it is important to understand traffic patterns across different languages to predict ad performance and improve targeting efficiency.

## Objectives

-  Perform exploratory data analysis (EDA) to understand the characteristics and distribution of the data.
-  Forecast the average daily number of future Wikipedia viewers using SARIMAX family time series models.
-  Identify trends, seasonality, and cyclical variations in the time series.
-  Analyze external factors influencing viewer counts and explain observed changes.
    
## Tools Used

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Google Colab

## Models Used

- ARIMA
- SARIMAX
- Facebook Prophet

## Dataset link: https://drive.google.com/drive/folders/1mdgQscjqnCtdg7LGItomyK0abN6lcHBb

## Data Dictionary:

There are two csv files given

train_1.csv: 

In the csv file, each row corresponds to a particular article and each column corresponds to a particular date. The values are the number of visits on that date.
The page name contains data in this format:
SPECIFIC NAME _ LANGUAGE.wikipedia.org _ ACCESS TYPE _ ACCESS ORIGIN
having information about the page name, the main domain, the device type used to access the page, and also the request origin(spider or browser agent)

Exog_Campaign_eng: 

This file contains data for the dates which had a campaign or significant event that could affect the views for that day. The data is just for pages in English.
There’s 1 for dates with campaigns and 0 for remaining dates. It is to be treated as an exogenous variable for models when training and forecasting data for pages in English

## Results & Recommendations

Detailed cluster analysis and business recommendations are provided in the notebook.
