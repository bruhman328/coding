
In Matplotlib, we can customize our plots. More specifically, the lines and markers

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([2, 4, 6])
y = np.array([10, 73, 129])

# marker will be what those 
plt.plot(x, y, marker='*')
plt.show()
```