
Bar charts are used to compare categories of data by representing each category with a bar

```python
import matplotlib.pyplot as plt
import numpy as np

categories = np.array(['Grains', 'Fruit', 'Dairy', 'Vegetables', 'Protein'])
values = np.array([4, 1, 7, 3, 8])

plt.title('Daily Consumption')
plt.xlabel('Foods')
plt.ylabel('Quantity')

plt.bar(categories, values)
plt.show()
```