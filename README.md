# PySpark [![Profile][title-img]][profile]

[title-img]:https://img.shields.io/badge/-LAVS-blue
[profile]:https://github.com/LAVS-TM



PySpark project is an **analysis**, a development of **insights** and a training of a **prediction model** for different stocks dataset such as `APPLE`, `AMAZON` or `GOOGLE`. All the work is done with **Spark** in python.

<img src="https://github.com/LAVS-TM/PySpark/blob/main/prices.png" alt="Prices">

## Repository

The repository is organised as follows :

* `project_part1.ipynb` is our first part with the data analysis and with the insights of the stocks.
* `project_part2.ipynb` contains the part 2 of the project with the machine learning on the data.
* `data` contains the data of the project.
* `Big_Data_presentation.pdf` is our slides for the final presentation.


## Analysis

First in this section, we **explore** the datasets to have more informations about them. We have 7 different dataset on the stocks of different companies : `AMAZON`, `APPLE`, `FACEBOOK`, `GOOGLE`, `MICROSOFT`, `TESLA` and `ZOOM`.

Then we study the datasets to answer those questions :
* What is the average of the **opening** and **closing prices** for each stock price and for different time periods (week, month, year) ?
* How do the stock prices change day to day and month to month ?
* Based on the opening and closing price, what is the **daily return** of each stock ?
* What are the stocks with the highest **daily return** ?
* What is the average **daily return** for different periods (week, month, and year) ?

We also analyse the **moving average** and the **return rate** of the stocks and the **correlation** between the different stocks.


## Insights

In this section, we implemented 8 different **insights** to get more informations about our datasets and that can be helpful for our use case.

* 1 - Price data :
**Close price** evolution for each stocks depending on the date.

* 2 - Variance :
Computation of the **variance** of our stocks, it helps us know how the price will evolve and how volatile the investment will be.

* 3 - Volatility (standard deviation) :
Computation of the **standard deviation**. Here it helps us to determine the risks of an investment in the stock. When the **standard deviation** is closer to the mean, the investment is less risky. But when the **standard deviation** is further from the mean, the investment is of greater risk.

* 4 - Covariance :
A positive **covariance** means that returns of the two assets move together while a negative **covariance** means they move inversely.

* 5 - Return Percentage

* 6 - Expected Returns

* 7 - Value At Risk

* 8 - MACD :
**MACD** is the Moving average convergence divergence (MACD), a trend-following momentum indicator that shows the relationship between two **moving averages** of a stock price.


Here is an example of the **MACD** for the `APPLE` stock :

<img src="https://github.com/LAVS-TM/PySpark/blob/main/macd.png" alt="MACD">

## Machine Learning

The **machine learning** part is quite simple, we want to predict the stock for the future using our dataset (here the `CLOSE` variable).

We are using the **Root Mean Square Error** (RMSE) which is a standard way to measure the error of a model in predicting quantitative data.
We are also using the **R2_score**.