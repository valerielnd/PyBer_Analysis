# PyBer_Analysis

## Project overview

This project aims to perform an exploratory analysis on the data of a python-based ride-sharing 
app company named Pyber. The goal is to showcase the relationship between the type of city, 
the number of drivers and riders, and the percentage of total fares, riders, and 
drivers by type of city. The analysis and visualizations produced will help PyBer improve 
access to ride-sharing services and determine affordability for underserved neighborhoods.

The list of deliverables for the project is:

- 	Create a bubble chart that showcases the average fare versus the total number of 
	rides with bubble size based on the total number of drivers for each city type, including 
	urban, suburban, and rural.
	
- 	To demonstrate the relevance of the data, compute summary statistics for:	
	* The total number of rides for each city type.
	*  The average fares for each city type.
	* The total number of drivers for each city type.

-	Create box-and-whisker plots that visualize each of the following:
	* The number of rides for each city type.
	* The fares for each city type.
	* The number of drivers for each city type

## Resources

To realize the analysis, we are given access to two large CSV files containing four months
of rideshare data:

[city_data.csv](https://github.com/valerielnd/PyBer_Analysis/blob/main/Resources/city_data.csv)

[ride_data.csv](https://github.com/valerielnd/PyBer_Analysis/blob/main/Resources/ride_data.csv)

We use Python libraries Pandas and Numpy to inspect, merge and perform calculations on the
data and Matplotlib to produce publication-quality figures to tell a visual story from
the data.

[First analysis file](https://github.com/valerielnd/PyBer_Analysis/blob/main/PyBer.ipynb)

[Second analysis file](https://github.com/valerielnd/PyBer_Analysis/blob/main/PyBer_Challenge_starter_code.ipynb)

## Analysis Results

### Bubble chart that showcases the average fare versus the total number of rides

This bubble chart showcase the average fare for each type of city on the y-axis,
the total number of rides for every kind of city on the x-axis and the size of each
marker correlates to the average number of drivers for each type of city.

As we can see in the figure below, there are three types of cities:
- Urban
- Suburban
- Rural

The total number of rides is smaller in rural cities and more significant in urban cities. 
In contrast, the average fare is more outstanding in Rural cities and less in Urban cities. 
Also the number of drivers is greater in urban cities among the three type of cities.

![bubble_chart](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/Fig1.png)

### Mean, median and mode for each type of cities

#### Summary Statistics for Number of Rides by City Type

We computed the mean, median, and mode of the number of rides by city type to
help the company decide which type of cities need more driver support.

![mean_ride](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/ride_mean.png)

The results confirmed the information showcased in the bubble chart; on average
there are more rides in urban cities, followed by suburban cities and rural 
cities.

#### Summary Statistics for the Fare by City Type

We computed the mean, median, and mode of the number of fares by city type to 
determine which city types are generating the most money.

![mean_fare_urban](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/mean_fare_urban.png)

![mean_fare_surburban](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/mean_fare_surburban.png)

![mean_fare_rural](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/mean_fare_rural.png)

The results confirmed the information showcased in the bubble chart; on average 
the fare price for rides is greater in rural cities followed by suburban cites
and urban cities.

#### Summary Statistics for the Number of Drivers by City Type

We computed the mean, median, and mode of the number of drivers by city type to
help the company decide which type of cities need more driver support.

![mean_driver_urban](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/mean_driver_urban.png)

![mean_driver_surburban](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/mean_driver_surburban.png)

![mean_driver_rural](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/mean_driver_rural.png)

The results confirmed the information showcased in the bubble chart; on average 
the number of drivers is greater in urban cities followed by suburban cites
and rural cities.

### Box-and-Whisker Plots for Ride Count Data

The Box-and-Whisker Plots for Ride Count Data let us visualize the summary statistics for the 
number of rides per city type and determine if there are any outliers.

The box-and-whisker plot has all three individual box-and-whisker plots with the 
city type on the x-axis.

![box_and-whisker_ride](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/box_ride.png)

There is one outlier in the urban ride count data, the city of West Angela. Also, 
the average number of rides in the rural cities is about 3.5-4 times lower per 
city than the urban and suburban cities.


### Box-and-Whisker Plots for Ride Fare Data

The Box-and-Whisker Plots for Ride Fare Data let us visualize the summary statistics for the 
ride fares per city type and determine if there are any outliers.

![box_and-whisker_fare](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/Fig3.png)

We see that there are no outliers. However, the average fare for rides in the rural cities 
is about $11 and $5 more per ride than the urban and suburban cities, respectively. 

### Box-and-Whisker Plots for Driver Count Data

The Box-and-Whisker Plots for Driver Count Data let us visualize the summary statistics for the 
number of drivers per city type and determine if there are any outliers.

![box_and-whisker_driver](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/Fig4.png)

The average number of drivers in rural cities is nine to four times less per city than in urban 
and suburban cities, respectively

## Challenger overview	

The challenge's goal is to create a summary DataFrame of the ride-sharing data by city type.
Then using Pandas and Matplotlib, we need to create a multiple-line graph that shows the total 
weekly fares for each city type. Finally, to conclude, we need to provide a written report summarizing 
how the data differs by city type and how decision-makers can use those differences at PyBer.


## Challenge analysis results

### Ride-sharing summary DataFrame by city type

The summary DataFrame provides the total number of rides, the total number of drivers,
the total fares for each type of city, the average fare per ride, and the average fare 
per rider for each type of city.


![Ride_share_summary](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/pyBer_df_summary.png)

The table presents a concise report of the data analyzed and gives key information about
each type of city.

Urban cities have by far a more significant number of rides and drivers and, as a result, 
a greater total fares. However, as rural cities have fewer drivers and rides, they have
a greater average fare for drivers and per ride. Suburban cities stand in the middle
with a total number of rides five times greater than rural cities and about 2.5 times less than 
urban cities.

### Multiple-line chart of total fares for each city type

The multiple-line graph shows the total fares for each week by city type.

First of all, we notice that urban cities, as expected, have the greater total fares per week
among the three types of cities. From January to April, the amount is, on average, over 
$2000 except in some week in January, march and start to decline at the end of 
April. The total fare for suburban cities per week from January to April varies between
$750 and $1500. It drops to the lowest amount at the beginning of January and the middle
of April. The total fare per week for rural cities is the lowest among the city types. The
amount rarely reaches $500 and has the lowest amount in the first week of January.

Also, each city type reaches its highest total around the third week in February.

![chart_line](https://github.com/valerielnd/PyBer_Analysis/blob/main/Analysis/PyBer_fare_summary.png)

## Summary

PyBer can use the result of those analyses to improve their services to each type of city by
deciding which cities need more driver support, which ones are generating the most money
and which need more driver support.

