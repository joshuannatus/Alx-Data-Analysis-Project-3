# (Ford GoBike Data Visual Exploration)
## by (Joshua Nnatus)


## Dataset

> The Bay Area's bikeshare program is called Ford GoBike was introduced in 2013, and have featured thousands of bikes and across 70 stations around San Francisco. The Ford GoBike uses a fleet of strong, durable bikes that are secured into a system of docking stations spread out over the city. This document explores individual rides made in a bike-sharing system covering the greater San Francisco Bay area.
This dataset is the ford Bikeshare for the month of Feburary 2019. The dataset consisted of 183412 rows and 16 columns
>
>`Source:` [Ford GoBike System Data](https://www.google.com/url?q=https%3A%2F%2Fvideo.udacity-data.com%2Ftopher%2F2020%2FOctober%2F5f91cf38_201902-fordgobike-tripdata%2F201902-fordgobike-tripdata.csv&sa=D&source=docs "Click here to download the data used for this analysis and visualization")

### Data Wrangling
I cleaned the following issues
#### Quality issues 
> 1. Missing values in member_gender, member_birth_year, end_station_id, start_station_name, start_station_id and end_station_name
> 2. Start_time, and end_time should be datatime datatype
> 3. bike_share_for_all_trip, User_type and member_gender should be catergory datatype 
> 4. The member_birth_year, start_station_id and end_station_id is having a decimal value and has a wrong data type

#### Tidiness issues
> There are no tidiness issues:

#### Feature Engineering
> Every cell is a single value and every rows and columns forms a table
> 1. But I want to create a feature age and see if we can further turn it to a categorical feature of young and old or more
> 2. Distance covered for each member
> 3. Create a column for Start month, end month, day of the week, minutes and hour of trip duration

## Summary of Findings

> Thursday had the highest usage in the month of february, closely followed by Tuesdays, and Fridays. Saturdays and Sundays showed a signficant drop of usage. This points to that bikes are mostly used on Weekday and/or that people are more inclined to stay home during the weekend hence reduced use of bikes and are most likely to start bike rides from the hours of 8am to 9am, suggestive of the fact that they would want to go to work or something, and it declines and peeks at 17:00 or 5pm to 18:00 or 6pm people trend to start riding the bike. This is great but requires further investigation

> Furthermore, during the work days Mondays to Friday start there ride between the 5 and 10 am in the morning (This suggestive that they ride bikes to work), 3pm and 8 pm in the evening (this is suggestive that the start riding the bike home after close of work). The weekend shows that at people mostly take bike rides between the hours of 10 am and 3pm. It is suprising also to note that ages 30 to 35 and between the hours of 3 pm to 8pm showed the highest starting hours for the use of bikes. 

>Subscription use is significantly higher than total consumer usage. Customers and subscribers have quite different riding habits and patterns. Most trips on work days (Mon-Fri) and especially during rush hours (when going to work in the morning and getting off work in the afternoon) were made by subscribers because they use the bike sharing system for commuting, whereas customers typically ride for fun in the afternoon or early evening on weekends. Regular rush hours are when most subscribers use the service at its height, which enhanced their intention to use it and their motivation to ride.

## Key Insights for Presentation

> There is an intresting finding here, knowing that most user, use the bike for all trip, the plot above shines a different light on the data, ratherless of most users using bike for all trips and most gender been male, we can see that the other gender aside male and female have the highest average distance covered for using bike for all trip and that customer users have average distance covered for the month of feburary. People who don't use bikes for all trips trend to cover higher average distances