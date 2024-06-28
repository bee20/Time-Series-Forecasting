# Time-Series-Forecasting

Some insights:

# ARIMA/ SARIMA  vs ETS- <br/>
ARIMA/ SARIMA usually used when series is stationary, if not stationary than convert to stationary. <br/>
ETS mainly used when trend seasonality is there, is also more easy to interpret as it is able to decompose into Level, Trend, Seasonality. <br/>

# Some errors while modelling:<br/>
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
