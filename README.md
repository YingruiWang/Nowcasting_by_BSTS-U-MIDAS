# Nowcasting_by_BSTS-U-MIDAS
This is my master thesis using Bayesian structural time series and MIDAS model to do nowcasting for Canadian GDP


Using high frequency data for forecasting or nowcasting, we have to deal with three major problems: 

- the mixed frequency problem, 

- the high dimensionality (fat regression, parameter proliferation) problem, 

- and the unbalanced data problem (miss- ing observations, ragged edge data). 

We propose a BSTS-U-MIDAS model (Bayesian Structural Time Series-Unlimited-Mixed-Data Sampling model) to handle these problem. This model consists of four parts. 

- First of all, a structural time series with regressors model (STM) is used to capture the dynamics of target variable, and the regressors are chosen to boost the forecast accuracy. 

- Second, a MIDAS model is adopted to handle the mixed frequency of the regressors in the STM. 

- Third, spike- and-slab regression is used to implement variable selection. 

- Fourth, Bayesian model averaging (BMA) is used for nowcasting. 

We use this model to nowcast quarterly GDP for Canada, and find that this model outperform benchmark models: ARIMA model and Boosting model, in terms of MAE (mean absolute error) and MAPE (mean absolute percentage error).
