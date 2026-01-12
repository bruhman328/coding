
Matplotlib allows us to create plots of data, this is very helpful in several scenarios such as finance or measuring 

```python
import matplotlib.pyplot as plt
# create x coordinates
x = [2023, 2024, 2025]
# create y coordinates
y = [6500, 7600, 9700]

# creates a plot with the x & y coordinates
plt.plot(x, y)

# if you don't call the show function, you cant see the plot
plt.show()

```

```python
import matplotlib.pyplot as plt

y = [5, 10, 15]

# plotting only the y values defaults the x values to have increments of 1
plt.plot(y)
plt.show()

```

```python
import matplotlib.pyplot as plt
import numpy as np
# we can also use numpy arrays since they are faster than lists and give more functionality

x = np.array([4, 8, 12])
y = np.array([25, 38, 52])

plt.plot(x, y)
plt.show()
```