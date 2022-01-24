# Bitcoin_Arbitrage

Welcome. In this application, we are looking for arbitrage opportunities between bitcoin prices at two different exchanges. It is a python application that uses pandas to look for cryptocurrency arbitrage opportunities.

## Technologies
[Python3.7](https://www.python.org/)

[Jupyter Lab](https://jupyter.org/)

[Pandas](https://pandas.pydata.org)

[Pathlib](https://docs.python.org/3/library/pathlib.html) 

[Matplotline](https://matplotlib.org/)

## Installation guide
In order to run this application you'll need to install Python3.7 in conjunction with jupyter lab and the pandas and pathlib libraries linked above. 

## Usage

### 1)Collecting the data
This application is designed to be used with csv files.
Here we collect the data using pandas read_csv function.
We then ensure the data has been imported properly by calling the "head" function.

### 2)Prepare the Data
Next, we convert strings ("$") into parsable data using str.replace, convert the data type of the "Close" column into a float for calculation

### 3)Analyze the Data
This is where the real fun begins. Summaries are generated from the csv_dataframes to show the price of bitcoin at both Bitstamp and Coinbase over time. We then plot this data using the .plot function. We create plots for different dates and times in order to be able to visually find arbitrage opportunities. The greater the difference between the price of an asset at any given time between exchanges, the more profitable the opportunity.

### 4)Calculate the Arbitrage profits
Here we take our compiled data and put it to work by calculating profits made possible through arbitrage. Here is where we figure out exactly where there are profitable opportunities (difference in price great enough to cover a 1% trading fee) and we filter out unprofitable trades where there aren't any opportunities.

This Data is presented both in summary using the .describe function as well as graphically using the .plot function.

## Contributors

Tim Tennyson 
<ttennyson.xyz@gmail.com>

License: Open source, free distribution/reproduction