### Introductory Options 2024 Hackathon
# Conducted by the Finance and Economics Club (FEC), Indian Institute of Technology Guwahati (IITG)
# Organized by QuantInsti Quantitative Learning Private Limited

## Project Title
**Designing, Implementing, and Backtesting an Options Trading Strategy**

## Objective
This project was undertaken as part of the Introductory Options Hackathon 2024 organized by QuantInsti Quantitative Learning Private Limited.
The main goal was to develop, implement, and backtest an options trading strategy using data for Reliance Industries, a NIFTY50 stock, with options data spanning from January 2022 to December 2024.

## Problem Statement
The goal of this problem statement is to design, implement, and backtest an options trading strategy.
The objective is to combine your analytical and creative abilities to craft an efficient trading strategy. Use the insights and techniques learned during the course to optimize your results.

Below is a step-by-step guide to approaching the problem:-

1. Read the Dataset
    Select any stock listed in NIFTY 50 as the underlying asset for your strategy.
        For NSE options data, you can use the NSE official website.
        Link: https://www.nseindia.com/report-detail/fo_eq_security

2. Preprocess the Dataset
    Preprocess the data you have obtained. 
        Handle any missing values using suitable technique (forward fill, interpolation etc.).
        Create new features that might be useful (lag variables, rolling statistics, spread dynamics etc.).

3. Analyze the Stock with Indicators
    Use a technical indicator or a combination of them of your choice to analyze the historical price movement of the stock and predict whether the underlying asset price will appreciate or decline.

4. Select the Option and Apply Strategy
    Based on your forecast:
        Decide whether to buy or sell an option of the underlying stock.
        Implement any options trading strategy learned during the course (e.g., Straddle, Strangle, Bull Call Spread, etc.).

5. Risk Management
    Incorporate risk management measures into your strategy to manage exposure effectively and minimize losses.
    Use tools such as stop-loss, position sizing, or other risk metrics.

6. Backtest the Strategy
    Backtest your strategy on historical data for the timeframe 1st January 2022 to 29th December 2024.
        Use relevant performance measures to analyze the effectiveness of your strategy (e.g., net returns, annual returns, Sharpe ratio, drawdown).
        Assume no transaction costs and enough liquidity for simplification.
        Compare the performance of different strategies.
            For backtesting purpose, you can use libraries such as backtesting, backtrader etc.

## Roadmap

The given steps have been followed, in order to solve the Problem Statement of the Hackathon:
    1. Download the required Datasets, from the given link of NSE website.
        Choose any of the NIFTY50 stocks options for analysis.
            I have chose the stock options of Reliance and have downloaded the data for both Call Option as well as Put Option, month-wise, for the time-period specified, in the problem statement of the Hackathon, from January 2022 to December 2024.
    2. Install all the required libraries and modules, if not install before-hand and import them, in the coding environment.
    3. Once the datasets are download, store them together in a single folder, which can be accessed either by path or by mounting Google Drive, while coding.
    4. Access the datasets and load them in the coding environment.
    5. Visualize the datasets, along with some basic information, such as Shape, Columns, Datatypes, Description (Statistical Summary), Null Values, etc..
    6. Perform Data Pre-processing Operations, such as changing the datatypes of the columns, which would be necessary for further analysis and also treating the null values present in the datasets, mainly by interpolation, forward fill (ffill) and backward fill (bfill).
    7. Perform Feature Engineering and create new features, which would be helpful for analysis.
        The features created include - 
            Lag Variables, 
            Rolling Statistics, 
            Spread Dynamics, 
            Relative Strenth Index (RSI), 
            Simple Moving Averages (SMA), 
            Exponential Moving Averages (EMA), 
            Bollinger Bands, 
            Change in Open Interest and its Ratio, 
            Price Change Ratio, 
            Ratio of Open Interest to Number of Contracts, 
            Rolling Correlation, 
            Volume - Weighted Average Price (VWAP), 
            Implied Volatility Approximation, 
            Historical Volatility, 
            Normalized Volatility and 
            Option Greeks.
    8. Performed Technical Analysis.
    9. Build 3 Machine Learning Models namely - 
        Random Forest, 
        Logistic Regression and 
        XGBoost.
    This has been done by splitting the data into train_data and test_data and evaluated the performance of those 3 models, which would help in Technical Analysis of stocks options.
    10. Option Trading Strategy is devised, by coding.
    11. Risk Management is implemented.
    12. Finally, Backtesting is performed on the data, ranging from January 1, 2022 to December 29, 2024, thereby, concluding this project.

## About this Repository
This repository contains the code and methodology developed for the Hackathon as a part of the course of Introductory Options Trading 2024, conducted the Finance and Economics Club (FEC) of Indian Institute of Technology Guwahati (IITG), organized by QuantInsti Quantitative Learning Private Limited.
The project focuses on designing, implementing, and backtesting an options trading strategy for Reliance Industries, a NIFTY50 stock.

## File Structure

This repository consists the following files and folders in the given way:
    1. Stocks Options Dataset:
        This folder consists of 72 files, in the CSV format, which are datasets for Call Options as well as for Put Options for stocks options data from January 2022 to December 2024.
    2. Notebook Ops:
        This folder contains the file titled "FEC_IITG_IntroductoryOptions24_QuantInsti_Hackathon.ipynb', which is the Jupyter Notebook file, containing the complete code for the project.
    3. Readme File: The file titled 'README.md' providing an overview of the project.

## Data Source
The data for a NIFTY50 Stocks Options has been downloaded from the website of NSE.
The NIFTY50 that has been used for this project is RELIANCE.
The data for stocks options have been downloaded for the time period of 1st January, 2022 to 29th December, 2024.

## Dataset Details
A total of 72 datasets have been downloaded in the form of CSV files.
A single dataset contains data for a single month.
So, starting from January 2022 to December 2024, in a span of 36 months, 36 datasets are for Call Options (CE) and 36 datasets are for Put Options (CE), thereby making a total of 72 datasets.

Each of the dataset consists of the following columns:

1. Symbol - Symbol of the stock whose options are to be studied. 
    In this case, the stock options of Reliance Industries have been studied, whose symbol in NSE is RELIANCE
2. Date - The trading date for the data entry.
3. Expiry - The expiry date of the trade.
4. Option Type - The type of options being traded. 
    It is either denoted by CE for Call Options or PE for Put Options
5. Strike Price - This column represents the agreed-upon price at which the underlying asset can be bought or sold if the option is exercised.
6. Open - The opening price of the option on the given date.
7. High - The highest price of the option during the trading day.
8. Low - The lowest price of the option during the trading day.
9. Close - The closing price of the option on the given date.
10. LTP - The Last Traded Price for the option.
11. Settle Price - The settlement price for the option contract at the end of the trading session.
12. No. of Contracts - The total number of contracts traded for the option.
13. Turnover in Rs. Lakhs - The monetary turnover value of the contracts traded, in lakh rupees.
14. Premium Turnover in Rs. Lakhs - The turnover value specific to premium amounts for the contracts, in lakh rupees.
15. Open Interest - The total number of outstanding contracts for the option at the end of the day.
16. Change in Open Interest - The net change in the open interest value compared to the previous trading day.
17. Underlying Value - The price of the underlying stock (Reliance Industries in this case) corresponding to the option.

## Key Steps

1. Data Preprocessing
    a. Handling Null Values:
        The datasets consisted null values, so treating them was a necessity.
            Interpolation, Forward fill and Backward fill techniques have been used in order to impute missing data.
    b. Feature Engineering:
        Added lag variables for `Open`, `High`, `Low`, `Close`, `LTP`, and `Settle Price`.
        Calculated rolling statistics (mean, standard deviation, sum) for key columns.
        Derived technical indicators such as RSI, Bollinger Bands, Simple Moving Averages (SMA) as well as Exponential Moving Averages (EMA).
        Generated spread dynamics, open interest changes, and implied volatility approximations.

2. Exploratory Data Analysis (EDA)
    EDA was performed to understand the underlying patterns and trends in the dataset:
        Time-series analysis of Close prices.
        Correlation heatmaps for key columns.
        Distribution plots for price changes and spread dynamics.
        Rolling volatility and trading volume analysis.
        Candlestick charts for visualizing price movements.

3. Strategy Design
    The strategy was designed using the following considerations:
        Entry and exit points based on:
            RSI thresholds.
            Bollinger Bands (upper and lower bands).
    Implied volatility and historical volatility for trade decisions.
    Spread analysis to identify optimal strike prices.

4. Backtesting
    The backtesting process included:
        Simulating trades based on the defined strategy rules.
        Calculating performance metrics such as:
            Profit/Loss per trade
            Win/Loss ratio
            Sharpe ratio
            Maximum drawdown
        Visualization of equity curves to evaluate strategy performance.

5. Optimization
    Parameters like RSI thresholds, moving average window sizes, and Bollinger Band deviations were optimized to improve the strategy's performance.

## Libraries Used

The following for libraries have been used in this project:
    Data Manipulation: 'pandas' and 'numpy'
    Data Visualization: 'matplotlib', 'seaborn', 'plotly' and 'mplfinance'
    Technical Indicators: 'pandas-ta'

## Execution

In order to execute this code, follow these steps:
    1. Clone this repository -
        'git clone https://github.com/ImAni07/OptionTradingStrategy_StocksOptionsDataAnalysis.git'
    2. Install the required libraries, if not installed before-hand, using the following commands - 
        pip install pandas 
        pip install numpy 
        pip install matplotlib 
        pip install seaborn
        pip install plotly
        pip install pandas-ta
    3. Open the Jupyter Notebook in your preferred environment.
    4. Run the notebook cells step-by-step to preprocess data, analyze trends, design a strategy and backtest it.

## Results

1. The analysis and backtesting revealed insights into the performance of the designed options trading strategy.
2. The strategy showed consistent performance on historical data with notable returns and acceptable risk levels.
3. Insights gained -
    a. Effective use of technical indicators can enhance trading decisions.
    b. The importance of feature engineering and EDA in developing robust strategies.

## Challenges

1. Managing and cleaning a large dataset with missing values.
2. Optimizing multiple strategy parameters to maximize profitability.

## Future Scope

1. Extend the strategy to other NIFTY50 stocks.
2. Incorporate advanced machine learning models for trade predictions.
3. Perform real-time trading simulations using live market data.
4. Develop a comprehensive dashboard for visualizing strategy performance.

## Acknowledgement
Special thanks to QuantInsti as well as Finance and Economics Club (FEC) of Indian Institute of Technology Guwahati (IITG) for organizing the Hackathon and providing an excellent learning opportunity.

## About Author

Name: Anirban Majumder
Qualifications:-
    1. Post Graduate: Currently pursuing MTech in Biomedical Science and Engineering with Specialization in Medical Devices and Diagnostics, from Indian Institute of Technology (IITG).
    2. Under Graduate: BTech in Biotechnology from Adamas University, Kolkata.

## Contact

For queries or feedback, please reach out, via anyone of the following:-
    1. Email: animouani123@gmail.com
    2. LinkedIn: https://www.linkedin.com/in/anirban-majumder-49344a288/
    3. GitHub: https://github.com/ImAni07
    4. Kaggle: https://www.kaggle.com/animou123
    5. Facebook: https://www.facebook.com/share/1FR6kdhKCs/
    6. Instagram: https://www.instagram.com/iamani_7.9?utm_source=qr&igsh=MXhjNGV5czNoOWJqOA== 

My other profiles:-
    1. Leetcode: https://leetcode.com/u/IamAni_07/
    2. HackerRank: https://www.hackerrank.com/profile/animouani123

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Note

As an MTech student in Biomedical Science and Engineering at IIT Guwahati with a passion for Data Science and strong analytical skills, this project marks my first step into the Financial Technology (FinTech) domain.
Participating in the Introductory Options 2024, a course conducted by the Finance and Economics Club (FEC) of Indian Institute of Technology, Guwahati (IITG) and a Hackathon organized by QuantInsti Quantitative Learning Private Limited provided an incredible opportunity to apply my analytical expertise to financial data.

This repository showcases my journey into the world of options trading, where I tackled challenges like handling large datasets, designing trading strategies, and backtesting their performance. With this project, I aim to build a foundation in Financial Analytics and contribute further to the exciting intersection of technology and finance, popularly known as FinTech.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Feel free to contribute or reach out with suggestions and improvements!
