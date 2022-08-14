# ****Surfs_up****
## Overview of Project
- The purpose of the project is to provide analyzed temperature trends of Oahu, Hawaii for a potential business venture in the surfing shop market to see if it is a lucrative business option. 
## Results:
- The average temperature in Oahu during June is ~3.86°F higher than the temperature in December.
- The lowest temperature in June is 64°F whilst in December it is 56°F. 
- There are 10.7% less data points in December than June.

![june_results](https://user-images.githubusercontent.com/106709942/184557386-b0eab417-44d6-4672-9d96-77fb4694e08f.PNG)
![December_results](https://user-images.githubusercontent.com/106709942/184557397-e35c58dd-de4f-4906-a55f-fd3ed4baf522.PNG)

## Summary:
Based on the temperature results above, It can be expected that there will be some seasonal fluctuations in sales, however, the temperatures are mainly stable leading to this venture being a possible profitable business. 

## Additional Queries:
- Other queries to add to this Analysis is the following:
  - Bad Weather such as rain is a major variable that can cause decrease in sales, thus, being able to see the precipitation statistics would be a benefical to the decision making process.
  - June
    - session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 6).all() 
  - December
    - session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 12).all()
