# Ford Go Bike Dataset Exploration
## by (ODINIGWE CHINYERE ROSEMARY)


## Dataset

> Ford GoBike, like other bike share systems, consists of a fleet of specially designed, sturdy and durable bikes that are locked into a network of docking stations throughout the city. The bikes can be unlocked from one station and returned to any other station in the system, making them ideal for one-way trips. The bikes are available for use 24 hours/day, 7 days/week, 365 days/year and riders have access to all bikes in the network when they become a member or purchase a pass. This dataset was provided by Udacity and it includes information regarding 183,000 rides made in a bike-sharing system covering the greater San Francisco Bay area. The data features include trip duration (secs),trip start and end time,start and end stations,customer type, gender, birth year and some additional variables.

### Data Wrangling
Here is a summary of my data cleaning process

- Dropped missing values
- Converted each features with incorrect data type to the appropriate data type
- Generated new features such as duartion(min),age,dayoftheweek,hour of the day from duration(sec), birth year and trip time respectively


## Summary of Findings

> ### Univariate Exploration Findings
- User type- The subscribers were more than the customers
- Member_gender- We had more male users compared to the female gender and insignificant number of trips belonging to other gender
- Age- The predominant age group was between 25 and 35 years. 
- Bike_share_trip- Majority of the users are not subcribers of the bike share program
- Duration -Most trip duration was between approximately 5-25mins, this information was obtained after plotting on a log scale and setting the xlim to 100minutes.
- Weekdays/hr- The bike rental system was found to have its peak usage on Thursdays and Tuesdays around the hours of 8-9am and 5-6pm with trip duration of about approximately 5-25mins. The most frequently used start station is Market St at 10th S
- The top 3 start stations are Market St at 10th St','San Francisco Caltrain Station 2  (Townsend St at 4th St)',and'Berry St at 4th St'

> ### Bivariate Exploration Findings
- Duration vs Usertype: The users who are **Customer** have longer bike trip on average as compared to users who are **Subscribers**.
- Duration vs gender: The **Female** users have longer bike trip on average as compared to **Male** users.
- Duration vs Bike share program: The non members on average,have longer trips compared to members of the program.
- Duration vs day of the week: Weekend trips(Sat & Sun) have longer durations on average as compared to trips taken during weekdays(Mon-Fri)
- Duration vs hr of the day: The trips taken between 8AM to 5PM is observed to have longer durations on average as compared to other times of the day.
- Age vs Usertype: The average age of the **Customer and Subscriber** users is approximately same.
- Age vs Gender: The average age of the **Male** users is higher than the average age of the **Female** users.
- Age vs Bike share program: The average age of non members is higher than that of the members. 
- Age vs day of the week: The average age of weekend users (Sat & Sun) is lower than the average age of the weekdays(Mon-Fri) users.
- Age vs hr of the day: The average age of the users whose trip starts at 4AM is considerably higher than the average age of the other users.There isnt any significant change in the average ages of users whose trips starts between 5AM to 8AM.Overall,the average age of the users whose trips start between midnight and 3AM is lower than the other time frames

> ### Multivariate Exploration Findings.
- Customers have higher average trip duration for all days of the week and hours of the day, although they spend longer times on weekends than on weekdays
- Female users have higher average trip duration for all days of the week and almost all hours of the day except for 5am where the male users spend longer time. The female users also spend longer times on weekends than on weekdays.
- Customer user type trips is characterised by younger users with longer duration and subscribers are characterised to be composed of older users with shorter durations
- The users of the top 3 start stations are characterised by consiting of Male subcribers whose average age is greater than the other genders, Although comparing the female gender numbers, Market st at 10th station has more female users than the other stations.

## Key Insights for Presentation

> For this presentation,i will focus on the distribution of the key features of interest such as 
- The user demographics with respect to age,usertype and gender.
- The distribution of trips across days of the week and hours of the day.
- Usertype and gender relationship with duration and age
- The duration of user type and genders across the days of the week
- The top 3 stations and its relationship to usertype and gender
