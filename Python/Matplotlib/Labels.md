
```python
import matplotlib.pyplot as plt
import numpy as np 

x = np.array([2023, 2024, 2025, 2026])
y1 = np.array([15, 25, 30, 20])
y2 = np.array([17, 23, 38, 5])
y3 = np.array([13, 15, 20, 30])

# we can set a title 
plt.title('Class size', fontsize=25,
						family='Arial',
						fontweight='bold',
						color='red')

# we can set a x and y axis label
plt.xlabel('Year', fontsize=20, family='Arial')
plt.ylabel('Count', fontsize=20, family='Arial')

# we can also force ticks to display only at the the given points instead of the numbers between each tick
plt.xticks(x)

plt.plot(x, y1)
plt.plot(x, y2)
plt.plot(x, y3)

plt.show()
```