---
title: "Data Visualization"
excerpt: "Repository of my participation in R for Data Science's Tidy Tuesday community of practice. Each week, a new dataset is released for people to practice their data visualization skills and receive help and feedback from the R community. I primarily work with {ggplot2} for graphics.<br><br><img src='/images/datViz.gif'>"
collection: portfolio
---

## Background
In June 2020, I began participating in a weekly data visualization challenge aimed at improving data wrangling and presentation skills. A subset of my work is presented here, but for further viewing see the below repositories for all of my visualizations with their respective R code. Each week, I aimed to try implementing a new type of chart, feature, or color palette to expand my coding skillset. Some of them took hours and some less than an hour depdening on the initial dataset and my goals for that week. 

[Github Repository](https://github.com/tessaeagle/TidyTuesday) of R4DS TidyTuesday attempts starting June 2020

[Github Repository](https://github.com/tessaeagle/30daychartchallenge) of my participation in the [30 Day Chart challenge](https://twitter.com/30daychartchall?lang=en)

**Project Year:** Ongoing

## Selected Visualizations
This plot utilized video game [data](https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-03-16/readme.md) from Steam. I looked across an eight year period (2012-2020) to explore the games with the highest number of players online at the same time. My design for this plot was insired by Atari's Breakout game.<br>
<img src='/images/game.png'><br>


The next visualization used [data](https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-03-02/readme.md) from FiveThirtyEight looking at the content of commercials aired during the Superbowl. I wanted to try implementing a stream graph which is a type of stacked area chart, which is somewhat reminiscent of the shape of a football.<br>
<img src='/images/super.png'><br>


R has a built in package for [data](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-09-08/readme.md) from the show Friends. It contains speaker and dialogue data broken down by season and episode. I tested out using a waffle chart to display the ratio of time each main character spent talking in each of the ten seasons.<br>
<img src='/images/friends.png'><br>


This was my first ever attempt at making a map in ggplot and it was a frustrating and time-intensive plot. I used [data](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-08-18/readme.md) on extinct plants and those at risk of extinction to visually explore where plants are under threat globally. I combined the map with a simple dot plot where I filtered for the top threats to endangered plants. <br>
<img src='/images/map.png'><br>


For this chart, I attempted a waterfall bar plot, where I mapped two variables against each other. The [data](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-11-10/readme.md) looked at phone use over time broken down by mobile and landline subscriptions. As you can see, mobile use is increasing over time compared to a decline in landlines. <br>
<img src='/images/phone.png'><br>

The following visualization was made as part of the 30 Day Chart Challenge. The prompt for this day was "experimental". I had been wanting to test out different implemntations of coord_polar to explore circular visualizations of line plots. <br>
<img src='/images/circles.png'><br>

Using [data](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-08-04/readme.md) on European country's sources of power. I created a stacked bar plot that shows the distribution of power sources broken down by country. I faceted the plot to show the breakdown by year from 2016-2018. The goal of this was to show the changes in utilization of power sources over time. <br>
<img src='/images/europeEnergy.png'>



