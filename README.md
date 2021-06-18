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
One needed to be careful when analyzing the data, for there is much room for error. A challenge of note would be to be wary of the COUNTIFS() logic. If you were to just copy the data for each cell in a column, your data would be inaccurate, for you needed to make sure each cell was counting for a different set of conditions unique to that cell. You need to make sure that for each goal bucket, your COUNTIFS() was making sure to count for the range specified for that goal bucket, as well for the outcome status indicated in the column.

Another challenge comes just from the nature of Excel reporting. The logic and charts for both Theater Outcomes by Launch Date and Outcomes Based on Goals were on separate pages separate from the Kickstarter data itself. One needs to be sure that when using logic that refers to off-page data that column/row/cell values are accurately representing what it's defined as on these new pages. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - That historically there are more successfully-funded theater kickstarters in May than any other month, and that there are less successfully-funded theater kickstarters in December than any other month.

- What can you conclude about the Outcomes based on Goals?
  - That the higher your goal amount, the more likely your play kickstarter will not be fully funded.

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

