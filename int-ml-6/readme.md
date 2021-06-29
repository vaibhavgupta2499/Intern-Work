# Data Preprocessing in Machine Learning
   <img src="https://d33wubrfki0l68.cloudfront.net/ef9037172858e9d72c032c8f10eb952a81765a9c/bc453/static/f63c42dedc9dae7e8e0b6190a0a88f2f/28bdc/garbage-in.png">
  Now-a-day mostly everything depends upon the Data and when that data is converted into information it leads to major changes and profit for the community.
  But what if the data gathered itself is not proper for the Analysis?
  That is when need for Data preprocessing arises.
  Machine learning algorithms are data-hungry. But there’s a catch. They need data in a specific format.
  Data preprocessing is the most important phase of a Machine Learning project.
 
## Need for Data Preprocessing?
  Collecting data from number of sources results in out-of-range values, impossible data combination, missing values, etc. Analyzing this kind of data that has not been prepared     properly for analysis can lead to misleading results. For achieving better results from the applied model in Machine Learning projects the format of the data has to be in a       proper manner.If there is much irrelevant and redundant information present or noisy and unreliable data, then knowledge discovery during   the training phase is more difficult.   The product of data preprocessing is the final training set. It also helps to select the most efficient model in Machine Learning.

  
## What is Data Preprocessing and steps involved in it?
  The process of cleaning raw data for it to be used for machine learning activities and analysis is known as data pre-processing. It’s the first and foremost step while doing a     machine learning project. Data preprocessing bascially helps us to get rid of the issues(missing values, outliers, null vlaues, etc) that can affect our analysis.
  
  ### Steps involved in data preprocessing:
  #### 1. *Data Collection*
  #### 2. *Importing Libraries*
  #### 3. *Importing the dataset*
  #### 4. *Data quality assessment*
  #### 5. *Data cleaning*
  #### 6. *Data transformation*
  #### 7. *Data reduction*
  #### 8. *Splitting of dataset*
  #### 9. *Feature Scaling*
  
### Now let us discuss each steps furthur:

## *Data Collection*
   There are many types of data collection: surveys, phone calls, records, forms, clinical studies, and etc. You could either get it from a primary source (the data your company    collects through various means) or a secondary source (government data sets or online repositories).
   Think about the goal of your analysis to get an idea of what kind of data you need to acquire.Once the data is collected, comes the next stage of the analysis: the data          preparation process.

## *Importing the Libraries*
   In order to perform data preprocessing using Python, we need to import some predefined Python libraries. These libraries are used to perform some specific jobs. There are        three specific libraries that we will use for data preprocessing, which are:
   ### Numpy: 
   Numpy Python library is used for including any type of mathematical operation in the code. It is the fundamental package for scientific calculation in Python. It also            supports to add large, multidimensional arrays and matrices. So, in Python, we can import it as:
     
     import numpy as np;
   Here we have used np, which is alias for Numpy, and it will be used in the whole program.  
   
  ### Pandas:
  The Pandas library, which is one of the most famous Python libraries and used for importing and managing the datasets. It is an open-source data manipulation and analysis       library. It will be imported as below:
  
    import pandas as pd;
   Here we have used pd, which is alias for Pandas, and it will be used in the whole program. 
   
  ### Matplotlib:
   The  matplotlib, which is a Python 2D plotting library, and with this library, we need to import a sub-library pyplot. This library is used to plot any type    of charts in      Python for the code. It will be imported as below: 
     
     import matplotlib.pyplot as plt;
   Here we have used plt, which is alias for Matplotlib, and it will be used in the whole program.  

## *Importing the dataset*
   Now we need to import the datasets which we have collected for our machine learning project. Data can be in any of the popular formats - CSV, TXT, XLS/XLSX (Excel),etc.
   Check whether header row exists or not.
   
   ## importing csv file##
   It is important to note that a singlebackslash does not work when specifying the file path. You need to either change it to forward slash or add one more backslash like          below
     
    (name for the dataset)= **pd.read_csv**("(url of the file)")
   ## Importing file from url ##
   You don't need to perform additional steps to fetch data from URL. Simply put URL in read_csv() function (applicable only for CSV files stored in URL).
     
    mydata = pd.read_csv("http://winterolympicsmedals.com/medals.csv")
    
   ## Reading text file ##
   We can use read_table() function to pull data from text file. We can also use read_csv() with sep= "\t" to read data from tab-separated file.
     
    mydata = pd.read_table("C:\\Users\\Deepanshu\\Desktop\\example2.txt")
    mydata = pd.read_csv("C:\\Users\\Deepanshu\\Desktop\\example2.txt", sep ="\t")
  
  ## Reading excel file## 
   The read_excel() function can be used to import excel data into Python.
     
## *Data quality assessment*
  Take a good look at your data and get an idea of its overall quality, relevance to your project, and consistency. There are a number of data anomalies and inherent problems to   look out for in almost any data set, for example:
   * Mismatched Data types:  When you collect data from many different sources, it may come to you in different formats. 
   * Mixed data values: Perhaps different sources use different descriptors for features – for example, man or male. These value descriptors should all be made uniform.
   * Data outliers: Outliers can have a huge impact on data analysis results.Check for extreme and unusual values.
   * Missing data: Take a look for missing data fields, blank spaces in text. This could be due to human error or incomplete data.
 
## *Data Cleaning*
  Data cleaning is the process of adding missing data and correcting, repairing, or removing incorrect or irrelevant data from a data set. Data cleaning is the most important     step of preprocessing because it will ensure that your data is ready to go for your downstream needs.
  Data cleaning will correct all of the inconsistent data you uncovered in your data quality assessment. Depending on the kind of data you’re working with, there are a number of   possible cleaners you’ll need to run your data through.
  
   ## Remove unwanted data##
  The first step to data cleaning is removing unwanted observations from your dataset.This includes duplicate or irrelevant observations.Duplicate observations most               frequently arise during data collection, such as when you: Combine datasets from multiple places, Scrape data, Receive data from clients/other departments. Irrelevant           observations are those that don’t actually fit the specific problem that you’re trying to solve. For this performing EDA is best to take a look on this kind of data.
  
   ## Fix Structural Errors##
  Structural errors are those that arise during measurement, data transfer, or other types of "poor housekeeping".For instance, we can check for typos or inconsistent             capitalization. Check for mislabeled classes, i.e. separate classes that should really be the same.
      
   ## Handling Outliers##
   In statistics, an outlier is an observation point that is distant from other observations.They may be due to variability in the measurement or may indicate experimental          errors.If possible, outliers should be excluded from the data set. Outliers can be of two kinds: univariate and multivariate. Univariate outliers can be found when looking      at a distribution of values in a single feature space. Multivariate outliers can be found in a n-dimensional space (of n-features).
       
   *How we can identify an Outlier?*
   
   1. Using Box plots
   
     import seaborn as sns
     sns.boxplot((dataset name)['(column name)'])
   <img src="https://media.geeksforgeeks.org/wp-content/uploads/20210129184918/2boxplot.PNG">
   2. Using Scatter plot
   <img src="https://media.geeksforgeeks.org/wp-content/uploads/20210129184920/4scatterplot.jpg">
   3. Using Z score
    Z- Score is also called a standard score. This value/score helps to understand that how far is the data point from the mean. And after setting up a threshold value one           can utilize z score values of data points to define the outliers.
    Zscore = (data_point -mean) / std. deviation
        
         from scipy import stats
         import numpy as np
         z = np.abs(stats.zscore(df_boston['DIS']))
         print(z)
   <img src="https://media.geeksforgeeks.org/wp-content/uploads/20210129184922/6zscore.PNG">  
   
   *How we can we handle an Outlier?*
   
  * Sometimes it’s best to completely remove those records from your dataset to stop them from skewing your analysis. We delete outlier values if it is due to data entry error,     data processing error or outlier observations are very small in numbers. We can also use trimming at both ends to remove outliers. But deleting the observation is not a good     idea when we have small dataset.
  * Like imputation of missing values, we can also impute outliers. We can use mean, median, zero value in this methods. Since we imputing there is no loss of data. Here median     is appropriate because it is not affected by outliers.
  * Transforming variables can also eliminate outliers. These transformed values reduces the variation caused by extreme values.Scaling, Log transformation are some of the           techniques we can use.

 ## Handling Missing Values ##
 <img src="https://analyticsindiamag.com/wp-content/uploads/2018/02/missing-values.png">
 
 For checking the presence of null values, we use methods like: isnull() and notnull()
  
  
  <img src="https://analyticsindiamag.com/wp-content/uploads/2018/02/missing-values-1.png">
   
 **Ways for handling missing values**
    
   *Deleting those rows:* 
   This method is advised only when there are enough samples in the data set. One has to make sure that after we have deleted the data, there is no addition of bias. Removing      the data will lead to loss of information which will not give the expected results while predicting the output.
   
   <img src="https://analyticsindiamag.com/wp-content/uploads/2018/02/deleted.png">
   
   *Replacing those values with Mean/Median/Mode:*
   
   For selecting which statistic will be best for filling the null values we first have to note that the column is categorical or numerical.
   **For Categorical Feature**
     Categorical Data is the data that generally takes a limited number of possible values. Also, the data in the category need not be numerical, it can be textual in nature.
     Here we can either delete the null values or Replace missing values with the most frequent value ie. **Mode**
     
   <img src="https://lh5.googleusercontent.com/GCzo2EIXFKprf04UgMAv-BVDVCOoCXtZLVvisf9_wOtg7LaYFaoSQcT5ohDFrIJ1kxR2ax5BkwPt4Fs_2yiJJwEK0W767wO0K1dFkVM9b3gImpjKjsQ617QXLiE7mcOXzaZ6ZgM3">
   
   **For Numerical Feature**
     Mean as a measure is greatly affected by outliers or if the distribution of the data or column is not normally-distributed. Therefore, it’s wise to first check the              distribution of the column before deciding if to use a mean imputation or median imputation. 
     
   *Mean imputation works better if the distribution is normally-distributed or has a Gaussian distribution, while median imputation is preferable for skewed distribution(be it     right or left)*
   
   Also its much better if inplace of filling the null vlaues with a particular number(mean/median), we just fill the values with random function in the IQR.
   
   <img src="https://miro.medium.com/max/875/1*5FkrD3kR0Z96dsobQDYkcg.png">
   
## *Data Transformation*   
   
   
     
     
   
   
   
    
  
       
    
   
     
     
  



