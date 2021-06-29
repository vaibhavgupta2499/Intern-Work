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
   
   * importing csv file
     It is important to note that a singlebackslash does not work when specifying the file path. You need to either change it to forward slash or add one more backslash like          below
     
    (name for the dataset)= **pd.read_csv**("(url of the file)")
   * Importing file from url
     You don't need to perform additional steps to fetch data from URL. Simply put URL in read_csv() function (applicable only for CSV files stored in URL).
     
    mydata = pd.read_csv("http://winterolympicsmedals.com/medals.csv")
    
   * Reading text file
     We can use read_table() function to pull data from text file. We can also use read_csv() with sep= "\t" to read data from tab-separated file.
     
    mydata = pd.read_table("C:\\Users\\Deepanshu\\Desktop\\example2.txt")
    mydata = pd.read_csv("C:\\Users\\Deepanshu\\Desktop\\example2.txt", sep ="\t")
  
  * Reading excel file
    The read_excel() function can be used to import excel data into Python.
     
     
    
   
     
     
  



