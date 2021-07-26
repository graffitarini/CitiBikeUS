# CitiBikeUS

In this project, we will be exploring data associated with the New York City bike share program, Citi Bike! Remember, it may be easiest to read these instructions by clicking on the "Preview" button in RStudio.

There are over 850 Citi Bike stations in New York City; users check a bike out from a starting station and then dock that bike at a different station when they reach their destination. Citi Bike offers a variety of memberships, but most memberships allow for trips between 30 and 45 minutes; this will be relevant once we start digging into the dataset.

Citi Bike publically releases a variety of datasets. We've included a dataset containing information about individual trips from January of 2020. If you'd like to download a more recent dataset, or investigate other data that Citi Bike provides, take a look at their [System Data](https://www.citibikenyc.com/system-data) page. 

Visualization 

This case study shows average speed of every age in our dataset. Utillizing ggplot2 to make a line graph we conclude that younger people really do bike faster. This visualization gives us some great insights on how Citi Bike users are using their bikes. 

![Average speed of City Bike users](https://user-images.githubusercontent.com/29014874/126963114-578c98fa-18ae-4d36-9dd0-b465b6eeef0e.png)

Average Citi Bike Users Speed by Gender in January 2020

![Avg speed of two genders](https://user-images.githubusercontent.com/29014874/126963857-bcb30114-f05d-4912-917f-da08da745f74.png)

It looks like we have some unusual data around the age of 50. It looks like there are a ton of bikers with an unknown gender at that age. This might be something we want to dig into a bit more. We filtered out bikers with an age over 100 — that seems like an error in data collection as well.

![final-average speed](https://user-images.githubusercontent.com/29014874/126964034-7f39867e-8d8d-4dcc-b296-9a199090af94.png)

This could be a valuable asset in helping Citi Bike understand how to make bike riding safer in New York. However, there is so much more you can do with this data!

To begin, there are some major flaws in the way we calculated the speed. Specifically, we made some huge assumptions when calculating the distance of each bike ride. Instead of calculating the straight line distance using the geosphere library, we could take advantage of a service like Google Map’s API to get a more accurate measurement of distance. If you’re interested in look more into this problem, investigate getting a Google Maps API key and using a library like gmapsdistance.

Another great way to extend this project is to investigate other data that Citi Bike makes available. We used data found in the Citi Bike Trip Histories section on the System Data page. On the System Data page, you can find different dataset, including information about membership data and real time station data. You could use this real time data to track how the flow of bikes changes over the course of the day. You could investigate how the weather impacts membership. We would love to see any graphs or insights you produce!
