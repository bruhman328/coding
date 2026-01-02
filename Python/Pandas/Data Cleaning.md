

Data cleaning is the process of fixing/removing: incomplete, incorrect, or irrelevant data


Drop irrelevant columns
```python
import pandas as pd

data = {'Name': ['Jack', 'James', 'Jimmy', 'John', 'Jorge'], 
		'Height' : [5.5, 5.8, 5.7, 5.95, 5.825],
		'Age' : [19, 18, 20, 22, 24]
}

df = pd.DataFrame(data)

df = df.drop(columns=['Age'])
print(df)
```