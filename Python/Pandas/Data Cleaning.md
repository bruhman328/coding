

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


Dropping missing data
```python
import pandas as pd
import numpy as np

data = {'Name': ['Jack', 'James', 'Jimmy', 'John', 'Jorge'], 
		'Height' : [5.5, 5.8, np.nan, 5.95, 5.825],
		'Age' : [19, 18, 20, 22, 24]
}

df = pd.DataFrame(data)

df = df.dropna(subset=['Height'])
print(df)
```



Filling missing data
```python
import pandas as pd
import numpy as np

data = {'Name': ['Jack', 'James', 'Jimmy', 'John', 'Jorge'], 
		'Height' : [5.5, 5.8, np.nan, 5.95, 5.825],
		'Age' : [19, 18, 20, 22, 24]
}

df = pd.DataFrame(data)

df = df.fillna({'Height' : 6.1})
print(df)
```



Fix inconsistent values
```python
import pandas as pd
import numpy as np

data = {'Name': ['Jack', 'James', 'Jimmy', 'John', 'Jorge'], 
		'Height' : [5.5, 5.8, np.nan, 5.95, 5.825],
		'Age' : [19, 18, 20, 22, 24]
}

df = pd.DataFrame(data)

df
print(df)
```
