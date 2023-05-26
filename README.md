# Portfolio-Optimization-usign-LSTMs

In this project I implemented portfolio optmization over a selected set of companies.

The companies are randomly selcted but taken care to have diverse field. The data of each company is obtained from Yahoo finance.
The data obtained for each company is processed to extract new features. The New Features are Moving Average, Relative Volatility Index,
On - balance Volume, Rate of Change, Relative Strength Index, Accumulation/ Distribution Line, etc.

The data of each company after feature extraction is then merged and prepared for autoregression.
A model based on LSTMs is designed. The model contains n branches of n inputs where n is the number of companies.
All these branches or individual models are combined to get further layers are added to these combined output to extract more features.

The purpose of this project is to get the "Annual Mean Sharpe Ratio (AMSR)" on 3 years data greater than 1.25. 

We defined a custom loss function based on AMSR.
