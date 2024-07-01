# County Income Features Analyses

The economy consistently ranks as a top issue among voters in every election cycle. Economies are commonly evaluated based on their prosperity or the average income of their population. Wealthier nations also typically rank higher in studies of [happiness](https://pubs.aeaweb.org/doi/pdfplus/10.1257/jep.22.2.53). If politicians want to help their constituents or remain in office, one of their chief goals needs to be enacting policies that encourage income growth. There is no single answer on how to achieve those goals. This analysis aims to identify the features that correlate most with higher incomes.

## 1. Data
The dataset used for this analysis was combined from two sources from the Census Bureau. The first dataset is the Educational Attainment dataset for each county. The second dataset is from the ACS 2015 County Data. From the education dataset, I extracted the high school and college graduation rates to merge with the other county data.

## 2. Method
The goal of this analysis is to identify features that contribute to the growth of wages for individuals and families. A regression analysis will be conducted to see how predictable the income per capita is. Additionally, classification models will be run in an attempt to identify counties with similar characteristics, with the goal of finding out if there are groups of counties that can be studied further. The two classification models that will be used are K-Means Clustering and DBSCAN.

## 3. Data Cleaning
There was no missing data in the datasets. I filtered the education dataset to include the male and female graduation rates for both high school and college. I also included the overall high school and college graduation rates. To merge the datasets, I isolated the county names and then merged the datasets based on these names.

## 4. EDA
![](https://github.com/Crit-Data-Science/Springboard/blob/main/Data%20Science%20Capstone%202%20Project/Data/Plots/IncomePerCap_Counts.png)
![](https://github.com/Crit-Data-Science/Springboard/blob/main/Data%20Science%20Capstone%202%20Project/Data/Plots/graduation_rates_by_incom.png) 
\n
The income distribution appears normal with a right tail. The trend of education rates and income shows a clear positive correlation.

## 5. Models

The best-performing model was the regression model without any scaled features. It was the only model that provided significant insights into the data. None of the models perfectly fit the data. The classification models were unable to provide accurate groupings of the data using relevant features. The regression model provided reasonable predictions. An interesting outlier was a county where the regression model predicted a negative value, which would be worth further investigation.

## 6. Conclusions
The data shows that education had the strongest correlation with income per capita. There did not seem to be a difference in the correlation between men and women. Attracting educated workers should yield benefits. Commute times also showed a definitive positive correlation with income per capita. This correlation could be due to a confounding effect, where people who earn more can afford larger homes located further from their workplaces.

## 7. Improvements
The data was well-documented and complete, but more detailed breakdowns of the features would be helpful. Breakdowns by age, job title, and degree would be good starting points for increasing the usefulness of the data. It would also be beneficial to spend more time analyzing the dataset and each of its features to better understand potential confounding variables.





