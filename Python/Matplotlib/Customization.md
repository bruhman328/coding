
In Matplotlib, we can customize our plots. More specifically, the lines and markers

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([2, 4, 6])
y = np.array([10, 73, 129])

# marker will be what those points on the plot will show up as, you can use any symbol
plt.plot(x, y, marker='*')
plt.show()
```


```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([2, 4, 6])
y = np.array([10, 73, 129])

# we can also set the marker size
plt.plot(x, y, marker='*',
				markersize = 10)
plt.show()
```