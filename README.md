# Housing Prices Analysis and Prediction of GTA
1. Introduction: Business Problem 
    As a resident of the Greater Toronto Area (GTA) for more than 10 years, I'd like to choose GTA data as my Applied Data Science Capstone Project. The basic idea is using the Venues Data and School Rankings to predict Housing Price. Also, look into some relationship or patterns between different factors.

    Toronto is the largest city in Canada, however, compare with those largest cities in the world, we have only 6 million people live in it, most of which lives and works in the south area. The population density and diversity are our unique features, that makes some of the parameters in our project needs to be customized.

    When we have all of the data and the models, we can create some visualization graphs to check those patterns and compare the performance among different models. We can also create a map to map each district is clustered according to the features like school ranking and venue density.

2. Data 
    At first, I took me hours to build a quick draft model: with only the data I gathered from some realtor website using web scraping method, then use foursquare API to combine each of the house records with Venues Data. However, the accuracy of the performance does not look great.

    The biggest issue is unlike in the US, here in Canada all of the sold price and most of the important detail information such as build year, sqrt, land size, property tax, are not opened to the public, so there's no good solution to get all of the data I required through open source.

    So the next step is to try to find other related could affect the housing price, in order to do so, I went through other websites including official school ranking for 2017-2018 provided by Fraser Institute, since just as many of other parents, the ranking of the school is one of the biggest concerns when we purchased our own house. Also, I chose a listing website for an approximate size and type for each of the property.

    Please note there's two way to get latitude and longitude information: I tried Google API and web scrapping, both worked.

    Eventually, here the key datasets I used:

    School Ranking Dataset - Obtained from the Fraser Institute website through web scraping methods

    The name of schools
    Cities of schools located
    2017-18 Rating of Elementary Schools
    Postcodes of schools
    Addresses of schools
    Housing Info Dataset - Obtained from residences listing websites through web scraping methods

    Addresses of houses
    Number of bedrooms for each house
    Number of bathrooms for each house
    Postcodes of houses
    Latitudes
    Longitudes
    The names of Neighborhood
    The type of the residences: House/Townhouse/Condo
    Listing prices
    Approximate sizes: Better than nothing, since I couldn't find an easy way to get the exact size of each residence
    Venues Data Dataset - Obtained through Foursquare API

    Counts of Venues closed to the Neighborhood
    The frequency of each Venues Category such as Office, Bus Stop, Pizza Place, Coffee, Chinese Restaurant, Italian Restaurant, etc.
