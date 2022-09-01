# surfs_up

## Overview
The purpsose of this challenge was to gather the temperature trends for the months of June and December in Oahu to see if it was advisable for the surf/ice cream shop to be all year-round.

## Results
### Month of June
* The average temperature is 74.94 degrees.
* At the lowest point it reached 64 degrees.
* The highest temperature of this month was 85 degrees.

### Month of December
* This months average is 71 degress which is somewhat cooler than June.
* The 50 and 75 percents are 71 and 74 degrees respectively.
* At its lowest point, the temperture decreased to 56 degrees.

## Summary
The data for June shows that it would be a given that the shop would thrive throught the month. It also showed that it stay relatively warm the whole month. 
From the data gathered, it shows that Oahu during one of the coldest months of the year is still somewhat on the warmer side. This would mean that buisness should be able to run throughout the whole year. 

Another point of data to gather is percipitation. The following code will allow you to do this for both months:
### June

session.query(Measurement.date,Measurement.prcp).filter(extract('month',Measurement.date)==6).all()

### December

session.query(Measurement.date,Measurement.prcp).filter(extract('month',Measurement.date)==12).all()

Both of this would be put in place of the temperature filter.
