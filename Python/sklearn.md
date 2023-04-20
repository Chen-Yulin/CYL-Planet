---
id: "sklearn"
aliases:
  - "Some basic operation"
tags:
  - "python"
  - "sklearn"
  - "numpy"
---

# Some basic operation

## Shuffle the training set for hold out validation
```python
from sklearn.utils import shuffle
training_set,dev_set = np.split(shuffle(data_sample_35),[25])
```
Also capable of spliting training set, validation(development) set, test set


