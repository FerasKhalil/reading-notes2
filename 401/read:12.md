# Read: Class 12
## Pandas in 10
- Pands is free python library that gives set of tools for data analysis
- you can see the count of the records
- you can do so much with few lines of code
- to import:
	In [1]: import numpy as np
	In [2]: import pandas as pd

- Object creation
Creating a Series by passing a list of values, letting pandas create a default integer index:
	In [3]: s = pd.Series([1, 3, 5, np.nan, 6, 8])
	In [4]: s
	Out[4]: 
	0    1.0
	1    3.0
	2    5.0
	3    NaN
	4    6.0
	5    8.0
	dtype: float64
		- from(https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)



- pandas primarily uses the value np.nan to represent missing data. It is by default not included in computations. 
	- from (https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)


- use concat() to combine Series and DataFrame objects with various kinds of set logic for the indexes and 
	relational algebra functionality in the case of join / merge-type operations.

- can merge
- group refers to a process  involving one or more of the following steps:
	- **Splitting** the data into groups
	- **Applying** a function to each group independently
	- **Combining** the results into a data structure
		- from (https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)
- can read and write to excel
- can also read and write to HDF5

- Pandas uses fast, flexible, and expressive data structures designed to make working with relational or labeled data 
	both easy and intuitive