# stock-analysis
##Purpose and Background
The primary purpose of this analysis is to obtain a clear understanding of how stocks perform in relation to one another, year on year. By looping over each row of stock data for a given year and then attributing it to the stock index variable, I was able to compute the total daily volume and annual return for a set of stocks. The secondary purpose of this analysis was to optimize the code to allow for quicker run time for the macro. Faster run times are valuable in this instance because of the potential of working with very high volumes of trading data. 

##Results
By looking at the results for 2017 and 2018 – visualized below in Figure 1 and Figure 2, respectively – we can immediately see that most of the stocks under this analysis were up in value in 2017 and subsequently lost value in 2018. There are two that stand out as having appreciated in price for both years: ENPH and RUN. Basing recommendations off of this set of data, I would highlight those as solid performers to keep an eye on.

![image](https://user-images.githubusercontent.com/92336585/149673125-e5ff2abb-f7ef-4e68-8ac2-bc97b3f27015.png)

![image](https://user-images.githubusercontent.com/92336585/149673135-9c543396-e2ef-4d3f-b91c-8940d2b65d5a.png)

The method for optimizing the code for run time was to connect the information to a ticker index variable that could access each ticker in the array. This was done instead of looping through each row and each individual ticker.


##Summary
Re-factoring code is a useful way to prepare for using much larger datasets, but it can be easy to add superfluous code at the expense of code optimization. Going in with a clear plan and an understanding of what is going on in the code in the first place – especially if it was written by someone else – is important in this endeavor. With regads to this VBA script in particular, it probably did not need to be re-factored. The difference in run-time was minimal, and computers these days have so much more computing power that the difference was only notable because we were paying specific attention to it. However, if many thousands of stocks were being analyzed, it could make a difference. It would definitely be worth it to compare the run time of the 12 stocks in this analysis with an analysis of all stocks in the S&P 500 or the NASDAQ. However, when considering that the Dow Jones Industrial Average, the main benchmark of stocks in the US, only contains 30 companies, the run-time issue does not appear very important. 
