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



## 4. PCA (*Principal Component Analysis*)
Principal Component Analysis is a multivariate analysis that transforms the original correlated variables into new, uncorrelated variables by reducing a number of these variables, so that they have smaller dimensions but can explain most of the diversity of the original variables. In this analysis, we will 2 methods of PCA: **Feature Selection** and **Feature Extraction.**

### - Feature Selection (FS)
Feature Selection is a process in PCA that selects certain features from a set of features. This method helps simplify, organize and shorten training time or it can be said that Feature Selection is used to remove features in data that are deemed unimportant. Here is the result of FS method:


![](/images/p12.png)


### - Feature Extraction (FE)
Feature Extraction is a process in PCA that converts raw data into several other types of data, which work with algorithms. Here is the result of FE method:


![](/images/p13.png)



## 5. K-Means Clustering
K-Means Clustering is one of the popular clustering algorithms. The purpose of this algorithm is to find groups (clusters) within the given data. So we can said that K-Means is a very simple algorithm that groups data into a number of K clusters. This following is a comparison of the scatter plot between raw data and data that has been grouped using the K-Means method.


| ![](/images/p14.png) | ![](/images/p15.png) | 
| ----------- | ----------- | 



## 6. Data Visualization using Pairplot
Pairplot is a graph used to determine the distribution of a variable and to determine the relationship between 2 variables. On the other hand, pairplots are a great method of identifying trends for follow-up analysis.


![](/images/p16.png)


In that pairplot, there are 12 scatterplots to determine the relationship between the two PCA variables and 4 histograms in the diagonal to see the distribution of each PCA variable. It can be seen that the PCA 2 variable histogram shows that the PCA 2 variable has a normal distribution visually, while the entire scatterplot shows that there is no linear relationship between each PCA variable.


## Conclusion
In this data analysis, it can be concluded that missing values must be handled first. Furthermore, PCA (Process Component Analysis) is carried out to classify and / or reduce variables. PCA that uses feature selection results in the initial 7 variables being reduced to 4 variables, while the feature extraxtion classifies the initial 7 variables into 2 variables.

At the last stage, clustering using K-means method, we got the number of clusters for Cervical Cancer (Risk Factors) data is divided into 2 clusters. For data visualization, a pair plot was used to determine the distribution and relationship between two variables and obtained for the PCA 2 variable visually normally distributed, while for all the scatterplots it showed that there was no linear relationship between each PCA variable.


