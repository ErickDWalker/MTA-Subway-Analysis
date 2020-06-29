# Real Estate Development Proposal

**Overview**
---
For Project 1 in the Metis bootcamp, groups were asked to utilize MTA Subway traffic data to explore a hypothetical business use case. This project is based on the idea of approaching luxury building developers with the proposal of using data-driven analytics to aid in the decision of where to build their next development. 

By analyzing MTA station traffic patterns and key neighborhood characteristics (income, demographics, the presence of other luxury buildings in the area), the aim is to provide actionable insights that can assist in identifying potentially favorable building sites. 


**Data**
---
Turnstile data was pulled from the [MTA site](http://web.mta.info/developers/turnstile.html). Since we were more interested in recent traffic patterns, as opposed to broad trends over extensive periods of time, we selected data from the September - November 2019, three-month period. We left out December to exclude any noise that might arise from holiday traffic patterns.

**Methodology**
---
We first set out to identify the station with the most turnstile exits in the morning (defined as 7-11am) during the weekdays. By doing this, we could get a sense for the station that is heavily utilized by commuters looking to get to work in the morning. Next we explored the subway lines that pass through that "top commuter" station, with the goal of finding stations along those lines that satisfy two criteria (listed in order of importance):
1. They are located within neighborhoods with relatively high median incomes, and 
2. They have relatively low number of entrances during work day mornings (again defined as 7-11am)


**Results**
---
Since we were more concerned with finding an area with incomes capable of sustaining a luxury development than we were with finding low foot traffic, we first identified neighborhoods with relatively high median income levels. The heat map below shows relative income levels (as well as foot traffic) among neighborhoods served by the 4 and 5 subway lines. Median income levels were taken from the [following link](https://ny.curbed.com/2017/8/4/16099252/new-york-neighborhood-affordability), and then scaled to be between zero and one.

<img src="https://github.com/ErickDWalker/MTA-Subway-Analysis/blob/master/img/Income_Entries_Neighborhood_Heatmap.png" width="900" height="500">

Downtown Brooklyn emerged as the neighborhood with the highest relative median income. Though it also appeared to have the highest entries, this number represents an aggreagation of multiple stations, and so can be misleading. To get around the aggregation issue, we then looked at the weekday morning turnstile entrances for individual stations. 

![alt text](https://github.com/ErickDWalker/MTA-Subway-Analysis/blob/master/img/Income_Entries_Station_Heatmap.png?raw=true)

Among the downtown Brooklyn stations, we found that the Nevins street station best satisfied both of our conditions, and ultimately was the location we chose as our recommendation to our hypothetical "client." 
