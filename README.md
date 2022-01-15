# stock-analysis
##Purpose and Background
The primary purpose of this analysis is to obtain a clear understanding of how stocks perform in relation to one another, year by year. By looping over each row of stock data for a given year and then attributing it to the stock index variable, I was able to compute the total daily volume and annual return for a set of stocks. The secondary purpose of this analysis was to optimize the code to allow for quicker run time for the macro. Faster run times are valuable in this instance because of the potential of working with very high volumes of trading data. 

##Results
By looking at the results for 2017 and 2018 – visualized below in Figure 1 and Figure 2, respectively – we can immediately see that most of the stocks under this analysis were up in value in 2017 and subsequently lost value in 2018. There are two that stand out as having appreciated in price for both years: ENPH and RUN. Basing recommendations off of this set of data, I would highlight those as solid performers to keep an eye on. 

The method for optimizing the code for run time was to connect the information to a ticker index variable that could access each ticker in the array. This was done instead of looping through each row and each individual ticker. The finding was that 
