# README

Is New York City the City that Never Sleeps?
New York City has been called many things: “The Big Apple,” “Gotham,” “the Concrete Jungle.” And who could forget: “The City that Never Sleeps.” Frank Sinatra whipped the slogan to a frenzy in his 1979 song “New York, New York,” and it stuck. Since then, media around the world have embraced the catchphrase, painting pictures of NYC’s round-the-clock transit, all-night restaurants and people forever in the streets. 

But does New York City deserve the title? And if so, where precisely does the party never stop? The accuracy of New York City’s nickname boils down to three parts: The hours of it transit system, businesses and people. While, its 24-hour subway system is indisputable, at least one question remains: Do NYC restaurants and nightlife spots operate later than in other American cities? 

# The data

Since I’m interested in New York City, I wanted to compare it to the three other largest cities in the U.S. by population: Los Angeles, Chicago and Houston. Plus Las Vegas because of its reputation for nightlife. 

To collect the data, I’m using Yelp, a popular business directory and crowd-sourced review forum, which specializes in restaurants in nightlife establishments. Yelp allows anyone to access its data using the Yelp Fusion API. Its business search feature will return up to 1000 businesses based on search criteria, such as location or category.

While it would have been nice to download data for all businesses in each city, because of Yelp’s 1000-item result limit, I had to come up with a way to geographically sample the data. To do this, I divided each city by its zip code areas and calculated the latitude and longitude of each zip code’s center point. I then asked Yelp to return 50 businesses within 1000 meters of each coordinate. 

After I had my list of restaurants from Yelp per city, I queried the API one more time and asked it to go find each restaurant and return its hours of operation. I used the same methodology to collect data about nightlife venues. 
 
# Current status

I’m still collecting the data. Although I performed some preliminary analysis on NYC and LA.

# New York City
Restaurant closing hour rates:
Mean = 5.9 (11ish)
Median = 5.86 (10:45ish)
Mode = 5.29 (10ish)
The standard deviation of NY closing hours is 1.916. 
# Los Angeles 
Restaurant closing hour rates:
Mean = 4.495 (9pm ish)
Median = 5.0 (10pm)
Mode = 0.0 (?)
The standard deviation of LA closing hours is 2.458.

# Sketch of what the final project might look like, noting any interactivity

Small multiples of choropleth maps of each city
Histograms of the closing hours of each city
Scrollytelling 
Interactive map? 
 

