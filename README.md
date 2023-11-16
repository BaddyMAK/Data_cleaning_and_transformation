# Data Cleaning 

In this article, I am going to present you all important points you need to know and to master, as a data scientist,
about Data Preprocessing step mainly data cleaning task. Choosing the correct and the consistent data values helps build a robust machine learning model,
finding proper insights or trends and so taking the right decision.

Data cleaning is the initial step that should be accomplished within any data science project. 
It is an essential task that plays a significant role to improve raw data quality, to increase data coherence and accuracy 
and to ensure that findings are based on reliable information. 


Finally, it is important to evaluate how data cleaning has affected the results and conclusions of our data science project.
For example, to emphasise the role of data cleaning, we can compare the performance and accuracy of our machine learning model before and after cleaning. 


<div>
<img src="images/Data-Cleaning-scaled.jpeg "Data cleaning" width="500"/>
</div>

## Contents 

  1- Summary
  
  2- Data Reading
  
  3- Data Cleaning
  
  4- Conclusion 
  
## 1- Summary 

As a data scientist, working directly with raw data without performing any cleaning or transformation tasks could be useless and critical. Firstly, raw data is unclean, incoherent and poorly structured. Secondly, it may contain duplicates, missing and outdated values. Finally, computers cannot intuitively process raw data like a human mind can. 

Thus, if the data quality is not good enough, we will not be able to build a reliable model and then your project could fail easily. 

## 2- Data Reading 

Retrieving Data can be accomplished using multiple data sources such as: 

- Databases SQL/NOSQL : MySQL, Cassandra etc.
- Data lakes : Snowflake, S3 etc.
- APIs
- Cloud data sources
  
SQL databases uses structured data that is coming under the .csv and .tsv formats which are the most common formats for delimited data flat files. Sometimes, you can use special characters as separators such as white space or normal letter like 't', 'v' etc. However, NOSQL databases and APIs uses unstructured data stored under .JSON format, JSON corresponds to JavaScript Object Notation.

Another option for retrieving data could be the Parquet format using `read_parquet()` of our famous `pandas` library but it is not recommended to use it as it requires very high CPU usage.

## 3- Data Cleaning

Data cleaning is the initial step that each data scientist must apply before starting any analysis or investigations and of course before applying any machine learning algorithm. It is a procedure that helps determine duplicate, missing, inconsistent samples and remove them. It improves data accuracy and increases data quality via discarding invalid and unwanted information.

Data cleaning is the process of determining and fixing incorrect data. It can be in incorrect format, duplicates, corrupt, inaccurate, incomplete, or irrelevant etc.

In my notebook `data_cleaning_and_transformation` I have chosen one random dataset from Kaggle site :
[weather-dataset](https://www.kaggle.com/datasets/muthuj7/weather-dataset). This dataset conatins 12 columns and 96453 rows.

The 12 features are the next : `Formatted Date`, `Summary`, `Precip Type`, `Temperature (C)`, `Apparent Temperature (C)`, `Humidity`, `Wind Speed (km/h)`, `Wind Bearing (degrees)`, `Visibility (km)`, `Loud Cover`, `Pressure (millibars)`, `Daily Summary`. I have selected some of them for my accomplished tasks.  

During the data cleaning phase, I had performed the next steps: 

- How to detect and Handle **Duplicates** and removing them.
- How to detect and Handle **missing values (NaN)** : removing or impute them using KNNImputer, mean or median etc.
- How to deal with **Categorical data** : nominal and ordinal examples.
- How to detect and handle **Outliers** : performing some plots and visualisations together with Interquartile range, Z-Score and 99th-percentile

Note : I have used various methods for the same tasks just to present you all and then you can choose whatever you want to apply in your code. 


## 4- Conclusion 

• Raw data could be challenging to work with as it could be skewed and it has lot of defects.

• Multiple sources could be used to read data from such as databases, APIs, datalakes etc.

• Data cleaning returns high quality data which increases overall productivity, building valid model and simplify taking right decisions. 







