# Price Analysis - NYC Airbnb data

<img src="images/airbnb.jpg?raw=true"/> <br>

*Author* - Sathish Manthani

*Statistics project* - NYC Airbnb Price Analysis using R

*Dataset* – New York City Airbnb Open Data

For those who don’t know Airbnb – it offers lodging, primarily homestays and tourism experiences. Just like Uber, the company does not own any of the real estate nor does it host any events. It acts as a middleman between the customer and the owner providing the accommodation and Airbnb receives commission from each booking.

## Problem Statement

Problem statement is to explore Airbnb cost in different areas of New York. What are the variables influencing the price of Airbnb stay.

## Questions

The questions I would like to ask on the dataset are:
1.	How the price is varying in the neighborhood
2.	How the price is varying with room type
3.	What is the relationship between location and price
4.	Are reviews influencing the price

## Solution Approach

I initially did the data cleansing steps like data type conversions, drop unwanted variables, duplicate data check and missing values check.
Later, I explored the categorical variables like room type, neighborhood and explored distribution of the variables using histograms.
I checked the correlation of price variable with other variables in the dataset. Correlation tells us the strength of the relationship between the variables. 
Target variable with LOG transformation gave me normal distribution, so that’s appropriate transformation. I further explored the relationship visually using scatter plots.
Finally, I used linear regression to build a model to predict Price using other related variables in the dataset and checked for p-value and R-squared values. Second regression model with Log transformation gave me better model compared to previous model. So, I concluded my model with interpretation there.


## Interesting insights

What I found interesting was distribution of Price variable without transformation was skewed and with Log Transformation it appeared like normal distribution. 
Another interesting insight is, Minimum number of nights stay is not impacting the Price of the hotel.

## Limitations 

Though I concluded the final model with Log transformation on target variable, the final model didn’t explain the variance in the dataset completely. It could only explain the variance around 50%, so the predicted price values would be off by a certain amount. Our dataset also has outliers, what if the outliers are genuine values and the model couldn’t fit them completely. 

### [Github Code](https://github.com/sathishmanthani/airbnb-data-analysis/)

## References

[Kaggle - New York City Airbnb Open Data](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data)

