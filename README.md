# Handling-skewed-data-sets

import numpy as np

## create a sample skewed dataset
data = np.random.gamma(1, 10, 1000)

## plot the histogram of the skewed data
import matplotlib.pyplot as plt
plt.hist(data, bins=50)
plt.show()

## perform a log transformation on the skewed data
data_log = np.log(data)

## plot the histogram of the transformed data
plt.hist(data_log, bins=50)
plt.show()
