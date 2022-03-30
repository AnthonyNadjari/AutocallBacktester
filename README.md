# Autocall Backtester for Athena/Phoenix Baskets : Worst-of, Best-of, Equally-Weighted & Single Stocks
The repository comes into two files:

 
* **Python file**: computes the backtest of an autocall from the Excel file. Details can be found directly in the Jupyter file. The user is invited to directly change the directory to where the Excel file is.
* **Excel file**: before running the code, parameters of the autocall shall be input in the Excel file. This implies : 
  * Start date and End date of the backtest
  * Bloomberg Tickers of the underlyings (note that Bloomberg is required to update the data)
  * Type of the basket
  * Maturity of the product
  * Barriers and coupons 
  * Memory of the bullet coupon
  * Details of the short leg : Geared Put, PDI,...   
* **Note that the backtest will end if the maturity is too short** : if the product is recalled before the backtest end date, but its maturity is above the backtest end date, it will not be processed.
