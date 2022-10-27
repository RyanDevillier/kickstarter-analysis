# Kickstarting with Excel

## Overview of Project / Purpose

  The purpose of this project is to give Louise insight into how well Kickstarter campaigns, especially Kickstarter campaigns involving theatrical productions, performed based on several different criteria. Specifically, the criteria that we chose to focus on were the outcomes of Kickstarter campaigns for theatrical productions based on the time of the year that the campaign was held, and the initial goal amount of money that a given campaign host desired.  The raw Kickstarter data is broken up into several main categories and subcategories, and we filtered through these categories to produce meaningful observations for Louise.  Upon analyzing the relevant data, we end our analysis by giving Louise suggestions for the best possible month to start her campaign in, as well as what goal amount she should strive to reach with her campaign.

## Analysis
  We began our analysis of the Kickstarter campaign data by determining how many Kickstarter campaigns in the US were successful, canceled, or failures.  This was done by using a pivot table that filtered our raw data by country and by the campaigns’ outcomes.  Given that Louise’s goal is to produce a play, we filtered our pivot table again so as to only show theater campaigns, and then we visualized this pivot table using a bar chart. 
  
  ![2022-10-26 (8)](https://user-images.githubusercontent.com/115128743/198161489-8a6f7e40-1d0d-487b-8f23-1f1396123b5d.png)

  
  
  After gathering data about the success rate of theater campaigns in the US, we created another pivot table.  This time, our pivot table filtered the raw data to display the successful, canceled, and failed campaigns based on their subcategories, one of which included plays.  
  
![2022-10-26 (9)](https://user-images.githubusercontent.com/115128743/198161549-e65e8fed-183c-4a79-806c-be4dc3b77689.png)



### Analysis of Outcomes Based on Launch Date
   Now that we have made observations about the success rate of theatrical productions as a whole and about plays in particular, we turn our attention to more specific attributes of the Kickstarter campaigns that could potentially be significant relative to Louise’s success or failure.  One of the specifics we considered is the launch date of the Kickstarter campaigns.  So, with this in mind, we created a pivot table that filtered our raw data both by month and by the outcome of the campaigns.  To easily visualize the results, we created a line graph that displayed the data generated in our pivot table.
   
![2022-10-26 (6)](https://user-images.githubusercontent.com/115128743/198161710-f3a96406-b29d-4a25-b24b-6da2f66cd8fa.png)


### Analysis of Outcomes Based on Goals
  Building on the data we generated about the launch date of the Kickstarter campaigns, we dove one step deeper to determine how many plays were successful based on their initial goal amounts.  This was done in eleven $5,000 increments, with the initial increment beginning at all plays whose goal amount was less than $1,000.  Unlike the previous portions of our analysis, this was not done with a pivot table.  We instead created a table using Excel formulas (specifically formulas that involved the COUNTIFS function) that filtered through the raw data to yield only the data points that were plays with a goal amount between $0 and $50,000.  After getting these data points, we determined how many of these plays were successful, canceled, or failed per goal increment.  Finally, using this data we created a line graph that shows how many plays were successful, canceled, or failed based on the goal increment. 
  
  ![2022-10-26 (7)](https://user-images.githubusercontent.com/115128743/198161780-e8809bca-555a-4166-90da-007e897014bb.png)



### Challenges and Difficulties Encountered
   There were not many difficulties in doing this Kickstarter campaign analysis.  The most difficult section of the analysis was generating the percentages of successful, failed, and canceled plays using the COUNTIFS function, but after realizing what basis the data needed to be filtered upon (the outcomes, the goal ranges, and whether or not the campaign was a play), the COUNTIFS function was not difficult to implement across the columns of data that required it.  Another possible difficulty that could have emerged is making conclusions with the “Outcomes Based on Goal” line graph.  It is evident that the percentage of successful plays spikes upwards between $30,000 and $45,000, though this does not follow the general trend that as the goal amount increases, the higher the likelihood that the play is not successful.  This sharp spike can be explained by observing that there were only nine successful plays between $30,000 and $45,000, which suggests that these campaigns should be considered as outliers to the overall trend that higher goal amounts are less likely to yield successful campaigns.
   
## Results
  Using the bar chart we produced that displayed data about the success rate of theater campaigns, we can conclude that in general, Kickstarter campaigns for theater productions were successful, with 525 successful campaigns of 912 total – good news for Louise.  More specifically, we can gather from the pivot table and bar chart we made using the subcategory data that almost a quarter of the theater production campaigns are plays (1066 of 4114 campaigns), and that most of these plays were successful in reaching their initial goal amount (694 of 1066). 						                                                                               
  
  The most important conclusions relative to Louise’s play come from the “Outcomes Based on Launch Date” and the “Outcomes Based on Goals” graphs and their corresponding tables.  From the “Outcomes Based on Launch Date” pivot table and line graph, we can see that there was an obvious spike of successful Kickstarter campaigns for plays in the month of May, as well as a relatively high number of successful play campaigns throughout the summer months.  Judging from the heights of the lines in our line graph, it is also apparent that not only are the most successful play campaigns in the summer months, but also that most play campaigns actually occur in the summer months.  We can thus conclude that Louise should consider starting her campaign at the beginning of the summer, both because the most successful campaigns occur in May and because the interest for theatrical productions like plays is highest around the beginning of summertime.							            
  
  From the “Outcomes Based on Goals” pivot table and line graph, we can see that there is a general trend towards failure as the goal amount for a given Kickstarter campaign increases.  However, as mentioned above, there appear to be several outliers that skew this data between the range of $30,000 and $45,000.  Thus, it would be advisable for Louise to choose a lower crowdfunding goal (which again is good news, since her initial budget was approximately $10,000).  In addition to the line graph we created for this section of our analysis, a box and whisker plot could have been helpful in visualizing the outliers that were evident in our data. 					
  
  There are several limitations that are to be noted with regards to our initial raw data set.  First, while we were given a dataset with several thousand rows of entries, it should not go unnoticed that we had to filter out the majority of these datapoints to do analysis on just theatrical productions, and, more specifically, just datapoints that were plays.  Also, given that we were doing analysis on only Kickstarter campaigns, we may not be showing the full story on how plays do generally, since we have only focused on one source of crowdfunding.  Finally, with regards to the “Outcomes Based on Launch Date” section of our analysis, we concluded that May was the best month to start a Kickstarter campaign for a play because the highest number of successful Kickstarter campaigns for plays was in May.  However, the highest number of total plays also occurred in May, and this inflates the graph to suggest that May is the best month by a significant margin.  If we were to calculate the percentage of successful play campaigns relative to the total play campaigns for each month, we would see that May has an overall success rate of approximately 66.8%, while June and July have success rates of 65.4% and 63.0%, respectively.  These differences suggest that June and July are also good months to start a play campaign in, and, given the potential aforementioned limitations of our raw dataset, June and July could possibly be as good as May or better if we were to have a more comprehensive collection of Kickstarter play campaigns.
