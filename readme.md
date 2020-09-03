# Ford GoBike System Data Exploration

## Introduction
This document explores a dataset that includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. it covers the first quarter of 2020. [Download here](https://www.lyft.com/bikes/bay-wheels/system-data), you'll find Bay Wheels's trip data for public use.
<br/>
In this project we will gather on real-world data to wrangle, explore, analyze, and comunicate our findings about Bay Wheels's trip data. We will do an exploratory analysis to answer the following.

* When are most trips taken in terms of time of day, day of the week, or month of the year?
<br/>
* How long does the average trip take?
<br/>
* Does the above depend on if a user is a subscriber or customer?



## Dataset
### The Data
Each trip is anonymized and includes:
- Trip Duration (seconds)<br/>
- Start Time and Date <br/>
- End Time and Date <br/>
- Start Station ID <br/>
- Start Station Name
- Start Station Latitude
- Start Station Longitude
- End Station ID
- End Station Name
- End Station Latitude
- End Station Longitude
- Bike ID
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
- Rental access method (using app or clipper, clipper is the all-in-one transit card for the Bay Area)


## Summary of Findings

### Talk about some of the relationships you observed in this part of the investigation. Were there features that strengthened each other in terms of looking at your feature(s) of interest?
I extended my investigation of the three vatiables date-time (Months, Days, Hours), user type, trip duration (min) in this section by looking at the impact of it on the trips..
To answer the following 
* When are most trips taken in terms of time of day, day of the week, or month of the year?
* How long does the average trip take?
* Does the above depend on if a user is a subscriber or customer?
The findings was just as we expected. 

### Were there any interesting or surprising interactions between features?
Looking back on the point plots, the time-date and user-type features has an effect on the trips. However, there were no relation between the rental method and the user type. Overall, the results match our previous observations and expectations.  

### Key Insights 
- The the bike is rented for about 5-10 minutes. Moreover, the average renting time according to the statistic summary is 12 minutes.
- 92.33% of the bike rental methods are by app and only 7.67% are rented by clippers (transit card).
- 86.11% of the users are subscribers while 13.88% of them are customer!
- February is the top month for bike trips.
- Most of subscribers trips has two peak hours at 8:00pm and 17:00pm which is work-time (I'm assuming people go to and come from work at these hours). Meanwhile, the customers distribution entails that the trip count increases as the day progresses from 14:00 until 17:00pm which is the peak time too.
- The subscriber type has consistency throughout the week days with averaage duration 5-10 minutes while, the customers type has higher duration (over 20 min trip duration) during the weekends. 
- Both subscribers and customers rented bikes by app, however, both have a relatively small number of trips rented using clippers.




## Key Insights for Presentation

For the presentation, I focus on the vatiables `date-time (Months, Days, Hours), user type, trip duration (min)` by presenting the the impact of it on the trips..
To answer the following 
* When are most trips taken in terms of time of day, day of the week, or month of the year?
* How long does the average trip take?
* Does the above depend on if a user is a subscriber or customer?
The findings was just as we expected. 

## Built With
* `pandas`, `NumPy`, `requests`, `Image`, `os`,`matplot`

## Acknowledgement 
Udacity's Data Analyst Developer - Connect Nanodegree Program with MISK Foundation
