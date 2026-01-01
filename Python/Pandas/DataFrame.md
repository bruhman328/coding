
A DataFrame is a tabular data structure with rows AND columns. This means that it is 2 Dimensional, such as an Excel spreadsheet
```python
import pandas as pd

data = {
	'Name' : ['Spongebob', 'Mr. Krabs', 'Squidward'],
	'Hourly Pay' : [17, 100, 15]
}

df = pd.DataFrame(data, index=['Employee 1', 'Employee 2', 'Employee 3'])

print(df)
```


Adding a new column and row
```python
import pandas as pd

data = {
	'Name' : ['Spongebob', 'Mr. Krabs', 'Squidward'],
	'Hourly Pay' : [17, 100, 15]
}

df = pd.DataFrame(data, index=['Employee 1', 'Employee 2', 'Employee 3'])

print(df)

df['Age'] = [30, 58, 32]
new_row = pd.DataFrame([{'Name' : 'Sandy', 'Hourly Pay' : 18, 'Age' : 27}], index=['Employee 3']])

df = pd.concat([df, new_row])


print(df)

```

