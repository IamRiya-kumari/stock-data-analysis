# stock-data-analysis

Questions:
1) How do you read the data from stock.csv file using pandas module.
2) Print out the number of stocks.
3) Print the name of stocks.(Try using for loop)
4) What is the average return of the S&P500?
5) Which stock or index has the minimum dispertion from the mean in dollar 
value?
6) What is the maximum price for AMZN stock over the specified time 
period?
7) Check if data contains any null values.
8) Get dataframe information.
9) Define a function to plot RAW STOCK PRICES (WITHOUT 
NORMALIZATION/WITHOUT SCALING).
# The function takes in a Dataframe df as an input argument and does not 
return anything back!
# The function performs data visualization.
# Pandas works great with matplotlib, you can simply plot data directly from a 
Pandas DataFrame using plot() method(Take Date on X – axis).
10)Plot Normalized/Scaled stock prices.
# To plot Normalized/Sclaed stock prices means to start all of the stock prices 
at one point so that they can be easily compared.This will help you to see the 
amount of gains you are going to get from the listed companies.
# Create a Function that takes in Dataframe and returns Normalized Dataframe.
# For Normalization take the stock prices and divide them by the value in the 
first row of dataframe.( Notice the massive gains in Tesla Stock)
11)Perform Interactive Data visualization using Plotly.
Ref: https://plotly.com/python/
Ref: https://plotly.com/python/line-charts/
# Write a Function to perform an interactive data plotting of RAW STOCK 
PRICES (WITHOUT NORMALIZATION/WITHOUT SCALING) using 
plotly express.
# Plotly.express module which is imported as px includes functions that can 
plot interactive plots easily and effectively. 
# Loop through each stock (while ignoring time columns with index 0)
# add a new Scatter trace.(hint:fig.add_scatter)
12)SimilarlyPlot normalized stock data in an interactive way.
13)It seems that most stocks experienced massive drops in 2020, let's assume 
that you own 100 shares of the S&P500 and you bought them on Feb 19th, 
2020. How much did you lose (in $) by March 23rd, 2020? Hint: S&P500 
dropped from $3386.15 on Feb 19th, 2020 to $2237.4 by March 23rd, 2020.
14)Calculate the daily return for S&P 500.
# get sp500 data from the dataframe.
#l loop through every element in the data frame.
# Calculate the percentage of change from the previous day.
Hint: df_daily_return[j] = ((df[j]- df[j-1])/df[j-1]) * 100
# put zero in the first line item
15)Calculate the daily return for Amazon stock.
16)Define a function to calculate stocks daily returns (for all stocks)
# With in the function Loop through each stock (while ignoring time columns 
with index 0)
# Loop through each row belonging to the stock
# Calculate the percentage of change from the previous day
Hint: df_daily_return[i][j] = ((df[i][j]- df[i][j-1])/df[i][j-1]) * 100
# Set the value of first row to zero since the previous value is not available
# Use the function to get Daily returns of all the stocks.
17)Plot the Daily returns vs. time graph using both static and interactive 
plots.
Hint: use function obtianed in question 10 and question 11.
18)Calculate correlation between Daily returns of all stocks.
# Drop Date column.
# Use .corr() function
# Use heat map to show correlation.
19) From the heatmap obtained ans the following questions.
# What are the top 2 stocks that are positively correlated with the S&P500?
#What is the correlation between Amazon and Boeing? Comment on your 
answer
# What is the correlation between MGM and Boeing? Comment on your 
answer
20) Plot Histogram for Daily returns.
21)Based on the histogram, which of the following stocks are more risky? T or 
TSLA
