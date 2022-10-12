# Project 2 Summary

This week I turned in Project 2, which was a group project this time. The purpose of the assignment was to create a vignette about contacting an API of our choosing from a list of seven options.

One of the hardest parts of this assignment was choosing the API. Some of the APIs had an overwhelming amount of information and some of the APIs had a lot of information that wasn’t going to be easy to use in order to meet the parameters of the assignment. My partner and I decided to go with a “write what you know” strategy and decided to work on the food data API. This API has an enormous amount of information about recipes, grocery costs, and nutritional information. We decided to work with just a small subset of the API and focused on Wine Data. (Again, write what you know.)

Once we decided on a topic, we decided to split the project up into three main parts. The first part was wine recommendations, where the user inputs a type of wine, the maximum price of the wine, and a minimum user rating for the wine, along with a max number of records to return. We then created several charts and tables off of this data. The second part was creating a wine pairing function where the user can add a particular type of food and get a recommendation of a wine to go with their dinner. The third function we created looked at if you had a particular wine, what food would go best with it.

I worked mostly on the wine recommendation function. The trickiest part of the programming logic for me was getting the data into a useable format from the API. I found contacting the API to be fairly easy to do, but the data was returned in lists. Here I used the `lapply` function to apply the function to a list of wines. Then, I discovered a new-to-me `dplyr` function called `bind_rows` along with `as.dataframe` to get the list into a single dataframe. The other thing I struggled with just a bit was putting a correlation line onto a 'geom_point()'. I had initially put the color coding in the global aesthetic which caused R to make a correlation plot for each of the colors. By putting the coloring aesthetic into one of the layers, I was able to easily overlay a correlation plot. 

In approaching a similar project in the future, I don’t think there’s a whole lot I would change. My partner and I worked very well together once we had a clear plan. I think narrowing down the API to just a small subset made the vignette more manageable and allowed us to clearly explain our processes.

Our Wine Data Vignette API vignette can be found [here]( https://kbelkna.github.io/Project2/).

The link to our github repository can be found [here]( https://github.com/kbelkna/Project2).
