# Data Cleaning 

In this article, I am going to present you all important points you need to know and to master, as a data scientist,
about data cleaning. 

Data cleaning is a fundamental and an essential step for any data science project.
It is the first task that must be accomplished by any data scientist when obtaining the raw data for first time. 

Finally, Data cleaning aims to provide high quality, consistent and reliable data to build our machine learning model,
finding proper insights or trends and taking the right decision.

<div>
<img src="images/Data-Cleaning-scaled.jpeg "Data cleaning" width="500"/>
</div>

## Contents 

  1- Summary
  
  2- Data Cleaning
  
  3- Conclusion 
  
## 1- Summary 

As a data scientist, working directly with raw data without performing any cleaning or transformation tasks could be useless and critical. Firstly, raw data is unclean, incoherent and poorly structured. Secondly, it may contain duplicates, missing and outdated values. Finally, computers cannot intuitively process raw data like a human mind can. 

Thus, if the data quality is not good enough, we will not be able to build a reliable model and then your project could fail easily. 

## 2- Data Cleaning
Data cleaning is the initial step that each data scientist must apply before starting any analysis or investigations and of course before applying any machine learning algorithm. It is a procedure that helps determine duplicate, missing, inconsistent samples and remove them. It improves data accuracy and increases data quality via discarding invalid and unwanted information.

In my notebook `data_cleaning_and_transformation` I have chosen one random dataset from Kaggle site :
[weather-dataset](https://www.kaggle.com/datasets/muthuj7/weather-dataset). This dataset conatins 12 columns and 96453 rows.

The 12 features are the next : `Formatted Date`, `Summary`, `Precip Type`, `Temperature (C)`, `Apparent Temperature (C)`, `Humidity`, `Wind Speed (km/h)`, `Wind Bearing (degrees)`, `Visibility (km)`, `Loud Cover`, `Pressure (millibars)`, `Daily Summary`. I have selected some of them for my accomplished tasks.  

During the data cleaning phase, I had performed the next steps: 

- How to detect and Handle Duplicates and removing them.
- How to detect and Handle missing values : removing or replacing them using KNNImputer, mean or median etc.
- How to deal with Categorical data : nominal and ordinal examples.
- How to detect and handle Outliers : performing some plots and visualisations together with Interquartile range, Z-Score and 99th-percentile

Note : I have used various methods for the same tasks just to present you all and then you can choose whatever you want to apply in your code. 

## 3- Conclusion 

• Raw data could be challenging to work with as it could be skewed and it has lot of defects.

• Data cleaning returns high quality data which increases overall productivity, building valid model and simplify taking right decisions. 





