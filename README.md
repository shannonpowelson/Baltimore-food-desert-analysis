# Baltimore City Food Desert Analysis
## Background
Food deserts are a major problem in Baltimore City, Maryland.  A food desert is described as an area where it is difficult to obtain fresh food.  According to [The Baltimore Sun](https://www.baltimoresun.com/politics/bs-md-pol-lyft-grocery-access-20191118-6wf65ioac5dh5hwjcq3trxzmsm-story.html), “About one in four people in Baltimore lives in a food desert".  Baltimore residents lack access to fresh food in grocery stores.  One solution is public transportation.  Public transportation exists, but not all of the bus routes are free, thus making the bus trip to the grocery store unaffordable for some people.  Baltimore had attempted to solve this problem by offering [subsidized Lyft rides](https://www.baltimoresun.com/politics/bs-md-pol-lyft-grocery-access-20191118-6wf65ioac5dh5hwjcq3trxzmsm-story.html) to grocery stores, but this has not solved the problem.  It still costs money and not everyone has a smartphone that they can use to order the Lyft.  In this analysis, we take a closer look at these food deserts by mapping the grocery stores, street food vendors, and free public transportation routes.  We also investigate the prevalence of different food sources and the food items sold by street food vendors.    

## Business Question
_How are food deserts distributed in Baltimore City, Maryland?_

## Data Sources


## Data Analysis
First we identify the main sources of food in Baltimore City, Maryland.  These main food sources are grocery stores, street food vendors, and restaurants.  We graphed the number of locations of each food source below.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/foodsourcegraph.png)

As shown in the graph, there are many more restaurants than grocery stores and street food vendors.  There are 1,327 restaurants, 77 street food vendors, and 45 grocery stores.

Now we map the grocery stores and free public transportation routes in Baltimore City, Maryland.  The free public transportation routes are the [Charm City Circulator](https://transportation.baltimorecity.gov/charm-city-circulator) routes.  These routes include [the orange line](https://moovitapp.com/index/en/public_transit-line-COMMERCE_STREET_COMMERCE_STREET-Washington_DCBaltimore-142-1196836-4921465-0) (Commerce Street - Commerce Street), [the green line](https://moovitapp.com/index/en/public_transit-line-RUTLAND_AVENUE_RUTLAND_AVENUE-Washington_DCBaltimore-142-1196836-4921464-0) (Rutland Avenue - Rutland Avenue), [the blue line](https://moovitapp.com/index/en/public_transit-line-FORT_MCHENRY_CONWAY_STREET-Washington_DCBaltimore-142-1196836-32493412-0) (Fort McHenry - Conway Street), and [the purple line](https://moovitapp.com/index/en/public_transit-line-PENN_STATION_EAGER_STREET-Washington_DCBaltimore-142-1196836-44580255-0) (Penn Station - Eager Street).  These routes are color coded based on the name of the route.  The grocery stores are labeled with the black map marker.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/grocerymap.png)

As we can see in this graph, the public transportation is concentrated in the middle of Baltimore City and around the inner harbor.  This leaves the rest of Baltimore without any free public transportation to use to get to grocery stores.  


Next, we add the street food vendors to the map (labeled with the light blue map markers).  Our original hypothesis was that the street food vendors would be more widespread throughout Baltimore.  Therefore, even if the food is not healthy, at least there would be more food options for those who cannot make it to a grocery store.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/streetfoodvendormap.png)

However, as shown in this graph, our hypothesis was wrong.  The majority of the street food vendors are clustered around the free public transportation routes and the inner harbor.

Street food vendors have the potential to help solve the food desert problem since they are mobile and can travel to the people in need.  However, is the food healthy?  We graph the different food items offered by the street food vendors.  

![alt text](https://github.com/shannonpowelson/Baltimore-food-desert-analysis/blob/main/StreetFoodVendorsBaltimore.png)

As shown in this graph, the food offerings are not fresh and healthy foods.

## Summary
Overall, from these graphs we can see that the middle of Baltimore and the area surrounding the inner harbor has a great deal of access to transportation in order to get to the grocery stores.  This is important because it shows Baltimore government officials that these areas are likely not the food desert areas.  In order to identify where the food deserts are, future analysis should include research on the percentage of people in community statistical areas who do not have access to a car.  Right now, we can see which areas do not have access to free public transportation, but we also need to see which areas do not have access to cars to truly know if the area is a food desert.  Our map is also important because it shows that the free transportation is concentrated around the inner harbor and the areas that the tourists visit.  Charging tourists for transportation could raise money for free public transportation for Baltimore residents.  In addition, our street food vendor analysis showed that the food offerings are not healthy and fresh food and therefore cannot serve as a solution to people living in food deserts.  However, this does raise an idea for a solution to the food desert problem: healthy food trucks.  Further research could also include smartphone ownership in community statistical areas to see if the subsidized Lyft plan works in these areas.  
