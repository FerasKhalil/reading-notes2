# Read: Class 11 Data Analysis

## What is Jupyter Lab
- jupyter supports many file formats
	- Json
	- .HDF5
- pdf, html, tex are all viewed easily

-jupyter has 2 modes:
	1. when it opens you are in command mode. 
		- command mode is for navigating and changing the framework of your notebook
		- to add a cell above use 'a', to add a cell below use 'b'.
		- copy a cell with 'c'
		- paste with 'v'
		- cut with 'x'
		- delete by pressing 'd' twice
		- press 'z' to undo
		- to redo use shift+'z'
		- to change the format to code use 'y'
		- to change format to markdown use 'm'
		- press '0' twice to restart the kernel
	2. Edit mode: 
		- press enter to edit the currently active cell
		- to see the result press shit+enter
		- use '>' in markdown for a blackqoute
		- shift+enter will run your python code after pressing 'y' to change to code mode



## Numpy Tutorial
- Numpy is a data analysis python package
- using Numpy can speed up your workflow 
-In a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis.
	 So the rows are the first axis, and the columns are the second axis.


-to create a Numpy array our code would be similar to this:
	import numpy as np
	wines = np.array(wines[1:], dtype=np.float)
	
	-from(https://www.dataquest.io/blog/numpy-tutorial-python/)