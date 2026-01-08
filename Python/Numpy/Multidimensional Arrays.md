
2D Array
- these are called ndarrays
	- used to store data in 2D, 3D, etc. and much more efficiently than lists
```python
import numpy as np
# 2D
a = np.array([[1, 2, 3],
			  [4, 5, 6]])
print(a[1, 2])
```

```python
import numpy as np
# 3D

a = np.array([
				[[1, 2], [3, 4]],
				[[5, 6], [7, 8]]
			])
print(a[0, 1, 0])
```