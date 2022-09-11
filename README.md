# Kickstarting with Excel

## Overview of Project

### The purpose of this project was to implement fundamentals discussed in this week's modules, and apply them to a real world example. We used functions such as countifs and sum, in order to create relevant charts and graphs. We also used the pivot table ability to create tables in which we were able to organize our data to any parameter we wanted, allowing for a more refined configuration to match needs. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date: Creating the graph for Theater Outcomes vs Launch was relatively simple, as we just needed to carry over information from the parent Kickstarter sheet without any modifications. The only area I experienced minor confusion was when I was creating the pivot table, and I had years as my row labels, as opposed to the months which we wanted. It was a relatively easy fix, as all I had to do was fiddle with the filter until I got months as my x axis label. 

(/Users/ryan/Downloads/Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals: This was a slightly more challenging task for me, as I actually spent a while trying to figure out my countifs function as I originally had my code set to '=COUNTIFS(Kickstarter!$D:$D, "<1000", Kickstarter!$F:$F, "failed")' but the data was not matching up to the provided graph of failed projects. After a lot of thinking and trying things out, I realized I needed to filter by theater/plays specifically, as this was a parameter we were asked to include, so I changed my code to '=COUNTIFS(Kickstarter!$D:$D, "<1000", Kickstarter!$F:$F, "failed", Kickstarter!N:N, "theater/plays")', which then solved my issue, and I wa able to make a line graph that matched the one provided. I greatly enjoyed this task, however, as I had to think and problem-solve my way through the struggle, which allowed my to apply several different techniques we have learned so far in order to troubleshoot.
(/Users/ryan/Downloads/Outcomes_Based_on_Goals.png)

## Results

### Two conclusions I am able to draw about the Outcomes Based on Launch Date are that the most plays are launched in May, and it seems to be that the later months of the year, like November and December, experience the lowest number of successful plays. As for the Outcomes Based on Goals, it seems to be that plays with an overly-ambitious goal, $45000 and higher, have a very low success rate, perhaps meaning a more moderate goal will lead to more realistic expectations and success. Some limitations on this dataset are limited sample size, as though there were several thousand samples, this is over the course of many years, and so the actual sample count per year is much lower, and perhaps less conclusive. Some other graphs we could have made could be a pie graph with success of every category, to see which types perform better overall, regardless of any other metric, and from there breakdown whichever the most successful subcategory into smaller metrics, to see if the reason for their higher success was a certain range of funding, certain time of the year, or etc.



