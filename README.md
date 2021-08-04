# PyBer_Analysis
Module 5 - Matplotlib

## Project Overview

Create a summary DataFrame of the ride-sharing data by city type and a multiple-line graph that shows the total weekly fares for each city type. 


Deliverable 1
- [x] 1. The total number of rides for each city type is retrieved
- [x] 2. The total number of drivers for each city type is retrieved
- [x] 3. The sum of the fares for each city type is retrieved
- [x] 4. The average fare per ride for each city type is calculated
- [x] 5. The average fare per driver for each city type is calculated
- [x] 6. A PyBer summary DataFrame is created
- [x] 6. The PyBer summary DataFrame is formatted as shown in the example


Deliverable 2
- [x] 1. A DataFrame was created to show the total fare amount for each date and time
- [x] 2. A DataFrame was created using the pivot() function
- [x] 3. A DataFrame was created to show data from 2019-01-01 to 2019-04-29
- [x] 4. A DataFrame was created to show the sum of the fares for each week
- [x] 5. An annotated chart showing the total fares by city type


Deliverable 3
- [x] 1. Purpose of the new analysis
- [x] 2. Differences in ride-sharing data among the different city types
- [x] 3. Business recommendations to the CEO for addressing any disparities among the city types


Jupyter Notebook with challenge analysis: [PyBer Challenge Analysis](https://github.com/GabrielaTuma/PyBer_Analysis/blob/282730cc4be3bfc10c0f1823a1ec7df603201af6/PyBer_Challenge.ipynb)

Previous analysis: [PyBer Analysis](https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/PyBer.ipynb)

## Resources 

- City Data: [city_data.csv](https://github.com/GabrielaTuma/PyBer_Analysis/blob/282730cc4be3bfc10c0f1823a1ec7df603201af6/Resources/city_data.csv)
- Ride Data: [ride_data.csv](https://github.com/GabrielaTuma/PyBer_Analysis/blob/282730cc4be3bfc10c0f1823a1ec7df603201af6/Resources/ride_data.csv)
- Software: Python 3.7.6, Visual Studio Code 1.58.1, Jupyter Notebook 6.3.0

## Summary 

PyBer is a ride-sharing app company valued at $2.3 billion and the main purpose of this document is to analyze all the rideshare data from January to early May of 2019 and create a compelling visualization for the CEO, V. Isualize. 

The beginning of the analysis was done previously and it will be used to support this document. 

### The summary DataFrame per city type
In order to summarize the results a DataFrame was created to sort the data per city type: Urban, Suburban and Rural. 
![Type Summary](https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Summary_per_type.png)

This dataframe contains a lot of information that can be better visualized using charts. First, we can see the pie charts representing the percentages of rides, drivers and total amount of fare collected per city type. 

<img src="https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Fig6.png" width="60%" height="60%">
<img src="https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Fig7.png" width="60%" height="60%">
<img src="https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Fig5.png" width="60%" height="60%">

Looking at the table, it is hard to see a trend among the numbers, specially because the units are different and we are analyzing more than one type of data. However, when we look at the pie charts it is clear that the number of rides, drivers and total amount of fare have a high level of correlation. 

In Canada, [more than 80% of the population](https://www.statista.com/statistics/271208/urbanization-in-canada/) lives in urban areas, which explains the high percentages compared to suburban and rural areas in the graphs. We can assume that cities with bigger populations will have more drivers, in order to attend the proportional demand. This demand means more rides, that generate more total fare amount.  


Looking at the DataFrame once again we can observe that the last two columns represent average values, that differ from the beginning of the table once the urban rows show smaller numbers compared to suburban and rural rows. 



![Type Summary](https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Summary_per_type.png)



As a general rule, it is known that a high volume of products leads to low prices, and this can be ilustrated in this section of the analysis. 

<img src="https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Fig2.png" width="60%" height="60%">
<img src="https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Fig4.png" width="60%" height="60%">
<img src="https://github.com/GabrielaTuma/PyBer_Analysis/blob/4e7b55a49411a2ad1ff931db8105dcdb04b3453e/analysis/Fig3.png" width="60%" height="60%">



The number of rides and drivers are greater in urban areas, but the opposite happens when it comes to fare per ride. The values for fare per ride and fare per driver are averages inversely proportional to the percentages of rides, drivers and total fare amount per city type. A summary of all that can be visualized in this scatter plot:




![Scatter Plot per type](https://github.com/GabrielaTuma/PyBer_Analysis/blob/b02d4ad40b2dadfdf4b9353f5009142eb3c9505f/analysis/Scatter%20Plot%20Ride-sharing.png)



Our last chart is a representation of the total fare amount over the time, more specifically from January to early May of 2019. Each line is a different city type and once again we can observe higher values for urban areas. However, trends can come from the date data and we shouldn't leave this section without proper visualization.  



![Total Fare by City Type - line plots](https://github.com/GabrielaTuma/PyBer_Analysis/blob/b02d4ad40b2dadfdf4b9353f5009142eb3c9505f/analysis/FigChallenge.png)




### Recommendations 

- [ ] There's a high volume of drivers in urban areas. An investment to generate more demand could really improve the company's profit if we manage to bring more custumers while maintaining the cost invested in the current drivers. 
- [ ] Urban areas keep growing every year and are the biggest contributor of the company, more attention should be given to those areas. 
- [ ] In the graph showing fare over time, a pike can be observed close to the beginning of March. An investigation needs to be done in order to evaluate this event that happened simultaneously among all city types. Was the company responsible for the success? Was the event related to the specific day of the year? Can it be replicated?   
- [ ] More relevant data should be collected to make better decisions, maybe the weather has a big influence in the daily profit but it's not being evaluated, for example.  

 
