# Ford GoBike System Data
## by Meisam Ashraf


## Dataset

This data set includes information about individual rides made in a bike-sharing system covering
the greater San Francisco Bay area. (https://www.lyft.com/bikes/bay-wheels/system-data)
The original data are available here, under the Bay Wheels License Agreement.

This dataset requires some data wrangling in order to make it tidy for analysis. There are multiple
cities covered by the linked system, and multiple data files need to be joined together for a full
year’s coverage.
At the time of writing this report, there are 26 csv files in the data set covering four years:
- 2017: one csv file covering from 2017-06-28 to 2017-12-31<br>
- 2018: twelve csv files each covering an individual month of the year 2018<br>
- 2019: twelve csv files each covering an individual month of the year 2019<br>
- 2020: one csv file covering the first month of 2020<br>
Data are saved in the workspace directory ‘./data/csv/’.<br>

Each trip is anonymized and is provided in multiple columns of information. I included those columns that are shared for all csv files:
- bike_id: Bike ID<br>
- duration_sec: Trip Duration (seconds)<br>
- start_time: Start Time and Date<br>
- end_time: End Time and Date<br>
- start_station_id: Start Station ID<br>
- start_station_name: Start Station Name<br>
- start_station_latitude: Start Station Latitude<br>
- start_station_longitude: Start Station Longitude<br>
- end_station_id: End Station ID<br>
- end_station_name: End Station Name<br>
- end_station_latitude: End Station Latitude<br>
- start_station_longitude: End Station Longitude<br>
- user_type: User Type (Subscriber or Customer – “Subscriber” = Member or “Customer”= Casual)<br>


## Summary of Findings
The following questions were addressed:
- When are most trips taken in terms of time of day, day of the week, or month of the year?<br>
-  What are the trip duration statistics<br>
-  The number of times the same bike is used throughout the year<br>
-  Does the above depend on if a user is a subscriber or customer?<br>
- How does the above depend on the location for start and end of the trip?<br>

The following findings were observed:
- From the distribution of duration time, we could devide the entries to three groups: short trips, medium and long trips.<br>
- The positions are distributed in three east-west locations.<br>
- There is a visible trend in the weekdays and hours for the rate of bike sharing.<br>
- The weekend, and more used in the mornings and evenings.<br>
- Almost one third of the bikes are heavily used, while others are used less frequently throughout the years.<br>

We have looked at the usage time over the weekdays and daily hours. The trends show that short
trips are mostly used for regular trips in the morning and evening in the working days.
The other observation was the average of the trips that is between 10 and 15 minutes.
Regular users use the system mostly at the working days and the casual customers at the weekend.

## Key Insights for Presentation

- Based on the data set, the trip duration shows a right-skewed ditribution.<br>
- Almost third of the bikes are used heavily through the two years period.<br>
- The subscribers use the bikes mostly in the early morning and evening and the customers are more leveled throughout the day.<br>
- The trend for subscription over 2018-2019 is declining. This is while more customer usage can be seen as we move towards the end of 2019.<br>
- The bikes sharing system is more frequently used in the morning and evening of working day times. While the numbers are fairly uniformly distrinuted along throughout the year, we see less usage at the end of the year.<br>
- The long trips (longer than 2 hours) show a declining trend over time. This is more pronounced for the subscribed users than the casual customers.<br>
- And finally, the interesting trend observed for the months on the weekend show an increase and decreas. End of the year is declining dramatically in duration time.<br>

## Required Resources
The following libraries used in the notebooks:
- numpy<br>
- pandas<br>
- matplotlib<br>
- seaborn<br>
- os <br>
- random<br>
- math<br>
- datetime<br>
- time<br>
- calendar<br>