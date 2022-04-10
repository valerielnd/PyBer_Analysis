# PyBer_Analysis

## Project overview

This project aims to perform an exploratory analysis on data of a python based ride-sharing 
app company named Pyber. The goal is to showcase the relationship between the type of city 
and the number of drivers and riders as well as the percentage of total fares, riders and 
drivers by type of city. The analysis and visualizations produced will help PyBer improve 
access to ride-sharing services and determine affodability for underserved neighborhoods.

The list of deliverables for the project is:

- 	Create a bubble chart that showcases the average fare versus the total number of 
	rides with bubble size based on the total number of drivers for each city type, including 
	urban, suburban, and rural.
	
- 	To demonstrate the relevance of the data, compute summary statistics for:	
	•The total number of rides for each city type.
	• The average fares for each city type.
	• The total number of drivers for each city type.

-	Create box-and-whisker plots that visualize each of the following to determine if there are any outliers:
	• The number of rides for each city type.
	• The fares for each city type.
	• The number of drivers for each city type

## Resources

To realize the analysis, we are given access to two large csv files containing four months
of rideshare data:

[city_data.csv]()

[ride_data.csv]()

We use Python libraries Pandas and Numpy to inspect, merge and perform calculations on the
data and Matplotlib to produce publication quality-figures to tell a visual story from
the data.

[First analysis file]()
[Second analysis file]()

## Analysis Results

### Bubble chart that showcases the average fare versus the total number of rides

This bubble chart showcase the average fare for each type of city on the y-axis,
the total number of rides for each type of city on the x-axis and the size of each
marker correlate to the average number of drivers for each type of city.

As we can see in the figure below, there are three types of cities:
- Urban
- Surburban
- Rural

The total number of rides is smaller in rural cities and greater in urban cities 
whereas the average fare is greater in Rural cities and less in Urban cities. Also 
the number of drivers in greater in urban cities among the three types of cities

![bubble_chart]()

### Mean, median and mode for each type of cities

#### Summary Statistics for Number of Rides by City Type

We computed the mean, median and mode of the number of rides by city type to
help the company decide about which type of cities need more driver support.

![mean_ride]()

The results confirmed the information showcased in the buble chart, on average
there are more rides in urban cities followed by surburban cities and rural 
cities.

#### Summary Statistics for the Fare by City Type

We computed the mean, median and mode of the number of fare by city type to 
determin determine which city types are generating the most money.

![mean_fare_urban]()

![mean_fare_surburban]()

![mean_fare_rural]()

The results confirmed the information showcased in the buble chart, on average 
the fare price for rides in greater in rural cities followed by surburban cites
and urban cities.

#### Summary Statistics for the Number of Drivers by City Type

We computed the mean, median and mode of the number of drivers by city type to
help the company decide about which type of cities need more driver support.

![mean_driver_urban]()

![mean_driver_surburban]()

![mean_driver_rural]()

The results confirmed the information showcased in the buble chart, on average 
the number of drivers in greater in urban cities followed by surburban cites
and rural cities.

## Challenger overview	

The goal of the challenge is to create a summary DataFrame of the ride-sharing data by city type.
Then using Pandas and Matplotlib, we need to create a multiple-line graph that shows the total 
weekly fares for each city type. To conclude, we need to provide a written report that summarizes 
how the data differs by city type and how those differences can be used by decision-makers at PyBer.
http://localhost:8888/tree?token=024e497224d4543b5cd13ccc238e6467053b778e3e50fff0

### Ride-sharing summary DataFrame by city type

The summary DataFrame provides the total number of rides, the total number of drivers,
the total fares for each type of city, the average fare per ride and the average fare 
per rider for each type of city.

![Ride_share_summary]()

This table presents a consise report of the data analyzed and give key information about
each type of city.

Urban cties have by far a greater number of rides and drivers and as a result a greater total
fares. However, as rural cities have the smaller number of drivers and rides, they have
the greater average fare per ride and average fare for Driver. Surburban cities stand in the middle
with a total number of rides 5 times greater than rural cities and about 2.5 times less than 
urban cities.

### Multiple-line chart of total fares for each city type

The multiple-line graph that shows the total fares for each week by city type.

First of all, we notice that urban cities as expected has the greater total fare per week
among the three types of cities. From juanuaray to april, the amount is on average over 
$2000 dollards exept in some week in january, march and start to decline at the end of 
april. The total fare for surburban cities per week from january to april varies between
$750 and $1500. It declines to the lowest amount at the begining of january and the middle
of april. The total fare per week for rural cities is the lowest among the city types. The
amount rarely reaches $500 and has the lowest point in the first week of january.

Also, each city type reaches their highest total around the third week in february.

![chart_line]()

