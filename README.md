# An Analysis of Kickstarter Campaigns

## Overview of Project

### Purpose
The purpose of this project is to analyze the various theater-related fundraising campaigns based on their respective launch dates and funding goals for Louise. By comparing these dimensions of these campaigns, we can observe trends and insights that may help explain as to why certain theater productions succeeded where others failed.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The first analysis was to analyze the outcome of various theater campaigns over time. The Kickstarter data was brought into a pivot table, with the data filtered to show the count of theater campaigns by month and campaign outcome.

![pivot](https://github.com/typicalchazz/Kickstarter-analysis/blob/main/Resources/Theater_Outcomes_Pivot.png)

From this pivot table, a line chart was generated to show the changes in volume of outcomes over time. 

![launch_chart](https://github.com/typicalchazz/Kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The second analysis was to analyze the outcome of play campaigns based on their goal amounts. For this analysis, COUNTIFS() logic was applied to determine the number of successful, failed, and canceled play campaigns within various goal buckets. Simple arithmetic was also applied to determine for the total amount of play campaigns per goal bucket, what percentage of them were successful, failed, or canceled.

![table](https://github.com/typicalchazz/Kickstarter-analysis/blob/main/Resources/Outcomes_Table.png)

From this table, a line chart was generated to visualize the percentage of successful, failed, and canceled play campaigns per goal bucket.

![goals_chart](https://github.com/typicalchazz/Kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
One needed to be careful when analyzing the data, for there is much room for error. A challenge of note would be to be wary of the COUNTIFS() logic. If you were to just copy the data for each cell in a column, your data would be inaccurate, for you needed to make sure each cell was counting for a different set of conditions unique to that cell. You need to make sure that for each goal bucket, your COUNTIFS() was making sure to count for the range specified for that goal bucket, as well for the outcome status indicated in the column.

Another challenge comes just from the nature of Excel reporting. The logic and charts for both Theater Outcomes by Launch Date and Outcomes Based on Goals were on separate pages separate from the Kickstarter data itself. One needs to be sure that when using logic that refers to off-page data that column/row/cell values are accurately representing what it's defined as on these new pages. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - That historically there are more successfully-funded theater Kickstarters in May, and that there are less successfully-funded theater Kickstarters in December.

- What can you conclude about the Outcomes based on Goals?
  - That the higher the goal amount is set for play Kickstarter campaigns, the more likely the campaign will not be fully funded.

- What are some limitations of this dataset?
  - The data is only so representative of the entirety of Kickstarter's data. While it is of a decent sample size where we can take comfort in our conclusions having some validity, it is only so representative of the entirety of data out there, meaning that our conclusion may only be true to the particular subset of data we analyzed as opposed to being truly valid of the entire population of data. 
  
  Another limitations is regarding Kickstarter campaigns that had significantly higher goal amounts set. While there were many rows of data related to campaigns with lower goal amounts, there is significantly less data with goals that are quite high. For example with the "Outcomes Based on Goals" sheet, one can see that there is only 1 campaign that had a goal between $45000 to $49999, while there were 534 campaigns in the $1000 to $4999 range. This disparity needs to be taken into account when analyzing the data.

- What are some other possible tables and/or graphs that we could create?
  - The main dimensions of the Kickstarter data that was analyzed for Louise were Outcomes based on their goal amount and launch date. There are other dimensions in the data that weren't the focus of this current analysis that could be informational. For example, a table comparing outcomes with regards to campaigns being staff picks or not to see if the staff pick had any influence of success rates in campaigns could be insightful. Or looking at not just launch dates, but how long campaigns ran for and see if that had any bearing on success rates. A line graph with the volume of outcomes mapped over a time series could also be very insightful.  

