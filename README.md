# K means Clustering
Clustering Analysis on Cervical Cancer Dataset using K-means method.



## Overview
The data for this analysis was obtained from the UCI Machine Learning Repository, namely the [Cervical Cancer (Risk Factors) Data Set](https://archive.ics.uci.edu/ml/datasets/Cervical+cancer+%28Risk+Factors%29). The dataset was collected at the 'Hospital Universitario de Caracas' in the city of Caracas, Venezuela, and consisted of demographic information, habits, and historical medical records from 858 patients. Some patients decided not to answer some questions because of privacy concerns so that there were missing values in several variables. The variables used in this study are 7 variables with integer and float data types.

![](/images/p1.png)

These are the steps to do clustering analysis process:


## 1. Pre-processing Missing Value
At this step, we will detect the missing value and resolve that missing value using imputation. 
The number of missing value for each variable and the result of imputation looked as follows:


![](/images/p2.png)


![](/images/p3.png)



## 2. Statistical Descriptive
Using statistical descriptive it can be seen the data characteristics of each variable.

![](/images/p4.png)

## 3. Outlier Detection
Outliers are extreme values that deviate from other observations on data and don't fit in some way. For the visualization of outliers, we can use the boxplot as follows:

| **Boxplot** | ![](/images/p5.png) | ![](/images/p6.png) | ![](/images/p7.png) |
| ----------- | ----------- |  ----------- |  ----------- |
| ![](/images/p8.png) | ![](/images/p9.png) | ![](/images/p10.png) | ![](/images/p11.png) |
