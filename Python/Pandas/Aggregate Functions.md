

Aggregate functions reduce a set of values into a single summary value used to summarize and analyze data used with the groupby() function
```python
import pandas as pd

data = {'Name': ['Jack', 'James', 'Jimmy', 'John', 'Jorge'], 
		'Height' : [5.5, 5.8, 5.7, 5.95, 5.825],
		'Age' : [19, 18, 20, 22, 24]
}

df = pd.DataFrame(data, index_col=data['Name'])
print(df)
```