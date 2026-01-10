
NumPy automatically expands the smaller array so shapes match.
- In order to broadcast, you must compare the shapes from right to left--for each dimension they must be either equal or one of them is 1, otherwise an error will occur
```python
import numpy as np

# 1 x 3
a = np.array([1, 2, 3])
# 1 x 1
b = np.array(6)
# this is compatible since right is equal and left has one 1
# 6 is broadcasted to [6, 6, 6]
print(a + b)
```