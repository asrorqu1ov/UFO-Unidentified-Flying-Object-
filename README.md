# UFO-Unidentified-Flying-Object-
This dataset contains data on UFO sightings. I analyzed the data and made visualizations.

# Dataset Information

This scrubbed.csv dataset is a collection of UFO (Unidentified Flying Object) sightings from 1906 to 2014.

#### Information about the columns in the dataset
1. **datetime** - The date of the incident, i.e. when and where the UFO incident was seen
2. **city** - The city where the UFO incident occurred
3. **state** - The state or province in which the city is located
4. **country** - The country in which the city is located
5. **shape** - The shape of the UFO How the witnesses saw the UFO
6. **duration (seconds)** - How long the incident lasted (in seconds)
7. **duration (hours/min)** - How long the incident lasted (in hours and minutes)
8. **comments** - Text comments written by the witnesses
9. **data posted** - The date the information about the incident was posted
10. **latitude** - The north-south coordinate of the location
11. **longitude** - The west-east coordinate of the location

#### Columns we added
1. **geolocation** - The coordinates of the location We combined them into one column (we dropped the latitude and longitude columns)
2. **year** - we separated the year from the datetime column
3. **month** - we separated the month from the datetime column
4. **day** - we separated the day from the datetime column
5. **hour** - we separated the hour from the datetime column
6. **minute** - we separated the minute from the datetime column
7. **season** - we separated the months by the month column, this is necessary for analysis and visualization as well
8. **time_of_day** - we determined when the event occurred by the hour column, night or day
9. **light_or_glow** - We created this column to find out whether there was light or not according to the text people wrote when this event occurred, the visualization was used

#### Deleted columns
1. **state** - We got more information from the city and country columns than this, this is unnecessary became and we dropped it
2. **duration (hour/min)** - Since there was a duration (seconds) column, this column became irrelevant to us and we took the main information from the duration seconds column
3. **comments** - After we found out whether there was light when the incident occurred or not, this column became unnecessary and we dropped it
4. **latitude** - We combined the coordinates into one column
5. **longitude** - We combined the coordinates into one column
