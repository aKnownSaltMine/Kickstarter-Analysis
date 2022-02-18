# Kickstarting with Excel

## Overview of Project
This project takes a look at Kickstarter Campaign success, failure, and cancel rates both based on the time of year for the launch of the campaign, as well as the overall funding goal of the campaign. We used data pulled from Kickstarter funding data of a wide source of campaigns in order to compare multitude of campaigns to theater based projects and more specifically plays.
### Purpose
The overall purpose of this examination was to outline any trends in campaign success rates based on time of year launched and the ranges of funding goals with larger success rates so as to better understand the best time of year to launch a campaign and the goal to set to increase chances of meeting funding goals. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Taking a look at 1369 total Theater based Kickstarter campaigns, a few things become clear. First and foremost, more campaigns that were looked at were successful than they failed or were canceled, and throughout most of the year the sheer number of campaigns does stay fairly consistent. While some of these successful campaigns are getting funded throughout other parts of the year, the months entering the summer, namely May and June, have seen the highest volume of successful campaigns more than any other part of the year. The times of years with the next most successful times for funding land in both February and October. One thing to note about these two months, however, is that the failures also increase along with the successes in contrast to a fairly consistent failure rates with the higher successes of the summers. This is largely due to the increase in volume of campaigns in these months, rather than actually being months that demonstrate successful campaigns.

 ![Outcomes Based on Launch Date](https://github.com/aKnownSaltMine/Kickstarter-Analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The data of overall funding goals for the 1047 plays in the dataset and looking at their success rates demonstrated a few things. First, the funding sees the most amount of success with goals that are below $5000 with an overall success rate at this funding goal of 73.47%. More specifically plays in the 1000 to 4999 range acheiving a success rate of 72.66%, and below 1000 at over 75%. As the goal scales up, there is a negative correlation with the success of the funding campaign, with the 5000-9999 range acheiving a 55% success rate, similar to the 10000-14999 range with a 54% success rate. As we reach the higher funding goals, the actual amount of campaigns is significantly smaller, making the actual success rates a lot more questionable to their use in predicting outcomes.

![Outcomes Based on Goals](https://github.com/aKnownSaltMine/Kickstarter-Analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
I did have difficulties in getting the chart "Outcomes Based on Goal" to match what was expected in the directions. When I kept doing the formula, it would have instances of cancelled which was making the entire graph off. When I was back tracking and checking my formulas however, I did realize that I did not add 'Kickstarter!$R:$R, "=plays' into my COUNTIF forumla, so rather than just pulling the data from just the play subcategory, it was pulling from the entire dataset. A small overlook that when fixed matched what was expected. This demonstrates that it is needed to look over the formulas placed before accepting the final visualization.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	- The best time to launch a campaign would be in May to increase  probability of reaching a successful funding campaign.
	- Failed campaigns stay largely consistent throughout the year. 
	- December would be the worst time of year to launch a funding campaign.

- What can you conclude about the Outcomes based on Goals?
	- For the largest chance of reaching goal, the funding goal should be set below $5,000.
	- A campaign of $10,000 is possible, but the success rate goes from 72% to 55%.
	- 85% of campaigns examined have a funding goal of less than $10,000 so it the larger goals have such a small sample size that their success/failure rates will be less accruate in use of prediciton. 

- What are some limitations of this dataset?
	- There are not a significant population of funding campaigns for plays to pull from for reliable prediction if the goal moves above $10,000. 
	- While the dataset does give the country of origin, it would be very useful to know the city of origin as well as a way to see if location of origin has a factor in achieving funding goals. 
	- This data is only coming from kickstarter data. It does not include data from other crowdfunding sites such as GoFundMe, Indiegogo, Patreon, etc. Including data from these sites, would not only provide a larger sample size, but also could show whether or not plays are better funded through different sites that the campaign is placed on.
	

- What are some other possible tables and/or graphs that we could create?
	- Rather than looking at just the count of successes, failures, and cancels over the course of a year of the Theater Parent Category, we also could look at the rate of success in comparison to the total amount of campaigns launched in that month so as to account for situations where a month just has fewer or more campaigns launched than other months which can effect the graph as laid out currently.
	- After finding out that so many of the successful campaigns were towards the lower end of the goals, it would have been interesting to do a further breakdown of the goals to show the success rates of funding on possibly $500 increments within the $0-$10,000 range. This would have allowed us to give a more specific recommendation for funding goals. 
	- We could have done a graph showing the average donation to a campaign throughout the course of a year as another way to examine when a funding campaign might be the most efficient in needing fewer backers to achieve a successful funding. 
	- There could be a chart that is similar to the successful funding through the course of a year, but we could do it on a year basis so see if certain years might be skewing the data being used. 
	- A table showing the average donation based on category and the average amount of backers per category of successful campaigns to see if plays and theater productions typically need more or less backers than the other types of campaigns or if they need to target getting a higher donation amount out of the backer. 
	- A table and a chart demonstrating the length that a Kickstarter campaign ran when comparing successes, failures, and cancelations. 
	- A chart showing the Success rates and Failure rates of plays when they were a part of the spotlight or not. And a similar chart and table for staff pick rather than spotlight. 
