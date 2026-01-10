
In NumPy, filtering means selecting elements that satisfy a condition

```python
import numpy as np

ages = np.array([[16, 17, 21, 30, 18, 59], 
				[55, 19, 28, 45, 23, 70]])
				
teens = ages[ages < 18]
adults = ages[(ages >= 18) & (ages < 45)]
elderly = ages[ages >= 45]
print('teens: ', teens)
print('adults: ', adults)
print('elderly: ', elderly)
```


where function
- will preserve shape of array and fill the elements in the array with whatever character or number if it doesn't meet a condition
```python
import numpy as np 

ages = np.array([[16, 17, 21, 30, 18, 59], 
				[55, 19, 28, 45, 23, 70]])
				
adults = np.where(ages >= 18, ages, -1)
print(adults)
```