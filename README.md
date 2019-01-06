# Investigation of time related features in Bikesharing system dataset


## Dataset

The data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. This dataset can be downloaded followin this [link](https://drive.google.com/file/d/1gsg4DPGEyyjharedDMKTb6WOhEmOrsfs/view?usp=sharing).


## Summary of Findings

In the exploration, some data wrangling was completed. 

The duration histogram was constructed which is right skewed. After applying log xscale transformation two modes were found at 4 and 13 minutes. Also, time of the day histogram is bimodal. It shows that the most popular hours of the day when bikes are taken for rides are 8am and 5pm. These time of the day correspnods to when people go to or coming from work. Log xscale transform just support our finding. Moreover, the relationship between hour of the day and day of the week shows that the most popular time when bikes are taken is 8am and 5pm while on weekends. We found that the the number of rides starts gradually increasing around 8-9am and gradually decreasing around 5-6pm . 

It is interesting to take a look at age and gender distributions. The first shows that 32 is the age when people use the bike sharing system the most. Moreover, it is interesting to note that men use bike sharing system **35 times more** often than women. In addition, bivariate exploration between age and gender was considered where we could see that males use bikes most often and after that the number of bike rides gradually decreasing. Women use bike sharing system most often at 26-35 years old and the number of rides is significantly lower compare to men at these ages. 

We found 4 the most popular starting stations and within this subset of dataset we found 4 the most popular arriving stations. On the route barchart it is shown that the most common route is between San Francisco Ferry Building station and Montgomery St BART Station. Facatgrid splitted by day of the week shows the distribution of log(duration). They have similar shapes but it is noticeable that on Weekends bikes are used significantly low number of time than during the weekdays. In addition to this plot a violin plot of duration for each popular route is shown. We can see that the routes # 1 and # 5 take more time with medians about 18 mins. The least time spent between station is for routes # 10 and # 11. 

One of the founding was that from Monday through Friday the average duration time is about 12.5-13 min, while on weekends this number increasing upto 18-19 minutes.  

Finally, multivariate exploration was conducted. The clustered barchart of the average duration with respect to day of the week splitted by gender was plotted. It shows that during the weekdays the average duration time is almost uniformly distributed. Man average duration time is abour 12 minutes and woman duration time is about 15 minutes. However, on weekends these number increases for men upto 15 minuts and for women it is about 23 minutes. In addition, the average duration was considered with respect ot gender and age. It shows that male duration time is less than it is for female. Men spend about 12-13 minutes on average when they are 26-70 years old. The maximum duration time for women is about 25 minutes when they are 61-65 years old.      


## Key Insights for Presentation

For the presentation, some plots were rearanged and subolotted with other plots in such way that they carry similar features. Our focus of interest was duration, demographic of riders, average time spent between popular stations. To satisfy ink to plot ration condition for the plot "Dependance of the duration mean value from the day of the week" it was changed from barchart to pointplot.  


## Conclusion 

According to this analysis now it is possible to better understand demographic of the users, time spent riding bikes, time spent between stations, and when bikes sharing system used most often. This information can help to develop a strategy to popularize more the bike sharing system for example using IT marketing targeting women or older people with advertisement. For olderly people it might be a solution by introducing 3 wheel bikes 

## Resources

* extracting month, day, year from datafram:  https://stackoverflow.com/questions/28009370/get-weekday-day-of-week-for-datetime-column-of-dataframe

* .cut method: https://pandas.pydata.org/pandas-docs/version/0.23.4/generated/pandas.cut.html

* udacity lectures

* python and pandas documentation
