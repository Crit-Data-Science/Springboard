# County Income Features Analyses

The economy consistently ranks as a top issue among voters in every election cycle. Economies are commonly ranked based on their prosperity or the average income of their population. wealthier nations also typically rank higher in studies of happiness<sub>[1](https://pubs.aeaweb.org/doi/pdfplus/10.1257/jep.22.2.53)</sub>. If politicians want to help their constituents or remain in office one of their cheifs goal needs to be enacating policies that encourage income growth. There is no single answer on how to achieve those goals. This analyses is aimed at looking for what features correlate most with higher incomes.

## 1. Data
The dataset used from this analyses was combined from two data sets from the Sensus Bureau. The first dataset is the Educational Attainment dataset for each county. The second data set is another combination of data from the ACS 2015 County Data.From the education data set i pulled out the high school and college graduation rates to merge with the other county data.

## 2. Method
The goal of this analsyses to be able to identify features that contribute to the growth of wages for individuals and families. A regression analyses will be run to see how predictable that income Per Capita is. What will also be run are classification models in an attempt to identifty counties that have much in common with the goal of finding out if there are grouping of counties that can be put together and studies further. To that end the two classification models that will be used are K-Means Classification and DBSCAN.

## 3. Data Cleaning
There was no missing data in the data sets. I filtered the data in the education data set down to the male and female gradation rates for both high school and college. I also included the overal high school and college graduates. To merge the the data sets I needed to isolate the names of the counties and then merge the data sets on those names to the smaller of the two data sets

## 4. EDA
![](https://github.com/Crit-Data-Science/Springboard/blob/main/Data%20Science%20Capstone%202%20Project/Data/Plots/IncomePerCap_Counts.png)
![](https://github.com/Crit-Data-Science/Springboard/blob/main/Data%20Science%20Capstone%202%20Project/Data/Plots/graduation_rates_by_incom.png) 
\n
The distributions appears normal with its right tail. The trend of education rates and income clearly trends positive.

## 5. Models






