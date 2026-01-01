

Filtering = Keeping the rows that match a condition

```python
import pandas as pd

data = {
	'Name' : ['Spongebob', 'Mr. Krabs', 'Squidward'],
	'Hourly Pay' : [17, 100, 15]
}

df = pd.DataFrame(data, index=['Employee 1', 'Employee 2', 'Employee 3'])


df['Age'] = [30, 58, 32]
new_row = pd.DataFrame([{'Name' : 'Sandy', 'Hourly Pay' : 18, 'Age' : 27}], index=['Employee 3'])

df = pd.concat([df, new_row])

young_ones = df[df['Age'] < 50]

print(young_ones)
```