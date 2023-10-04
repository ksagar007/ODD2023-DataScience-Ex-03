# Ex03-Univariate-Analysis

# Aim:

To read the given data and perform the univariate analysis with different types of plots.

# Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:

# Step1:

Read the given data.

# Step2:

Get the information about the data.

# Step3:

Remove the null values from the data.

# Step4:

Mention the datatypes from the data.

# Step5:

Count the values from the data.

# Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:

# (1) Diabetes.csv

```py
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

# (2) SuperStore.csv

```python
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

# OUTPUT:

# DIABETES.csv
![Screenshot 2023-05-29 215840](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/9d0add0c-d13f-472f-a69c-e0c57e361d66)


## INFO

![Screenshot 2023-05-29 215847](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/eb41de83-33b1-49d3-a633-c052bbc57204)


## ISNULL.SUM
![Screenshot 2023-05-29 215852](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/e2178ba4-3332-48fd-8e37-9c0d5ce83756)



## DTYPES
![Screenshot 2023-05-29 215901](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/909c2582-3592-4640-acdb-dbc47f1df49a)



## DESCRIBE

![Screenshot 2023-05-29 215907](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/fbc725be-cf8d-4835-bcaf-7c88d2b6cfc8)


## VALUECOUNTS
![Screenshot 2023-05-29 215933](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/0013c23d-c434-4b47-88ad-6371ff591954)



## BOXPLOT

![Screenshot 2023-05-29 215937](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/edd09d03-c35d-46e2-8602-def08664f8d5)


## COUNTPLOT
![Screenshot 2023-05-29 215943](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/afda6a8a-85f3-4232-947a-0f0da0817c59)


## DISTPLOT
![Screenshot 2023-05-29 215950](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/9ee5512c-a490-4b83-922d-524833f519e8)


## HISTPLOT

![Screenshot 2023-05-29 215957](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/b365618e-85ac-410c-bc5c-63e149d9f9df)


## SKEW
![Screenshot 2023-05-29 220003](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/b881eb2c-dc39-4924-8bbf-9acec96e4baa)


## DISTPLOT SKEW

![Screenshot 2023-05-29 220012](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/78460e8f-e4af-4f38-9285-a8efc53a6576)


## HISTPLOT SKEW

![Screenshot 2023-05-29 220017](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/3e46e5f0-f4e1-4b1c-9f4b-b9432236d086)


## KURTOSIS
![Screenshot 2023-05-29 220022](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/8d585b2b-8825-4d40-8427-57c0f4654959)



## BOXPLOT KURTOSIS

![Screenshot 2023-05-29 220026](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/58547041-8833-453f-afc0-1ecc683f69b4)


# SUPERSTORE.csv

![Screenshot 2023-05-29 220040](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/8293005f-b788-46c1-a26e-7e56b6c28c07)

## ISNULL.SUM
![Screenshot 2023-05-29 220046](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/8e888348-2d64-40b2-99fd-283b4ab687c3)



## AFTER CLEANING

![Screenshot 2023-05-29 220052](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/74414b11-4f95-4e0b-8807-6f54d43e6637)


## DTYPES
![Screenshot 2023-05-29 220058](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/5d401b24-8e9d-4c7c-8027-899529fe6e1c)



## DESCRIBE

![Screenshot 2023-05-29 220104](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/2a1bb2a4-716e-44b9-b947-ea72085fe192)


## VALUECOUNTS

![Screenshot 2023-05-29 220109](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/a8718d96-7a69-4905-a2cc-38cd85ffa809)


## BOXPLOT

![Screenshot 2023-05-29 220114](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/487e1924-04bf-46d9-8e4f-c81933b1bd7f)


## COUNTPLOT
![Screenshot 2023-05-29 220120](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/9633286b-0ce4-4fac-b8be-28c442248ec9)


## DISTPLOT
![Screenshot 2023-05-29 220127](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/86b0e62f-4862-4943-9bb9-bb83a432393a)



## HISTPLOT

![Screenshot 2023-05-29 220134](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/4e190e5f-5fad-416e-aa75-9158667b5a50)


## SKEW
![Screenshot 2023-05-29 220140](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/8b5815a2-dceb-48af-8033-2d8a93422310)


## DISTPLOT SKEW

![Screenshot 2023-05-29 220147](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/9b23c8de-589b-4d4a-84fa-d9f8169871cd)


## HISTPLOT SKEW

![Screenshot 2023-05-29 220154](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/2d6b68cd-d413-46f8-9694-2a5a698a67dc)


## KURTOSIS
![Screenshot 2023-05-29 220200](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/ddfe8c10-2310-479f-8cb7-a30bfae04f75)



## BOXPLOT KURTOSIS

![Screenshot 2023-05-29 220205](https://github.com/Nagul71/Ex03-Univariate-Analysis/assets/118661118/82120631-f7f2-4bf3-816c-b1a1ffbcd1eb)


# RESULT:
Thus we have read the given data and performed the univariate analysis with different types of plots.
