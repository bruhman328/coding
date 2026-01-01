

Selection by column

```python
import pandas as pd

data = {
	'Name' : ['Spongebob', 'Mr. Krabs', 'Squidward'],
	'Hourly Pay' : [17, 100, 15]
}

df = pd.DataFrame(data, index=['Employee 1', 'Employee 2', 'Employee 3'])

print(df['Name'].to_string())
//can also put a lists of columns inside the brackets for multiple columns//
```

