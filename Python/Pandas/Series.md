

Series
- A series a is a pandas 1-Dimensional label array that can hold any data type
	- Sort of like a single column in a spreadsheet
```python
import pandas as pd

data = [1, 2, 3]

series = pd.Series(data)

print(series)

```


 
- You can set a specific index, so it doesn't only have to be labeled by numbers
	- ```python
	  import pandas as pd
	  
	  ages = [23, 27, 12]
	  
	  series = pd.Series(ages, index=['John', 'Adam', 'Becky'])
	  
	  print(series)
	  ```



loc and iloc
- loc is used to locate the value at a specific index, even if the index key is a string
- iloc is used to locate the value at a specific index, using an integer. Whether its the first index or the last index or whatever
- ```python
  import pandas as pd

  ages = [23, 27, 12]
	  
  series1 = pd.Series(ages, index=['John', 'Adam', 'Becky'])
  
  data = [1, 2, 3]

  series2 = pd.Series(data)
  
  print(series1.loc['Adam'])
  print(series2.iloc[0])
  ```
