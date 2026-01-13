
Scatter plots/graphs show the relationship between two variables. This helps to identify a correlation (+, -, none). Example: Study hours vs test scores.

```python
import matplotlib.pyplot as plt
import numpy as np

x = np.array([0, 2, 3, 1, 5, 3, 8, 2, 3, 7])
y = np.array([45, 65, 73, 54, 82, 70, 95, 64, 78, 89])

x2 = np.array([3, 1, 5, 7, 5, 7, 6, 4, 9, 3])
y2 = np.array([75, 50, 85, 92, 82, 93, 88, 65, 98, 69])

plt.scatter(x, y, color='red',
				  label='Class A')
plt.scatter(x2, y2, color='skyblue',
					label='Class B')

# we call legend function to add legend			
plt.legend()
plt.show()

```