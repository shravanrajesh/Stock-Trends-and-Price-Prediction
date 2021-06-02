![test](https://sevensreport.com/wp-content/uploads/2016/07/stock-market-3.jpg)
# Stock Market Trends and Price Prediction

## Demo Preview
### ARIMA Model Predictions
AMAZON.COM INC Stock Prediction  |  ProShares UltraPro Short QQQ Prediction
:-------------------------:|:-------------------------:
![](https://github.com/brobotan/stocks_eft_predict/blob/main/Output/results/final(Amazon.com%20Inc).png)  |  ![](https://github.com/brobotan/stocks_eft_predict/blob/main/Output/results/final(ProShares%20UltraPro%20Short%20QQQ).png)

### XGBOOST Predictions
Prediction 1  |  Prediction 2
:-------------------------:|:-------------------------:
![](https://github.com/brobotan/stocks_eft_predict/blob/main/Output/XGBOOST-Results/xg_test_predict_z.png)  |  ![](https://github.com/brobotan/stocks_eft_predict/blob/main/Output/XGBOOST-Results/xg_dev_predict.png).png)

# Table of contents

<!-- After you have introduced your project, it is a good idea to add a **Table of contents** or **TOC** as **cool** people say it. This would make it easier for people to navigate through your README and find exactly what they are looking for.

Here is a sample TOC(*wow! such cool!*) that is actually the TOC for this README. -->

- [Table of contents](#table-of-contents)
- [Description](#description)
- [Usage](#usage)
- [Installations](#installations)
- [Database](#database)
- [License](#license)

# Description
[(Back to top)](#table-of-contents)

For stock price prediction two models have been used in this project.
* **ARIMA MODEL**
* **XGBOOST MODEL**
## ARIMA MODEL
ARIMA stands for Auto-Regressive Integrated Moving Averages. ARIMA (p, d, q) is a generalization of an autoregressive moving average (ARMA (p, q)) model. ARIMA models
are applied in some cases where data show evidence of nonstationarity. The AR term p of ARIMA indicates that the evolving variable of interest is regressed on its own lagged
(i.e., prior) values. The MA part indicates that the regression error is a linear combination of error terms whose values occurred contemporaneously and at various times in the past. The I (for "integrated") indicates that the data values have been replaced with the difference between their values and the previous values (and this differencing process may have been performed more than once)
### Architecture Diagram
![](https://github.com/brobotan/stocks_eft_predict/blob/main/resources/ARIMA%20ARCH(b).png)

## XGBOOST MODEL
XGBoost stands for Extreme Gradient Boosting, it is a performant machine learning library. XGBoost implements a Gradient Boosting algorithm based on decision trees. XGBoost
is an ensemble of decision trees. Those trees are poor models individually, but when they are grouped they can be really performant. Gradient boosting is a process to convert weak learners to strong learners, in an iterative fashion. Each tree is called a “weak learner” for their high bias.

XGBoost starts by creating a first simple tree which has poor performance by itself. It then builds another tree which is trained to predict what the first tree was not able to, and is itself a weak learner too. The algorithm goes on by sequentially building more weak learners, each one correcting the previous tree until a stopping condition is reached, such as the number of trees (n_estimators) to build.

### Architecture Diagram
![](https://github.com/brobotan/stocks_eft_predict/blob/main/resources/XGB%20ARCH(b).png)

# Usage
[(Back to top)](#table-of-contents)

To use any of the two models mentioned above you just need to downlaod the corresponding jupyter notebook file which has an extension of .ipynb and import the packages required.

# Installations
[(Back to top)](#table-of-contents)
<!-- Let's also add a footer because I love footers and also you **can** use this to convey important info.-->
- numpy
- matplotlib
- seaborn
- statsmodels
- pandas
- sklearn
- pmdarima
- tqdm
- xgboost

# Database
[(Back to top)](#table-of-contents)
<!-- Let's also add a footer because I love footers and also you **can** use this to convey important info.-->
We used [Database](https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs) which contains data for 7165 Stocks and 1374 ETFs.
Data is presented in txt format that we will convert it into a csv file. It includes attributes such as Date, Open, High, Low, Close, Volume, OpenInt. A lot of Ups and Downs in the value of Stocks and ETFs are present in the Dataset therefore we have a very wide variety of Database which we will perform to train and test our Model.

# License
[(Back to top)](#table-of-contents)

<!-- Adding the license to README is a good practice so that people can easily refer to it.

Make sure you have added a LICENSE file in your project folder. **Shortcut:** Click add new file in your root of your repo in GitHub > Set file name to LICENSE > GitHub shows LICENSE templates > Choose the one that best suits your project!

I personally add the name of the license and provide a link to it like below. -->

[The MIT License](https://opensource.org/licenses/MIT)


