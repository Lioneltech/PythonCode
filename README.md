# PythonCode
This is for my python codes and scripts for learning, my python project portfolios and for everyday work.
In details this contains my bootcamp projects and scripts making up my Python portfolio.




## Project 1: Amazon Web Scraping Using Python

This code is a web scraping script that extracts data from an Amazon product page using Python. The script uses the BeautifulSoup and requests libraries to scrape the data, specifying the data to be extracted using the unique identifiers of the HTML elements. The extracted data is then cleaned and formatted before being saved to a CSV file using the csv and pandas libraries. The resulting dataset can be used for actual analysis in fintech, pharma, or e-commerce, or as a portfolio project.

### Data Manipulation:
This project is focused on data manipulation. I performed operations such as filtering and sorting the data based on certain conditions. This was done to transform and reshape the data to get insights or prepare it for further analysis.


## Project 2: Using Crypto Api and Script Automation in Python

In this project we demonstrate how we used a public API in Python to access the latest cryptocurrency data from CoinMarketCap. The code uses the requests library to send a GET request to the CoinMarketCap API, specifying query parameters such as 'start' and 'limit' to filter the results. The response data is then converted from JSON to a Pandas DataFrame to make it easier to work with. The DataFrame is then normalized and a timestamp is added to indicate when the script was run. Finally, the code shows how to automate the API call by creating a function that can be run anytime we need to get the latest cryptocurrency data. The function normalizes the response data, adds a timestamp, and appends the new data to an existing CSV file.

### Data Collection, Manipulation and Visualization: 
The second project end game was data visualization.

#### Steps 1: API Calling
I got the API documentation python code, limited it to 100 different cryptocurrencies and used my API keys to called it.

#### Step 2:  Data Cleaning
a. Now we have some data to play with. 
b. I imported pandas to use in cleaning and manipulating the data.
c. Coverted the datafrom JSON format into a dataframe.

#### Step 3:  Automating the Python Script
a. Added Timestamps so i can know the time the scripts where automatically ran and also to keep track on whats happening.
b. Now i created a function that will call the API, collect that, format and clean the data from JSON format, create the timestamp, append(add) new data it will collect each time to the original already existing dataframe, create a CSV files and add this data to the CSV file thereby updatinf the CSV files each time the function is ran.
c. Using Sleep module and loop i automated the unction to be called every 1 min (60 sec) thereby giving me information chnage and price fluctuation per minute and it worked.
d. Called the csv file to appear on our notebook instead of checking the API and it worked well.

#### Step 4: Pre- Visualization
Did a little more formatting to ensure the data numerical numbers are displayed fully and not in scientific form. Then used the groupby() method to pull out the percentage change values and the currency names. It wasnt in the best visualization format so i used the stack() medthod to convert it into rows for effective visualization. Changed it back to a dataframe as using the Stack() method chnage to a series. Did some column rename and indexing then our data was ready.

#### Step 5: Visualization
Imported Seaborn libraby and matplotlib. 
Used the catplot() in seaborn to visualize the averages of the Percentage change.
Also tried using lineplot() in seaborn to show Bitcoin Price change overtime with the timestamp column we created.
Lastly i used visialized the Market cap for the top 20 crypto currencies.
