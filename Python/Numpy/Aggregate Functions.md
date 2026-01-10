
```python
import numpy as np

a = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

print(np.sum(a))
print(np.mean(a))
print(np.std(a)) # measure of spread of data, statistics term
print(np.var(a)) # square of standard deviation
print(np.min(a))
print(np.max(a))
print(np.argmin(a)) # position of min val
print(np.argmax(a)) # position of max val
print('----------------------------------')
print(np.sum(a, axis=1)) # outputs sum of rows
print(np.sum(a, axis=0)) # outputs sum of col
```