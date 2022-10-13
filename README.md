# Workshop-Multivariate-analysis


## Aim
To perform Multivariate EDA on the given data set.

##Explanation
Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

## Algorithm

### Step1
Import the built libraries required to perform EDA and outlier removal.

### Step2
Read the given csv file.

### Step3
Convert the file into a dataframe and get information of the data.

### Step4
Return the objects containing counts of unique values using (value_counts()).

### Step5
Plot the counts in the form of Histogram or Bar Graph.

### Step6
Use seaborn the bar graph comparison of data can be viewed.

### Step7
Find the pairwise correlation of all columns in the dataframe.corr()

### Step8
Save the final data set into the file.

### Types of bivariate analyis
    1)Numerical & Numerical(Scatter plot)
    2)Numerical & Categorical(Bar plot,Box plot,Dist plot)

## Code

```
Developed by : VISHAL GOWTHAMAN K R
Registration Number : 212221230123
```

```
import pandas as pd
import numpy as py
import seaborn as sns
import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)
df.corr()

```

## Output

### Data Head
![](./1.png)

### Data Information
![](./2.png)

###  Numerical & Numerical(Scatter plot)
![](./3.png)

### Numerical & Categorical(Bar plot)
![](./4.png)

### Non-Graphical method(correlation)
![](./5.png)

## Result
Thus we have performed Multivariate EDA on the given data set.
