# Baltimore City Food Desert Analysis
## Background
Food deserts are a major problem in Baltimore City, Maryland.  A food desert is described as an area where it is difficult to obtain fresh food.  According to [The Baltimore Sun](https://www.baltimoresun.com/politics/bs-md-pol-lyft-grocery-access-20191118-6wf65ioac5dh5hwjcq3trxzmsm-story.html), “About one in four people in Baltimore lives in a food desert".  Baltimore residents lack access to fresh food in grocery stores.  One solution is public transportation.  Public transportation exists, but not all of the bus routes are free, thus making the bus trip to the grocery store unaffordable for some people.  Baltimore had attempted to solve this problem by offering [subsidized Lyft rides](https://www.baltimoresun.com/politics/bs-md-pol-lyft-grocery-access-20191118-6wf65ioac5dh5hwjcq3trxzmsm-story.html) to grocery stores, but this has not solved the problem.  It still costs money and not everyone has a smartphone that they can use to order the Lyft.  In this analysis, we take a closer look at these food deserts by mapping the grocery stores, street food vendors, and free public transportation routes.  We also investigate the prevalence of different food sources and the food items sold by street food vendors.  The goal of this analysis is to determine what kinds of Baltimore City government policies should be implemented in order to solve the food desert problem. 

## Business Question
_What kinds of Baltimore City government policies should be implemented to solve the food deserts problem?_

## Data Question
_How are food deserts distributed in Baltimore City, Maryland?_

## Data Sources

1. Grocery Store

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Grocery_Store%20(2).csv

This data set contains data on the grocery stores in Baltimore City.  The street address, zipcode, city, and state columns are used in the code.  This data can be found [here](https://data.baltimorecity.gov/datasets/grocery-store?geometry=-76.870%2C39.262%2C-76.376%2C39.355) on the Baltimore Open Data website.  

2. Grocery List

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/grocerylist.csv

This data set contains the addresses, latitude, and longitude of the grocery stores in Baltimore.  It was made from the manipulated Grocery Store data set downloaded from the python code.  The latitude and longitude of each address were manually entered using [LatLong.net](https://www.latlong.net/convert-address-to-lat-long.html) and [gps-coordinates.net](https://www.gps-coordinates.net/).

3. Food Vendor Locations

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Food_Vendor_Locations.csv

This data set contains data on the street food vendors in Baltimore City.  The address, latitude, longitude, and items sold columns are used in the code.  The raw data can be found [here](https://data.baltimorecity.gov/datasets/food-vendor-locations-1) on the Baltimore Open Data website. 

4. Restaurants

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Restaurants.csv

This data sets contains data on the restaurants in Baltimore City.  The number of total restaurants was used in the bar graph.  The raw data can be found [here](https://data.baltimorecity.gov/datasets/restaurants?geometry=-77.115%2C39.193%2C-76.126%2C39.379) on the Baltimore Open Data website.  

5. Charm City Circulator Data Sets

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Charm%20City%20Circulator%20-%20Blue%20Line.csv

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Charm%20City%20Circulator%20-%20Green%20Line.csv

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Charm%20City%20Circulator%20-%20Orange%20Line.csv

https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/Charm%20City%20Circulator%20-%20Purple%20Line.csv

These four data sets are for the four Charm City Circulator lines.  The addresses of the bus stops for each line were found on [Moovit](https://moovitapp.com/index/en/public_transit-lines-Washington_DCBaltimore-142-1196836) and entered manually into excel.  Using these addresses, the latitude and longitude were manually entered using [LatLong.net](https://www.latlong.net/convert-address-to-lat-long.html) and [gps-coordinates.net](https://www.gps-coordinates.net/).

## Data Analysis
First we identify the main sources of food in Baltimore City, Maryland.  These main food sources are grocery stores, street food vendors, and restaurants.  We graphed the number of locations of each food source below.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/foodsourcegraph.png)

As shown in the graph, there are many more restaurants than grocery stores and street food vendors.  There are 1,327 restaurants, 77 street food vendors, and 45 grocery stores.

Now we map the grocery stores and free public transportation routes in Baltimore City, Maryland.  The free public transportation routes are the [Charm City Circulator](https://transportation.baltimorecity.gov/charm-city-circulator) routes.  These routes include [the orange line](https://moovitapp.com/index/en/public_transit-line-COMMERCE_STREET_COMMERCE_STREET-Washington_DCBaltimore-142-1196836-4921465-0) (Commerce Street - Commerce Street), [the green line](https://moovitapp.com/index/en/public_transit-line-RUTLAND_AVENUE_RUTLAND_AVENUE-Washington_DCBaltimore-142-1196836-4921464-0) (Rutland Avenue - Rutland Avenue), [the blue line](https://moovitapp.com/index/en/public_transit-line-FORT_MCHENRY_CONWAY_STREET-Washington_DCBaltimore-142-1196836-32493412-0) (Fort McHenry - Conway Street), and [the purple line](https://moovitapp.com/index/en/public_transit-line-PENN_STATION_EAGER_STREET-Washington_DCBaltimore-142-1196836-44580255-0) (Penn Station - Eager Street).  These routes are color coded based on the name of the route.  The grocery stores are labeled with the black map markers.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/grocerymap.png)

As we can see in this graph, the free public transportation is concentrated in the middle of Baltimore City and around the inner harbor.  This leaves the rest of Baltimore without any free public transportation to use to get to grocery stores.  


Next, we add the street food vendors to the map (labeled with the light blue map markers).  Our original hypothesis was that the street food vendors would be more widespread throughout Baltimore.  Therefore, even if the food is not healthy, at least there would be more food options for those who cannot make it to a grocery store.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/streetfoodvendormap.png)

However, as shown in this graph, our hypothesis was wrong.  The majority of the street food vendors are clustered around the free public transportation routes and the inner harbor.

Street food vendors have the potential to help solve the food desert problem since they are mobile and can travel to the people in need.  However, is the food healthy?  We therefore graph the different food items offered by the street food vendors.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/StreetFoodVendorsBaltimore.png)

As shown in this graph, the food offerings are not fresh and healthy foods.

## Summary
Overall, from these graphs we can see that the middle of Baltimore and the area surrounding the inner harbor has a great deal of access to free transportation in order to get to the grocery stores.  This is important because it shows Baltimore government officials that these areas are likely not the food desert areas.  In order to identify where the food deserts are, future analysis should include research on the percentage of people in community statistical areas who do not have access to cars.  Right now, we can see which areas do not have access to free public transportation, but we also need to see which areas do not have access to cars to truly know if the area is a food desert.  Our map is also important because it shows that the free transportation is concentrated around the inner harbor and the areas that the tourists visit.  Charging tourists for transportation could raise money to fund free public transportation for Baltimore residents.  In addition, our street food vendor analysis showed that the food offerings are not healthy and fresh food and therefore cannot serve as a solution to people living in food deserts.  However, this does raise an idea for a solution to the food desert problem: healthy food trucks.  Further research could also include smartphone ownership in community statistical areas to see if the subsidized Lyft plan works in these areas.  Ultimately, additional analysis is needed to determine what kinds of government policies are needed to combat the food desert problem.  
