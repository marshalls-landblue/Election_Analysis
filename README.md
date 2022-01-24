# Election Anaysis Tool

## Overview of Project

### Purpose

This analysis was designed to perform an audit on the vote count by district/county and for each of the top 3 candidates. Running these totals and numbers was important to create an accurate picture of how close the race was, and how the distribution of votes fell geographically to validate the final tally.

## Results

The first step of this project was to read in the csv file provided with the election data, then iterate through the rows of the document to extract the raw information:

![image](https://user-images.githubusercontent.com/17416097/150716989-2f5866a4-bf0a-4024-83db-1f9ff4945ca7.png)

We were able to compare the data from each county to the totals using a simple for loop:

![image](https://user-images.githubusercontent.com/17416097/150716845-4ab61aa1-11b7-4268-b1df-434ec37b28d5.png)

Then we used conditionals to gather which county was the winner.

![image](https://user-images.githubusercontent.com/17416097/150716770-533d38c6-8811-42b6-8f2a-69576a72bf45.png)

Then we did the same for the candidates, indivdual

From this, we were able to gather the following statistics:

* 369711 Votes were cast in total in this election. This includes votes from 3 Counties.
  * Jefferson County had 10.51% of total votes (38,855 votes).
  * Denver County had of total votes (306,055 votes).
  * Arapahoe County had 6.71% of total votes (24,801 votes.
* Denver County had the most pronounced turnout with 306,055 votes.
* The candidate vote tally is as follows:
  * Charles Casper Stockham with 23.0% of total votes (85,213)
  * Diana DeGette with 73.8% of total votes (272,892)
  * Raymon Anthony Doane with 3.1% of total votes (11,606)
* This makes Diana DeGette the clear winner with 272,892 votes (73.8%)

See the text file in the analysis directory for confirmation:
![image](https://user-images.githubusercontent.com/17416097/150717090-378cf2fc-6bf0-45db-b174-35165d28bf97.png)

## Summary

Using a script to programatically run through this election data increased the efficiency of the operation drastically. This made for a piece of software that is easily extendable for multiple purposes. For example we could add functionality to be able to read in more columns from data of elections wit more verbose geographical information, like city, postal code, etc. We could also compare the distribution of votes for particular candidates by county or district to see how the voter support is for each runner by area. These are just a few ways we could repurpose the code, but for this purpose at least, it is complete as-is.
