
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

# you can also customize the line style like dashed, dotted, dashdot, solid, or None(for no line). you can also change the line width, line color

plt.plot(x, y, marker='*',
				linestyle='dashed',
				linewidth=4,
				color='green',)
plt.show()
```

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([2, 4, 6])
y1 = np.array([10, 73, 129])
y2 = np.array([55, 23, 87])

# you can also plot multiple different lines, through using different x and y values

plt.plot(x, y1)
plt.plot(x, y2)
plt.show()
```

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([2, 4, 6])
y1 = np.array([10, 73, 129])
y2 = np.array([55, 23, 87])

line_style = dict(marker='*',
			   markersize=30,			           markerfacecolor='red',)
# now if you wanna use the same customization for both lines, you could just copy it but the best way is to place it into a dictionary
plt.plot(x, y, marker='*')
plt.show()
```