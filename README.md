# Overview of Project
Louise is a playwright who came to me for assistance in funding her play, Fever. In a short period of time, she was close to reaching her fundraising goal. She would like me to determine how her fundraising campaign compares to other theatre fundraising campaigns. Specifically, she is interested in how successful or unsuccessful a campaign was based on their funding goals and the date the campaign was launched. 

To perform this analysis for Louise, I used data obtained from Kickstarter campaigns around the world.
 
# Analysis and Challenges 
## Outcomes Based on Launch Date
In order to provide results that are most relevant to Louise I filtered for theatre campaigns only. I created a pivot table that compared the month the campaign was launched to the outcome of the campaign. Using the pivot table, I created a line chart to visually demonstrate the relationship between outcome of campaign and the launch month. 

! [Theatre_Outcomes_vs_Launch](https://github.com/mdhugge/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

I was able to perform this analysis without any difficulties. A possible challenge that could have arose is determining where each dataset should placed in the pivot table. Although, it is clear that I want to perform an analysis on the outcome of a campaign based on when it was launched, I had to determine for myself where each set of data would be placed in the pivot table. 

## Outcome Based on Goal
To perform an analysis of the outcome of a campaign based on the goal, I had to first gather and organize my date. I grouped campaigns by ranges of goal amounts. I than used the `COUNTIFS` function to determine how many successful campaigns there were based on each goal range. I repeated this with failed and canceled campaigns as well. In order to provide information that is most relevant to Louise, when preforming the `COUNTIFS` function I filtered for plays only. I used the `SUM` function to determine the total number of campaigns for each goal range. I determined a percentage of successful campaigns by dividing the number of successful campaigns in a goal range by the total number of campaigns for that goal range. I repeated this with failed and canceled. Using the goal ranges and the percentage of successful, failed and canceled campaigns I created a line chart. 

! [Outcomes_vs_Goals](path/to/Outcomes_vs_Goals.png)

Using the `COUNTIFS` function was challenging because there were a lot of criteria to filter for and it required going between two spreadsheets. Another element that added to the confusion was understanding the language used in excel functions. I broke down each component to help me grasp the concept of the `COUNTIFS` function. To understand the symbols used in the function I performed a google search. I than thought about exactly what I am trying to find to help me determine which criteria I need to filter for (e.g. when I am looking for number of successful play campaigns that have a goal of less than 1000 I need to filter for the subcategory plays, successful outcomes and goals that are less than 1000). 

# Results
Based on the Theatre Outcomes by Launch Date analysis it is clear that the number of successful theatre campaigns is greatest in the month of May. It also evident that theatre campaigns that are launched in the month of December are less likely to be successful.

From the Outcomes Based on Goals Analysis it is apparent that number of successful play campaigns is greater when the goal is lower and having a goal less than $5000 is ideal. 

A limitation of this dataset is that …

Other tables and graphs…
