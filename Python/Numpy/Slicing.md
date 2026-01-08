
Slicing means to output a specific range of indexes
- note that slicing is exclusive, so 

```python
import numpy as pd

a = np.array([
				[[1, 2, 3], [4, 5, 6]],
				[[7, 8, 9], [10, 11, 12]]
			])
	
print(a[0, 1, 1])
```