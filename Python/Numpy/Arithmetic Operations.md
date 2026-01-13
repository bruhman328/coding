

numpy allows you to do arithmetic operations between 2 array's, unlike lists

```python
import numpy as np

array1 = np.array([1, 2, 3])
array2 = np.array([4, 5, 6])

print(array1 + array2)
print(array2 - array1)
print(array1 * 2)

```


Comparison operators
- numpy allows you to also output the values that fit a comparison
```python
import numpy as np

array1 = np.array([1, 2, 3])
print(array1 > 1)
```

```python
import numpy as np

array1 = np.array([1, 2, 3])

# np.pi is pi
array1[array1 > 1] = np.pi
print(array1)
```