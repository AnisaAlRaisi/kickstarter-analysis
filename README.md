# An Analysis of Kickstarter Campaigns
performing  analysis on Kickstarter data to uncover trends

## Overview of Project
The purpose of this analysis was to use highlight data on theater play kickstarters to show Louise how different campaigns fared in relation to their launch dates and their funding goals in comparison to her campaign.

## Analysis and Challenges
In this project, I conducted two different types of analysis, one to compare Theater Outcomes vs their Launch date and the other to compare Outcomes vs Goals.

###### creating an Outcomes Based on Launch Date Chart
To start, I extracted the year of the launch date from the Unix timestamp in the original data.
<img width="798" alt="Screen Shot 2021-09-05 at 12 45 48 AM" src="https://user-images.githubusercontent.com/31663190/132107615-9a2e2bbb-5b89-49d3-b4b2-808f1218f6e0.png">
Next, I created a pivot table that filtered the data by "Parent Category" and "Years" to isolate the data specific to the "theater" parent category. I then dragged "date created" into rows and "outcomes" into columns and values to highlight the illustrate the relationship between the two.
<img width="1021" alt="Screen Shot 2021-09-05 at 1 01 11 AM" src="https://user-images.githubusercontent.com/31663190/132107956-e082900c-60b6-4e68-82c1-72064f045872.png">
After filtering the parent category to just theater, I created a line chart to visualize this relationship.
My biggest hurdle during this process was figuring out how to group the dates into months. As I failed in doing so, I opted to group the days into 100's (of days.) This chart does not show the information that Louise is looking for.

###### Outcomes Based on Goals Chart
For this visualization, I created a new sheet to extract and group data on the kickstarters original goal and find out what percentage of them were successful in reaching it, and which percentage had failed or canceled.
To do this, I used the COUNTIFS function to extract the data from the original sheet and find out how many data points belong to which goal range.
<img width="1140" alt="Screen Shot 2021-09-05 at 1 15 28 AM" src="https://user-images.githubusercontent.com/31663190/132108253-3cdd917d-0318-4427-a6ff-2ace0602e719.png">
Next, I created a line graph to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.
<img width="524" alt="Screen Shot 2021-09-05 at 1 20 20 AM" src="https://user-images.githubusercontent.com/31663190/132108333-0277257a-559a-4021-be35-50837c320b83.png">

## Results
Based on the results of the "Theater Outcomes Based on Launch Date" graph, the most successful theater kickstarters launched in May. This could be an indicator that the time of the year does affect the success of theater kickstarters, possibly as may is the start of the summer which is a time that often experiences an influx of tourists. 
Compared to the level of success over the year to the level of failure, the level of failure is pretty consistent. 
The Outcomes vs Goals chart shows that projects in the 20000 to 24999 range and 45000 to 49999 range have a higher percentage of success.
