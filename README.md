# Kickstarting with Excel

## Overview of Project
An analysis was performed using Kickstarter data to find trends amongst successful campaigns and to determine how to run a successful Kickstarter campaign to raise money for a play. 

Kickstarter Excel Analysis File: [Kickstarter_Challenge.xlsx](https://github.com/borkard/kickstarter-analysis/files/Kickstarter_Challenge.xlsx)

### Purpose
The goal of this challenge was to discover common factors of successful Kickstarter campaigns and to see how different launch dates and fundraising goals affected the campaigns' outcomes. These insights are used to navigate how to launch a successful Kickstarter to fundraise for a play.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Analysis of the Outcomes Based on Launch Date was conducted by creating a pivot table to count the number of theater campaigns per outcome (successful, failed, canceled) by the month in which they were launched. The pivot table was created by selecting the data and creating a pivot table filtered by the parent category (theater) and year, with the rows as the date created and the columns as the outcomes. The outcomes are also filtered to only show successful, failed, and canceled campaigns. A visualization of the analysis is below.

![Theater_Outcomes_vs_Launch](https://github.com/borkard/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png?raw=true)

### Analysis of Outcomes Based on Goals
An analysis of the Outcomes Based on Goals was conducted by grouping the goals into ranges and counting the number of campaigns within those goal ranges by outcome and further calculating the percentage of projects that fell into each outcome and goal range.A spreasheet was created with a table with the goal intervals in the first column and headings for the number and percent by outcome on top. The goals were grouped into 12 intervals, in mostly intervals of $5,000. A COUNTIFS formula was applied in each of the other cells within the table to count the number of campaigns based on the appropriately titled outcome, goal interval, and for the category "plays". The SUM function was used to calculate the total number of projects per goal interval. The number of projects per goal interval and outcome was then divided by the total for that goal interval to determine the percentage of projects that were successful, failed, or were canceled per goal interval. A visualization of the analysis is below.

![Outcomes_vs_Goals](https://github.com/borkard/kickstarter-analysis/blob/main/Outcomes_vs_Goal.png?raw=true)

### Challenges and Difficulties Encountered
A challenge I encountered when analyzing the Kickstarter data was performing the COUNTIFS function to find the number of campaigns by outcome for each goal. It took some time to figure out which fields to include or change within the formula for the different outcomes and goals. I had initially left "plays" out of my calculation which produced incorrect results overall. I corrected my errors by checking the formulas for each section to make sure the relevant fields were included, including plays. Once the table was correctly configured, it also took some time to learn how to make the chart with the right legend and axes. I was able to edit the chart to have the right fields and data selected by right-clicking on the chart and selecting the necessary data and formatting the chart accordingly.

## Results
From the Outcomes based on Launch Date, it can be concluded that May is an ideal month in which to launch a theater campaign as the highest number of successful campaigns are launched in May; over double  the number of failed campaigns. December is not an ideal month in which to launch a theater campaign because the number of successful and failed campaigns begin to even out. In the realm of Kickstarter campaigns, theater is a good category in which to launch a campaign because there are a high number of successful campaigns year-round and very few that are cancelled.

The Outcomes based on Goals shows that all campaigns fail if the goal is between $45,000-$50,000. Additionally, very few campaigns succeed when the goal is set over $50,000. Most Kickstarter campaigns with a goal of under $1,000 are successful and it is likely that a campaign will succeed with a goal of under $15,000. If Kickstarter campaign for a play were to be launched with a goal of $10,000, there is a 54% chance that it will succeed.

Some information the Kickstarter dataset did not have that may have been helpful would be who the donors for the campaigns are, especially those within the same category. Additionally, to fully understand the funding and success of a project, it would also be useful to know if there were any additional funding sources beyond Kickstarter and how much money was raised through other methods.

Other possible tables and graphs that could be created include analyzing the outcomes of plays by country, as well as comparing the amount pledged to the initial campaign goal for the plays subcategory to get a more nuanced view of how much money could be raised and what to set as the goal.
