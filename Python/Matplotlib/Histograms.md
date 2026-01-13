
Histograms are a visual representation of the distribution of quantitative data. They group values into bins(intervals) and counts how many fall in each range.

```python
import matplotlib.pyplot as plt
import numpy as np

# lets make a list of random score. loc is the median of the data, scale is the standard deviation aka the spread aka how far the scores deviate from the center, size is number of test scores
scores = np.random.normal(loc=80, scale=10, size=100)

# to make sure there arent scores that go below the standard deviation, we can use the clip function. second parameter we set anything below 70 as 0, and above 90 we set to 100. basically setting bounds. 
scores = np.clip(scores, 0, 100)
# bins changes number of bars there is for more specification
plt.hist(scores, edgecolor='black',
				 bins=20)
plt.show()
```