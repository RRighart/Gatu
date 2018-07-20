# Sensor time-series of aircraft engines
# Gatu

**Summary:**
The main question treated in the blog is if remaining useful lifetime (RUL) of an engine can be predicted using data from multiple sensors. The data that were used for this purpose are the C-MAPSS data, available at http://ti.arc.nasa.gov/project/prognostic-data-repository

**Original blog:**
https://rrighart.github.io/Gatu/

**Script:**
Gatu-script.ipynb

Python 2 was used (Python 3 may be used but may produce a few errors).

**Modules:**

import os
import pandas as pd
import numpy as np
np.random.seed(1337)
import requests, zipfile, StringIO
from IPython.display import Image
import matplotlib as mpl
import matplotlib.pyplot as plt
from pandas import read_csv
from matplotlib import pyplot as plt
from sklearn.metrics import mean_squared_error

from keras.models import Sequential
from keras.layers.core import Dense, Activation
from keras.wrappers.scikit_learn import KerasRegressor
from sklearn.model_selection import cross_val_score
from sklearn.preprocessing import StandardScaler
from sklearn.pipeline import Pipeline
from sklearn.preprocessing import MinMaxScaler

**Contact:**
rrighart@googlemail.com
