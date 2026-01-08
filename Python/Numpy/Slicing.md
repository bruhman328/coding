
Slicing means to output a specific range of indexes
- note that slicing is exclusive, so do n:m+1 or n::

```python
import numpy as np

a = np.array([
				[[1, 2, 3], [4, 5, 6]],
				[[7, 8, 9], [10, 11, 12]]
			])
	
print(a[0, 1, 1::])
```