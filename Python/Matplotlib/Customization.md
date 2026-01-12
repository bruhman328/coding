
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

# we can also set the marker size or ms and markercolor(either rgb, hexadecimal, or name)
plt.plot(x, y, marker='*',
			   markersize=30,			           markerfacecolor='red')
plt.show()
```

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([2, 4, 6])
y = np.array([10, 73, 129])

# you can also customize the line style like dashed, dotted, dashdot, solid, or None(for no line). you can also change the line width
plt.plot(x, y, marker='*',
				linestyle='dashed',
				linewidth=4)
plt.show()
```