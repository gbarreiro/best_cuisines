# Best Cuisines in Town
## Introduction
There are plenty of well-know cuisines around the world, like the Chinese, Japanese, Mexican, Spanish... It might be obvious that the best place to taste Mexican food is Mexico, and so on, but it might be very tedious to visit so many countries to taste each different cuisine. With this solution, foodies will be able of trying the best dishes of international cuisine without having to visit every single country. Moreover, this project will give people interested in migration movements an insight into how people from some nationalities move to specific cities and open restaurants where they prepare the food from their countries.

In this project, we'll explore the cities of New York, Tokyo, Hong Kong, Sydney, Barcelona, Paris, Moscow, Buenos Aires and Mexico DF, in order to find which are the top 5 cuisines on each city, and which city is the best to try each cuisine.

## Data
For this project, we'll use the [Foursquare API](https://developer.foursquare.com). For each city mentioned above, we'll ask the API for the restaurants (endpoint `/venues/explore?section=food&near=city_name`), and get for each restaurant (`response.groups[0].items[]`) the type of cuisine from the `venue.categories` field. 

Then, we'll be able of extracting a top 5 of cuisines for each city, and plot them in a bar graph. For each cuisine, we'll be able of showing the cities where there are more restaurants.