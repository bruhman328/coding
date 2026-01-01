
For CSV files
```python
import pandas as pd

df = pd.read_csv('name_of_file.csv')

print(df)
```



For JSON files
```python
import pandas as pd

df = pd.read_json('name_of_file.json')

print(df)
```



to_string()
- Since printing the file normally only shoes first 5 and last 5 rows, using the to_string() function prints the entire dataframe
- 