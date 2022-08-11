# FordGoBike Data Exploratory Analysis
## by (Oluwadunsin Olajide)


## Dataset

Ford GoBike is the first bike-sharing system introduced in the US West Coast. Its 540 stations and 7,000 bikes sprawl across five cities in San Francisco Bay Area
The dataset consists of 183412 entries of Fordbike trips with 16 columns (duration_sec', 'start_time', 'end_time', 'start_station_id','start_station_name', 'start_station_latitude','start_station_longitude', 'end_station_id', 'end_station_name','end_station_latitude', 'end_station_longitude', 'bike_id', 'user_type','member_birth_year', 'member_gender', 'bike_share_for_all_trip).

The dataset contains some incorrect data types. some cleaning will be carried out to correct the datatypes and remove missing values from the dataset.
The start and end time data types will be changed from object to datatime ns, end_station_id to object, bike_id, start_station_id, end_station_id will be changed to object, bike_share_for_all_trip will be changed from object to boolean.
From the dataset, the start_hour, start_day_of_week and Period of the day will be gotten from the start time. The duration_min will be calculated from duration_sec by dividing the duration_sec by 60.( this is because the trip is priced in minutes, this will make the analysis easier when compared with the user_type). Member age will be calculated from member_birth_year by subracting member_birth_year from 2019 (which is the year under consideration).

The cleaned data used for analysis has the total of 174952 entries of bike trips with 21 columns( the colums gives information about the duration in secs and mins each rider used the bike, start and end time,the day of the week and hours the users used the bike, start and end stations with their latitudes and longitudes, bike id, start and end stations ids, user type( i.e whether the user is a subscriber or customer), bike_share_for_all_trip (this column indicate whether the user is registered for the reduced pricing option), the gender and age.

The dataset can be didvided into categorical and numerical variables.

Numerical variables 

duration_min: the duration of trip in minutes.

member_age: The age of bike users in year.

Categorical are variables

Start_day_of_week
time_of_day
start_hour
day_in_month
user_type
member_gender
bike_share_for_all



## Summary of Findings

The highest bike trip was recorded on Thursday with 33712 trips with the lowest trip on Saturday and Sunday. It appears that people tend to rest during the weekend and go out less often. I can also infer that majority of the people that used the bike system in february go to work majorly during the week and don't have weekend shift or don't work on weekends.

The major bike users in the month february falls with the age range of 30 - 40 years. The age is negatively (slightly) correlated with the duration of trips in minutes as there are less bike users within the older age group. This can be due to the fact that these age group go out less than the younger ones.

The customers have used the bike for a longer duration than the subscribers. Most subscriber use the bike system more during the week and less on Saturday and Sunday while the customers use the bike almost at the same rate on any day of the week. The bike usage is mostly used in the morning and afternoon. None of the customers registered for bike share for all trips option, this further explain that they dont us the bike system regularly and so they did not see reason to subscribe or register for the price reduction option.

## Key Insights for Presentation
<ol>
   <li> Distribution of Trips based on User_type </li>

   <li>   Age Distribution of Bike Users </li>
    
   <li>   Duration of Trip </li>
   <li>   Distribution of user type and day of week </li>

   <li>  Age and Duration Distribution with respect to User Type </li>
</ol>