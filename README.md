# Investment-and-Trading-Capstone-Project

- [Project Proposal](Project%20Proposal.pdf)
- [Project Report](Project%20Report.pdf)

### Libraries used:
- numpy
- pandas
- matplotlib
- boto3
- sagemaker

## Project Overview
Investment firms, hedge funds and even individuals have been using financial models to better understand market behavior and make profitable investments and trades. A wealth of information is available in the form of historical stock prices and company performance data, suitable for machine learning algorithms to process.
In this project, we will build a stock price predictor that takes daily trading data over a certain date range as input, and outputs projected estimates for given query dates. The predicted output will be in the form of Adjusted Close price.
We will use DeepAR for our project. DeepAR utilizes a recurrent neural network (RNN), which is designed to accept some sequence of data points as historical input and produce a predicted sequence of points.
During training, you'll provide a training dataset (made of several time series) to a DeepAR estimator. The estimator looks at all the training time series and tries to identify similarities across them. And then we used the trained model to predict the adjusted closed price for some specific company.
The stock price data is obtained from [Yahoo Finance](https://finance.yahoo.com/) from the first trading day in 2015 to the last trading day in 2019 (total of 5 years).

## Reference
[SageMaker Case Study - Time Series Forecasting](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Time_Series_Forecasting)

[Yahoo Finance](https://finance.yahoo.com/)

[DeepAR](https://docs.aws.amazon.com/sagemaker/latest/dg/deepar_how-it-works.html)
