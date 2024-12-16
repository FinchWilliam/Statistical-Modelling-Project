# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Our goal here was to build out a regression model by looking through several API's (yelp, foursquare and citibikes(https://citybik.es/)) to look through and find some links. 
I decided to hypothesis that the Restaurants ratings are linked to the number of bike stations nearby.


## Process
1. We first link to the Citibikes API and grab all bike data for Miami
2. Then we will link to Yelp and Foursquare to grab all restaurants near the bike depot's
3. We will build a database of all that information to have easy access to it all as needed.
4. Finally we will run a regression model on the data and dive through our results.

## Results
On analysis we found a much more complete set of information (with categories such as price and rating) from Yelp so I chose to run my tests using them. 

Final regression model showed us a a 32% chance of being significant with a insignificant p value and lastly it helped us see that for ever 1 extra bike station we would have a .1859 raise in restaurant star

![image](../images/ols_regression_results.png)

now obviously there are many other external factors at play here and we would be able to find many other reasons why the restaurant has those stars.


## Challenges 
I have worked through a few different challenges, 
 - connecting to the different API's (and working inside the call limits they have set)
 - interpreting the json files I get back, and deciding what information was worth keeping and storing and what was not.
 - creating a database from scratch and deciding what should be a primary key and foriegn key and how they should be seperated.
 As you can see as you go through the files I have learnt at every step of the way (sometimes going back and re-doing certain parts after learning new things, so if you wonder why I did something then dropped it soon later it is because it wasn't needed at a later date) and managed to rise to and overcome these challenges

## Future Goals
 - eventually I would like to fully normalize the database, it was put together quickly and it could be set out nicer.
 - run some more models across the different features, a classification model with the price, run the same model in reverse, do higher rated restaurants get more bike staions, etc.
 
