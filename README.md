# Regression on LT Finance Holdings Ltd Stock Price Dataset

This project aims to predict the trading volume of a specific stock. Regression shall be used to predict the trading volume of L&T Finance Holdings Ltd through various attributes

Dataset Link: https://www.kaggle.com/datasets/sanjogyadav/lt-finance-holdings-ltd-stock-price-2017-to-2020

### Dealing with empty value
Empty value is found in the row of 31-Aug-17 on ‘Deliverable Quantity’ and ‘% Deli. Qty to Traded Qty’ columns. To solve this issue, missing data was found on the source of the dataset – the Bombay Stock Exchange.

![Picture1](https://user-images.githubusercontent.com/72193228/185613987-4da7d445-69a6-432b-9cc4-18760d4fe30e.png)
###### Raw data for 31-Aug-17 row
![Picture2](https://user-images.githubusercontent.com/72193228/185614049-95283281-3213-49c1-839c-f72176ce5295.png)
###### Updated data for 31-Aug-17 row

### Result
![image](https://user-images.githubusercontent.com/72193228/187373007-da12a68a-c301-4c1d-97c1-22aad60f36f9.png)

Overall, the linear model outperforms with lower MAE, MSE, RMSE and high R2 values as shown in the table above with green highlights. This indicates the linear model adapts well to the data. The simple model is sufficient to predict the trade volume.

By looking at the linear model, it is found that it learns better with a complete dataset compared to highly correlated attributes. MAE, MSE and RMSE of the linear model are higher when trained with highly correlated attributes. The higher R2 value in the complete dataset indicates how well the values fit compared to the original values.

As for the non-linear model, the result is surprisingly similar for both the complete dataset and highly correlated attributes. There is not much difference in terms of performance metrics, density plot and parameter tuning. The ability of the non-linear model to learn the pattern is similar in both situations.
