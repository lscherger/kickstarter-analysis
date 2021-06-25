# kickstarter-analysis
Analysis of kickstarter data and visualization of campaign outcomes 

### Kickstarting with Excel
## Overview of Project

### Background

 Louise is launching a kickstarter campaign, "Fever," and would like to visualize trends in past theater kickstarter campaigns to determine what funding goals and launch dates tend to produce successful outcomes. 

### Purpose

 The purpose of this project is to analyze kickstarter data, then provide visual tools to give Louise insight on outcomes based on launch date and goals. In this project, I used conditional formatting, formulas, pivot charts and filters in Excel to analyze and visualize the data.

## Analysis and Challenges


### Analysis of Outcomes Based on Launch Date

To analyze kickstarter outcomes based on launch dates, I created a “Years” column in the spreadsheet by using the YEAR() function to extract the year from the Date Created Conversion column. By creating a "Years" column, I was able to analyze and visualize the data over the course of a year to understand what launch month/season tends to produce successful outcomes. 
  

<img width="335" alt="Screen Shot 2021-06-25 at 11 15 16 AM" src="https://user-images.githubusercontent.com/85946042/123468480-709cfc80-d5b7-11eb-9b1d-929674a9ca4f.png">


Next, I created a pivot table to analyze trends in outcome frequencies by launch date, while also filtering by category and years. I filtered by parent category, then filtered further to include only theater campaigns, so that the data would be relevant to visualize for Louise. The pivot chart rows showed months based on the date created conversion data from the kickstarter sheet. Because the date conversion cells contained quarters, years and date created, I only kept the date created so that I could visualize trends with launch dates more specifically by the month. The columns represented the different campaign outcomes: "successful," "failed," and "canceled." The outcome categories were arranged in descending order, so that the highest frequency outcome (successful outcome) appeared first in the chart from left to right. The data points in the chart were summations of outcome frequencies by month. The result shows how outcome frequencies differ between months. 

<img width="332" alt="Screen Shot 2021-06-25 at 11 18 26 AM" src="https://user-images.githubusercontent.com/85946042/123468776-de492880-d5b7-11eb-96ab-e7b11b560524.png">          <img width="327" alt="Screen Shot 2021-06-25 at 11 21 28 AM" src="https://user-images.githubusercontent.com/85946042/123469119-439d1980-d5b8-11eb-9f63-06970ed3ba49.png">

Because months are a unit of time, it was useful to visualize this data within a line graph. In this graph, launch date (by month) is the independent variable and campaign outcome frequency is the dependent variable. The line shows how frequency tends to change over a year as launch date changes. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/85946042/123469484-b73f2680-d5b8-11eb-9595-1d9b09d8d6f7.png)


### Analysis of Outcomes Based on Goals

The other deliverable Louise requested was an analysis of kickstarter outcomes by funding goals. I used COUNTIFS statements to collect frequencies of successful, failed and canceled outcomes for plays (from the parent category of “theater”) based on their funding goal. 

<img width="962" alt="Screen Shot 2021-06-22 at 4 38 21 PM" src="https://user-images.githubusercontent.com/85946042/123467788-85c55b80-d5b6-11eb-9ec3-aed6d5b34ce0.png">


After the first 1000 increment, the funding goals increased per row by 5000 until reaching 50,000. The outcomes were totaled per funding bracket. Next, I compared what percentage of outcomes in each bracket succeeded, failed, or were canceled. These percentages were displayed in a line graph, with funding goal brackets as the independent variable and campaign outcome percentage as the dependent variable. The trend line shows how the outcome percentages change with increases in funding goals. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/85946042/123467923-b4dbcd00-d5b6-11eb-8e41-596713183866.png)


Since the funding goals were broken into brackets, I also think this graph could be displayed as a stacked bar graph to compare percentage rates for all brackets side by side. 

### Challenges and Difficulties Encountered

As a first time advanced Excel user, I encountered some challenges with keeping track of the filters applied in the master sheet. In the future, it would be helpful to create new sheets with those applied filters. I also had difficulty understanding how to filter multiple columns. I got through this by selecting the whole header row after trying first to select multiple columns and selecting the filter first. My most significant challenge was timing. There are many things that I typed in manually, which led to syntax errors. To help expedite the process, it is important to keep the sheet very organized and become more familiar with Excel formulas. I plan to practice creating pivot tables to experiment with filters.


## Results
Based on the analysis of outcomes based on launch date, I concluded that failed outcome numbers do not fluctuate significantly as the launch month changes, generally staying within 30-50 failed cases per month. While there are a few more canceled projects in January, the amount of canceled outcomes does not seem to fluctuate with changes in launch date. 

I also discovered that the first half of the year generally sees a positive change in amount of successful projects, with May launch dates yielding close to double the count of successful projects from January. May through July seems to be a good time to launch a project. After this window, successful outcome percentages begin to decrease for the rest of the year, reaching the lower percentages seen earlier, in April. 


Moving on to outcomes based on funding goals, the percentage of successful outcomes tends to decrease as funding goal increases. This makes sense; bigger goals may seem less likely to reach compared to smaller goals. Still, there is a jump in the $35,000-$45000 range that doesn't follow the negative trend of goal versus outcomes. It would be useful to break down that segment to see if there are confounding variables that make those campaigns more successful even though they require large funding goals.


The limitation of the data is its size. With more data, the outcomes should fall closer to the real distribution of all kickstarter campaigns. The other limitation is other possible confounding variables that we don't see in the dataset that could have also affected the ouctomes. Factors that could influence amount pledged and campaign outcome could be staff size, budget breakdown visibility, or project progress. There are other questions we could ask to filter the data further, such as: do any of these projects conduct multiple campaigns at different points in their timelines? 

In abother iteration, there are other edits that I might add. The current graphs do not have axes titles, which could be difficult for a client to interpret in the future. Also, I think it would be useful to specify the other filters that were used; for example, the outcomes based on goal chart does not specify that it is just in the US, or only for plays, so this would be an important distinction to make in the next iteration in order to make the data interpretation clearer. 

Finally, there are other possible tables and graphs that we could create to visualize the data for a more thorough report in the future. One new chart could show outcomes based on goals for all possible projects to see if this pattern is characteristic of all kickstarter campaigns, or just for plays. Additionally, since Louise is interested in future projects in Great Britain, we could compare campaign outcomes from the US and Great Britain directly. Finally, I would also like to see a chart comparing campaign duration versus coutcomes; does the length of the campaign affect how many backers the kickstarters recieve? While we answered the primary questions that Louise requested (launch date versus outcomes and goals versus outcomes) there are many more ways we could filter the data to discover different trends. 
