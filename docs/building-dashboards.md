---
title: "Building Your Dashboard"
parent: "Home"
nav_order: 4
---

# Building Your Dashboard  

## Understanding DataFrames (DFs)  
A **DataFrame (DF)** is a table-like structure used in Pandas.  

```python
import pandas as pd
df = pd.read_csv("your_data.csv")
df.head()  # Show first 5 rows
```
* [Pandas](https://pandas.pydata.org/docs/)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)

## Creating Basic Data Visualizations
```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.countplot(x='species', hue='height', data=df)
plt.title('Cats vs. Dog Height')
plt.show()
```
