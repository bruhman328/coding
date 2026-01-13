
Pie Charts are circular charts divided into slices to show percentages of the total. Good for visualizing distribution among categories

```python
import matplotlib.pyplot as plt
import numpy as np

categories = np.array(['Freshmen', 'Sophomores', 'Juniors', 'Seniors'])
count = np.array([134, 70, 154, 223])
colors = np.array(['red', 'cyan', 'purple', 'green'])

# autopct is to show percentages, to round to 1st decimal just add the .1, colors sets colors, explode makes which ever value is not 0 and is under 1 to pop out corresponding with the label index
plt.pie(count, labels=categories,
				autopct='%1.1f%%', 
				colors=colors, 
				explode=[0.2, 0, 0, 0])

plt.show()
```