

Aggregate functions reduce a set of values into a single summary value used to summarize and analyze data used with the groupby() function
```python
import pandas as pd

data = {'Name': ['Jack', 'James', 'Jimmy', 'John', 'Jorge'], 
		'Height' : [5.5, 5.8, 5.7, 5.95, 5.825],
		'Age' : [19, 18, 20, 22, 24]
}

df = pd.DataFrame(data)

# Whole DataFrame

print(df.mean(numeric_only=True))
print(df.sum(numeric_only=True))
print(df.min(numeric_only=True))
print(df.max(numeric_only=True))
print(df.count())

# Single Column
print(df['Age'].mean())
print(df['Age'].sum())
print(df['Age'].min())
print(df['Age'].max())
print(df['Age'].count())
```



groupby() function
- You can use this function to group together rows such as the 