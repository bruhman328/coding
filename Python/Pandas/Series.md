

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



Dictionaries have their own index names already
```python
import pandas as pd

data = {'Tim' : 15, 'Bob' : 19, 'Gilbert' : 17}

series = pd.Series(data)

print(series)
```



Updating values
- You can just use the basic +=, -=, etc operators to update any values
```python
import pandas as pd

data = [4, 5, 6]

series = pd.Series(data)
print(series)

series.iloc[1] += 5
print(series)
```



Locating using a specific range
```python
import pandas as pd

data = [1, 2, 3]

series = pd.Series(data)

print(series[series > 1])
```