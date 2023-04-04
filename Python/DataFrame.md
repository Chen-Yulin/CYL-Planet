---
id: "DataFrame"
aliases:
  - "Creating a DataFrame"
tags:
  - "dataframe"
  - "python"
---

# Creating a DataFrame
```python
import pandas as pd
df = pd.read_csv("a.csv")
df = pd.DataFrame({dict_t}) #convert a dict to a dataframe
df = Series_t.to_frame()
```
---
# Location
```python
df.loc[0:4,"Year":"Party"]
df.loc[[1,2,5],["Year","Candidate"]]
df.loc[:,["Year","Candidate"]]
df.loc[:,"year"] # return series
df.loc[1,"year":"Party"] # return series
df.shape[0] # count of row
df[["Year","Candidate"]][0:5]
```
---
# type transforming
```python
df['column_name'] = df['column_name'].astype(int)
df['column_name'] = df['column_name'].astype(float)
df['column_name'] = df['column_name'].astype(str)
```
---
# Groupby and agg
```python
df.groupby('column_name').agg(['sum', 'mean', 'max', 'min'])
df.groupby(['column_name_1', 'column_name_2']).agg({'column_name_3': ['sum', 'mean'], 'column_name_4': ['max', 'min']})
df.groupby(['column_name_1', 'column_name_2']).agg(['sum', 'mean', 'max', 'min'])
```




