This project finds out the Management Efficiency of largest companies listed in 3 different stock exchanges, Dhaka Stock Exchange, New York Stock Exchange, And Toronto Stock Exchange. 

<h3><strong>Dhaka Stock Exchange (DS30_Growth.ipynb, DSEX_Growth.ipynb):</strong></h3> 
<p>DS30 index constitutes 30 largest companies by market cap and trading volume while, DSEX index constitues all 317 companies. I used BeafulSoup to scrape list of stocks from offcial website of dhaka stock exchange because there are no API to get data from DSE. Then I scraped EPS and NAV data to calculate ROE of each stock to create a growth index fund by filtering ROE values above certain threshold. I then visualized the data to check for outlier values in the stock index. </p>

<h3><strong>New York Stock Exchange(SP500_Growth.ipynb) & Toronto Stock Exchange(TSX60_Growth.ipynb):</strong></h3> 
<p>S&P500 index constitutes around 500 largest companies by market cap listed in the United States while, TSX60 index constitutes 60 largest companies listed in Canada. I used Yfinance to get income statements and balance sheets for recent 4 quarters. I then used them to calculate trailing 12 months' Net Income, TTM Assets, and TTM Shareholder's Equity. Then I calculated Return on Assets and Return on Equity for each stock and filtered the stocks with ROE and ROA values above a certain threshold. </p>

<p>I ensured that I only make 2 http requests per 5 seconds.</p>


<p> My main motivation behind this project was to find out management efficiency of each countries largest companies. But doing it manually would be very time consuming. For example, in S&P500 index, I needed to go through quarterly income statements and quarterly balance sheets, So I would have to go through 4 financial documents for each company. That means for all companies in S&P500 index I would have to read through around 2000 documents. Through this project I cut down multiple day's worth of work into minutes.</p>

<p>Tech used: Python, Numpy, Pandas, Seaborn, BeautifulSoup, YFinance</p>
