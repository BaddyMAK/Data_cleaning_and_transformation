# Data Cleaning and Data Transformation 

In this article, I am going to present you all important points you need to know and to master, as a data scientist,
about data cleaning and data transformation.

This two processes are fundamental and essential for any data science project. They aim to provide high quality,
consistent and reliable data to build your model, finding proper insights or trends and taking the right decision.



<div>
<img src="images/Data-Cleaning-scaled.jpeg "Data cleaning" width="500"/>
</div>

## Contents 

  1- Summary
  
  2- Data Cleaning
  
  3- Data Transformation 
  
  4- Conclusion 
  
## 1- Summary 

As a data scientist, working directly with raw data without performing any cleaning or transformation tasks could be useless and critical. Firstly, raw data is unclean, incoherent and poorly structured. Secondly, it may contain duplicates, missing and outdated values. Finally, computers cannot intuitively process raw data like a human mind can. 

Thus, if the data quality is not good enough, we will not be able to build a reliable model and then your project could fail easily. 

## 2- Data Cleaning
Data cleaning is the initial step that each data scientist must apply before starting any analysis or investigations and of course before applying any machine learning algorithm. It is a procedure that helps determine duplicate, missing, inconsistent samples and remove them. It improves data accuracy and increases data quality via discarding invalid and unwanted information.

In my notebook `data_cleaning_and_transformation` I have chosen one random dataset from Kaggle site :
[weather-dataset](https://www.kaggle.com/datasets/muthuj7/weather-dataset). This dataset conatins 12 columns and 96453 rows. The 12 features are the next : `Formatted Date`, `Summary`, `Precip Type`, `Temperature (C)`, `Apparent Temperature (C)`, `Humidity`, `Wind Speed (km/h)`, `Wind Bearing (degrees)`, `Visibility (km)`, `Loud Cover`, `Pressure (millibars)`, `Daily Summary`.

During the data cleaning phase, I had accomplished the next steps: 

- How to detect and Handle Duplicates
- How to detect and Handle missing values : removing or replacing them using KNNImputer, mean or median etc.
- How to deal with Categorical data : nominal and ordinal ones 
- How to detect and handle Outliers : performing some plots together with Interquartile range, Z-Score and 99th-percentile

Note : I have used various methods for the same tasks just to present you all and then you can choose whatever you want to apply in your code. 


## 3- Data Transformation 
The data transformation step could be required either before some data cleaning tasks or between data cleaning and Exploratory Data Analysis (EDA). Data transformation before data cleaning, is the process of converting data from one format to another such as from JSON to CSV or data aggregation etc. After data cleaning, this process helps convert our cleaned data into useful information and more significant features. 

Some examples of data transformation are:

•	Aggregation: concatenate data from multiple sources and store them into a single format. 

•	Normalization: transform attributes to be on a similar scale e.g., from 0 to 1, which ameliorate model performance and training stability. 

•	Standardization: rescale data values so that its mean will be 0 and its standard deviation will be 1. The new data distribution fits standard normal distribution. 

•	Manipulation: data is transformed to render it more readable and organized. 

•	Attribute construction: adding one new attribute or more from existing ones.

•	Etc

During the data transformation part, I have accomplished the next steps: 

- Data Normalization : means transforming features to be on a similar scale which improves the performance and training stability of the model. I have used :
    - Min-Max feature scaling (Normalization)
    - Maximum absolute scaling (Normalization)
    - Z-score method (Standardization Scaling)
    - Log scaling or Log transformation
  
- Transforming categorical values to numeric variables : both nominal and ordinal data were considered. I have used :
    - Python’s Category Encoder Library
    - Dummy Variable Encoding
    - Using Scikit-learn
    - Ordinal Encoding
    - How to choose the best Encoding Method 
  


## 4- Conclusion 
 
• Data cleaning returns high quality data which increases overall productivity, building valid model and simplify taking right decisions. 

•	Transformed data is easier to understand and to analyze either by computer or human.

• Raw data could be challenging to work with as it could be skewed and it has lot of defects.



