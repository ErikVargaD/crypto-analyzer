# Crypto Analyzer

Project made in Python and Tableau to explore and compare tendencies between the top performing cryptos.
For this project, only the top 15 most performing or more prevalent cryptos were used.

All the data was extracted from [coincodex](https://coincodex.com/).

## Data Visualization

### Summary View
![](https://github.com/ErikVargaD/crypto-analyzer/blob/main/img/combined_view.png)

The summary view shows the four primary charts, historical price, volume, market cap and daily variability of price. On top of the charts, a date filter allows to select the range of dates to visualize. On the left side of the screen there's a filter that allows to select multiple cryptos to compare between.

### Historical Price Chart
![](https://github.com/ErikVargaD/crypto-analyzer/blob/main/img/historical_price.png)

The historical price chart allows to compare the price between different cryptos, where each data point represents the maximum price of each day, in the interval established in the date filter.
This chart can be used to establish the most dominant periods, using multiple cryptos to XXXXX

The straight lines (not dotted) indicate the average price for each crypto in the period of time specified.
The dotted line indicates the trend of the crypto, in the specified period of time. 
In the example above, using both the average and the trend line, we can see that even though the average price is very similar, the trend is postive in one and negative in the other, indicating a possible change in dominance between them.

### Historical Market Cap Chart
![](https://github.com/ErikVargaD/crypto-analyzer/blob/main/img/historical_market_cap.png)

The historical market cap chart allows to represent the weight of each crypto in the market. Each data point represents the average market cap of each day, in the interval established in the date filter.

The market cap is a calculated formula, using the total amount of coins in circulation multiplied by the price of the coin.
Using the previous example, we can see that even though the average price is very similar, the average market cap is almost double on one of them. These could be due to the different amount of coins in circulation, not only the price.
The continuous addition of coins into circulation can create a big difference in market cap over time, and the stability and/or growth in price can show the strenght of the coin.

### Historical Volume Chart
![](https://github.com/ErikVargaD/crypto-analyzer/blob/main/img/historical_volume.png)

The historical volume chart represents the total amount of transactions of each day, in the interval established in the date filter, for each crypto.

The volume is used to assess the trends and the market sentiment overall, indicating if a market is stable or volatile.
The average volume over time can be used to compare the overall interest of the market in each coin, meanwhile a positive trend indicates a possible future perspective and a growing interest.

### Daily Variability of Price
![](https://github.com/ErikVargaD/crypto-analyzer/blob/main/img/daily_var_price.png)

The daily variabily of price chart represents the difference, in percentage, between the maximum and the minimum price of the day compared to the average, in the interval established in the date filter.

The daily variability can be used to represent the overall price stability of a crypto, or indicate periods of high volatility.
Using this chart can be useful to assess which cryptos suffer less price variability, or they do but in a more consistent way, as seen in the average line in the example above. On the other hand, more price variability could also mean that the crypto offers better trading opportunities.

## Installation
- Make sure you have ``Python3`` installed [(Download here)](https://www.python.org/downloads/).
- Install the necessary packages from the terminal:
```bash
pip install pandas
pip install openpyxl
```
- Install Tableau for free from [here](https://www.tableau.com/products/public).

## Usage
- Place all ``.csv`` files inside the ``/data`` folder, or use the ones provided already.
- Execute ``crypto_market.ipynb`` in order to generate the excel file.
- Open Tableau and import the excel file generated, or open the ``tableau_crypto_analyzer.twb`` file provided to follow the example.

## Contributing

Pull requests are welcome. For any change suggestion open an issue first.