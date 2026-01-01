

Selection by column

```python
import pandas as pd

data = {
	'Name' : ['Spongebob', 'Mr. Krabs', 'Squidward'],
	'Hourly Pay' : [17, 100, 15]
}

df = pd.DataFrame(data, index=['Employee 1', 'Employee 2', 'Employee 3'])

print(df['Name'].to_string())
# can also put a list of columns inside the brackets for multiple columns
```



Selection by row
```python
import pandas as pd

data = {
	'Name' : ['Spongebob', 'Mr. Krabs', 'Squidward'],
	'Hourly Pay' : [17, 100, 15]
}

df = pd.DataFrame(data, index=['Employee 1', 'Employee 2', 'Employee 3'])

df['Age'] = [30, 58, 32]
new_row = pd.DataFrame([{'Name' : 'Sandy', 'Hourly Pay' : 18, 'Age' : 27}], index=['Employee 4'])

df = pd.concat([df, new_row])

print(df)

print(df.loc['Employee 1':'Employee 3', ['Name', 'Hourly Pay']])
# can also put a list of rows inside the brackets for multiple rows
```