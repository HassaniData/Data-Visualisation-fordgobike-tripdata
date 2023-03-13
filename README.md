# Ford GoBike System Data
## by Hassani Imane


## Dataset


The Ford GoBike System dataset contains information on bike trips taken using the Ford GoBike bike-sharing system in the San Francisco Bay Area. The data covers the period of feb 2019 with 183412 row and 16 columns, it includes information such as the start and end time of the trip, the start and end stations, the duration of the trip, and the user type (either a subscriber or a customer). Additionally, some demographic information about the users is available, including their age, gender, and the bike they used.

The preliminary data wrangling steps performed before exploration include:

a) Converting categorical variables like bike_share_for_all_trip, user_type, and member_gender to category type for better data representation.
b) Converting start_station_id, end_station_id, and bike_id to str type for easier manipulation.
c) Converting member_birth_year type from float to int type for better data analysis.
d) Converting start_time and end_time types from object to datetime type for easier time-based analysis.
e) Creating new columns start_day and start_hour for better time-based analysis.
f) Creating a member_age column to better understand the age distribution of users.
g) Dropping unnecessary columns such as 'start_station_latitude', 'start_station_longitude', 'end_station_latitude', 'end_station_longitude' to reduce the dimensionality of the data.
h) Replacing the member_birth_year column with the member_age column for better understanding of the user's age distribution.


## Summary of Findings

Summary of findings from exploration 

The majority of users are subscribers, approximately more than 9 times greater than the number of customers.
The bike sharing system is used more by males than females, approximately three times more.
The bike sharing system is least used during the hours of 11 PM to 5 AM when most people are sleeping.
The number of rides during weekdays is higher than during weekends, with the most rides on workdays (Monday to Friday).
The peak hours for using the bike sharing system are from 7 to 9 AM and 4 to 6 PM, which is the typical ordinary working schedule time.
The majority of duration trips values are less than 1500 seconds, and 50% of trip duration takes approximately between 300s and 780s.
The bike-sharing system is used by users of different ages, but it is more concentrated among users between 25 and 40 years old.
The three most commonly used start stations are Market St at 10th St, San Francisco Caltrain Station 2 (Townsend St and 4th St), and Berry St at 4th St.
The three most commonly end stations are San Francisco Caltrain Station 2 (Townsend St and 4th St), Market St at 10th St, and Montgomery St BART Station (Market St at 2nd St).
The top 10 used bikes are used more than 160 times in one month (February), with top three Bike_ids: 4794, 4814, 5175.
More than half of the bikes were used less than 30 times during the month of February.
Subscribed members are taking a higher number of rides during weekdays compared to weekends.
The number of customer riders is significantly lower than that of subscribed riders.
Male riders are taking a higher number of rides during peak hours, specifically between 7-9 AM and 4-6 PM.
None bike sharing for all trips riders are taking a higher number of rides during working days, specifically between 7-9 AM and 4-6 PM.
We can see that most of the customers have a relatively longer trip duration compared to subscribers.
There are more younger riders on weekends compared to other weekdays, and the age group of 20 to 40 years is the most common among riders during working days.
The maximum age of members is around 120 on almost all days except for Monday, which is around 140 (considered outliers).
Duration of trip is uniform across all hours of the day for subscribers.
The relationship between the Age and the Duration of the trip appears to be relatively independent of the User Type, Gender, and bike sharing for all trips. However, other visualizations may provide more interpretable information.


## Key Insights for Presentation


Subscribed members take a higher number of rides during weekdays compared to weekends. This trend is consistent across all genders. In contrast, the number of customer riders is significantly lower than that of subscribed riders and looks uniform across all weekdays. This suggests that customers may be using the bike-sharing service more for leisure or recreational purposes, while subscribers may be using it more for practical purposes like commuting to work.

Riders take a higher number of rides during peak hours, specifically between 7-9 AM and 4-6 PM. This suggests that men may be more likely to use the bike-sharing service for commuting to work or other daily activities.