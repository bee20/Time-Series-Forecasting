# Time-Series-Forecasting

Some insights:

## AR/ ARIMA/ SARIMA  <br/> vs  <br/> ETS (Simple Exponential/ Holt/ Holt Winter and others)  <br/> vs  <br/> UCM (structural model): <br/>
1. ARIMA/ SARIMA usually used when series is stationary, if not stationary than convert to stationary.
2. ETS mainly used when trend seasonality is there, is also more easy to interpret as it is able to decompose into Level, Trend, Seasonality.
3. In ARIMA you can add exogenous variables / X variables/ Independant variables but in ETS we can not (although some ETS models with exogenous variables are in progress which are not stable).
4. ETS are state space models because the forecasting equation can be represented as state space equations. Wherein, the observed component is y series and the unobserved components are level, trend, season.
5. Further, UCM (structural time series models) are also state space models but can include exogenous variables and can be considered like regression. That is now we can have multivariate data instead of univariate.
6. UCMs are easily constructed in state space form. This enables the application of the Kalman filter algorithms, through which maximum likelihood estimation of the structural parameters are obtained, optimal predictions are made about the future state vector and the time series itself, and smoothed estimates of the unobserved components can be determined.
7. These are general guidelines, however, final model can be selected using error (like RMSE), AIC, BIC.
8. There are some common models which are both ETS and ARIMA, Example: ETS(A,N,N)	= ARIMA(0,1,1)

   
## Some errors while modelling:<br/>
1. If error with .predict() -> index mismatch with test data and predicted series ->
2. check for date time format and
3. check if there are any irregular patterns in date
4. or check for any missing values. dates must be at regular intervals for this to work.<br/>
<br/>


Books:
https://otexts.com/fpp2/ets.html


Simple explanations:
https://www.youtube.com/watch?v=2XGSIlgUBDI 

https://www.youtube.com/watch?v=8FCDpFhd1zk&list=PLqYFiz7NM_SMC4ZgXplbreXlRY4Jf4zBP&index=6

https://www.youtube.com/watch?v=QnBGtvKnGqk
