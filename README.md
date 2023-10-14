# Ex03-Univariate-Analysis

## Aim:
To read the given data and perform the univariate analysis with different types of plots.

## Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm:
Step1:
Read the given data.

Step2:
Get the information about the data.

Step3:
Remove the null values from the data.

Step4:
Mention the datatypes from the data.

Step5:
Count the values from the data.

Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program:
### (1) Diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
sns.distplot(df["Glucose"])
sns.histplot(x="Glucose",data = df)
df.kurtosis()
sns.boxplot(x="Glucose",data=df)
```

### (2) SuperStore.csv
```
df2 = pd.read_csv("/SuperStore.csv")
df2.head()
df2.isnull().sum()
df2['Postal Code'] = df2["Postal Code"].fillna(df2['Postal Code'].mode()[0])
df2.isnull().sum()
df2.dtypes
df2.describe()
df2['Sales'].value_counts()
sns.boxplot(x="Sales",data=df2)
sns.countplot(x="Sales",data=df2)
sns.distplot(df2['Sales'])
sns.histplot(x="Sales",data=df2)
df2.skew()
sns.distplot(df2["Postal Code"])
sns.histplot(x="Postal Code",data = df2)
df2.kurtosis()
sns.boxplot(x="Row ID",data=df2)
```

## OUTPUT:
### DIABETES.csv
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/f4ffbedd-5a04-454e-a8b8-264fe7fa7445)

### INFO
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/4c9866bc-10d2-4b04-824e-b2f5112c7584)

### ISNULL.SUM
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/6a61cd6a-9e7f-40be-b898-dfdf9fd2ecbd)

### DTYPES
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/e20ace77-96bb-41d7-aac1-5eaf0022ab68)

### DESCRIBE
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/a73b76f6-d75a-4098-a875-aaa023a9f9ec)

### VALUECOUNTS
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/ff24998b-4ca2-4094-a30b-448751d872ee)

### BOXPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/1da54175-be1b-4fbf-a706-92df3e2a7782)

### COUNTPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/a9294558-4ec0-4aab-a4ab-b6c001febca5)

### DISTPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/72bbd8ab-0043-48b9-a7a1-8501fc0a9e16)

### HISTPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/d9a03e8a-bb96-44ac-91b6-09e6e9523184)

### SKEW
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/83a2ac3f-8f49-4000-93f1-857691b902ee)

### DISTPLOT SKEW
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/9eb7144d-9d66-463e-b28d-f727eb263fa5)

### HISTPLOT SKEW
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/79a38818-8f39-4206-b79c-c859ca6e9135)

### KURTOSIS
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/01146438-f100-43b8-8942-9a38c35f31f4)

### BOXPLOT KURTOSIS
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/65d73f32-3cbe-424d-aa10-5dbfaa43f2b9)

### SUPERSTORE.csv
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/52e4bdd1-7fe3-4190-9780-98a1eecd26c1)

### ISNULL.SUM
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/1eb0b5a5-c1f8-491d-a570-1bc425300d0c)

### AFTER CLEANING
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/4c0f3431-3450-4748-93e6-c75f0ccf234f)

### DTYPES
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/181a6d0e-e105-43e0-b2da-969ddbca355c)

### DESCRIBE
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/9d568a1b-9be6-4463-8e36-cb24b5f65f9f)

### VALUECOUNTS
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/d0afaf75-d015-4b53-91a1-fcf908846363)

### BOXPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/de15b88e-858f-4b49-880e-8ef11d88896f)

### COUNTPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/d84149bc-4e0e-4df7-8476-b9f320cb39eb)

### DISTPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/b738acfd-e7ea-4edc-b9fa-92fa8e5edf57)

### HISTPLOT
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/6decf40c-90e1-4370-aa51-40e0aa85b876)

### SKEW
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/0b861a04-a6a0-453b-9656-3a9c744f8c5c)

### DISTPLOT SKEW
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/bd00315b-b411-4d1d-a94b-25d78bf9eb0e)

### HISTPLOT SKEW
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/0b86d72b-f6da-4250-8efa-78950b557177)

### KURTOSIS
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/ac9db8bc-0b23-42f1-92ec-16666d580ce7)

### BOXPLOT KURTOSIS
![image](https://github.com/Priya-Loganathan/ODD2023-DataScience-Ex-03/assets/121166075/b0c07764-b581-4412-a975-ad6dc7098cb1)


## RESULT:
Thus we have read the given data and performed the univariate analysis with different types of plots.



