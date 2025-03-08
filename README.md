# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()
df.tail()
df.isnull()
df.notnull()
df.fillna(500)
df.dropna(axis=0)
df.dropna(axis=1)
df.info()
df.describe()
df.shape
df.isnull().sum()
df.isnull().any()
df.fillna(method='ffill')
df.fillna(method='bfill')
df.fillna({'GENDER':'MALE','NAME':'SRI','ADDRESS':'POONAMALLEE','M1':98,'M2':87,'M3':76,'M4':92,'TOTAL':305,'AVG':89})
sample=pd.read_csv("/content/iris.csv")
sample
sample.shape
sample.info()
sample.describe()

# Result
          <<include your Result here>>
