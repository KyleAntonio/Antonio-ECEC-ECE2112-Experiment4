# Antonio-ECEC-ECE2112-Experiment4
##### General summaries of each problem. see main code for a more detailed breakdown
## 1.) Create the following data frames based on the format provided
### a.) Instru
##### The first problem involves displaying a filtered output of the given dataframe. For this, I used .loc produce the rows and columns that fit the conditions in it's parameters. Using the logical operator AND (&), we can put multiple conditions for the values that it needs to look for.
### b.) Mindy
##### This problem is similar to the previous problem, however, an additional data column which wasn't included in the given dataframe is needed. The approach is to then, first, filter the dataframe with the given conditions then take all their grades and assign it to "Mindy". This is done in order to prevent tampering with the original given dataframe. From this table, we can use .mean(axis=1) to get the row mean for every student then declare a new column for mindy called average for the values to be assigned to. .iloc was used in order to exclude the name column from the mean equation. After this, .loc was used in order to filter the students who had greater than or equal to an average of 55 as well as displaying only their names, electronics grade, and average.

## Problem 2
##### The approach to this problem is to convert the provided data to visual graphs. First, the row average is computed using .mean(axis=1) then it is assigned to the column "Average". From the new dataframe, we can simply choose to make a boxplot using matplotlib. In this instance, we choose average and track to see the which track performed better. From the graph, people who chose microelectronics had a slightly better median average score than the other tracks, indicating a slightly better performance on average. However, people who chose communication track tended to have a higher average. In terms of gender, men had a higher median, indicating that they performed a bit better in terms of average score. However, the females can be seen to have a more scattered average than the males. In terms of hometown, people living in luzon tended to have a better median thus indicating a better performance on average. However, they also have a more scattered data than people living in Mindanao and visayas.
