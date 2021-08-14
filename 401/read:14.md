# Matplotlib Tutorial
- matplotlib is probably the single most used Python package for 2D-graphics
- can change colors and line widths
### IPython
- IPython is an enhanced interactive Python shell that has lots of interesting 
	features including named inputs and outputs, access to shell commands, improved debugging and much more.
	 When we start it with the command line argument -pylab (--pylab since IPython version 0.12),
	 it allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality.

	-from (https://github.com/rougier/matplotlib-tutorial)

### pyplot
- pyplot provides a convenient interface to the matplotlib object-oriented plotting library.
	 It is modeled closely after Matlab(TM). Therefore, the majority of plotting commands
	 in pyplot have Matlab(TM) analogs with similar arguments. Important commands are explained with interactive examples.
	- from (https://github.com/rougier/matplotlib-tutorial)


- to draw sine and cosine functions on the same plot 
	- the first step is to get the data for sine and cosine
	- import numpy as np
	X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
	C, S = np.cos(X), np.sin(X)
	
	- to make line for both sine and cosine thicker while changing cosine line to blue and cosine line to be in red we use this code:
	plt.figure(figsize=(10,6), dpi=80)
	plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")
	plt.plot(X, S, color="red",  linewidth=2.5, linestyle="-")


- can add a legend and assign its location to be wherever you prefer
- can also add ticks.
- ticks have a lot of types:
	- NullLocator: no ticks
	- IndexLocator: Place a tick on every multiple of some base number of points plotted.
	- FixedLocator: Tick locations are fixed.
	- LinearLocator: Determine the tick locations.
	- MultipleLocator: Set a tick on every integer that is multiple of some base.
	- AutoLocator: Select no more than n intervals at nice locations.
	- LogLocator: Determine the tick locations for log axes.
- to use animation is matplotlib is to use one of the animation classes
	- Animation: A base class for Animations.
	- FuncAnimation: Makes an animation by repeatedly calling a function function
	- ArtistAnimation: Animation using a fixed set of Artist objects
	
	- from (https://matplotlib.org/stable/api/animation_api.html)