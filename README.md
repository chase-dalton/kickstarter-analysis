# An Analysis of Kickstarter Campaigns

## Overview of Project

### Purpose
The purpose of this project is to analyze the various theater-related fundraising campaigns based on their respective launch dates and funding goals. By comparing these dimensions of these campaigns, we can observe trends and insights that may help explain as to why certain theater productions succeeded where others failed.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The first analysis was to analyze the outcome of various theater campaigns over time. The Kickstarter data was brought into a pivot table, with the data filtered to show the count of theater campaigns by month and campaign outcome. 
![pivot](https://github.com/typicalchazz/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_Pivot.png)

From this pivot table, a line chart was generated to show the changes in volume of outcomes over time. 
![launch_chart](https://github.com/typicalchazz/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The second analysis was to analyze the outcome of play campaigns based on their goal amounts. For this analysis, COUNTIFS() logic was applied to determine the number of successful, failed, and canceled play campaigns within various goal buckets. Simple arithmetic was also applied to determine for the total amount of play campaigns per goal bucket, what percentage of them were successful, failed, or canceled.
![table](https://github.com/typicalchazz/kickstarter-analysis/blob/main/Resources/Outcomes_Table.png)

From this table, a line chart was generated to visualize the percentage of successful, failed, and canceled play campaigns per goal bucket.
![goals_chart](https://github.com/typicalchazz/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
