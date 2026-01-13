
A figure is the entire canvas in which we plot to. An ax is a single plot(subplot), which is technically a numpy array

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([1, 2, 3, 4, 5])

# subplots(rows, columns)
figure, axes = plt.subplots(2, 1)

# don't necessarily need to use plot, you can use other graphs too like bar graph 
axes[0].plot(x, x**2, color='red')
axes[0].set_title('Power of 2')

axes[1].bar(x, x**5, color='blue')
axes[1].set_title('Power of 5')

plt.show()
```