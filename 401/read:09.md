# Read: Class 09  Game of Greed 4

## Dunder Methods
- dunder methods are special or magic methods that are predefined methods you can use
to enrich your classes.
- dunder methods are methods that start and end with double underscores
	- like __init__ or __str__
- '__init__' is the constructor in python
	- the constructor takes care of setting up the object 
	if the parameter of a contructor was = 0 or empty string etc.. it meanns it's an optional parameter
- '__repr__' : is the official string representation of an object.  this is how you would make an object of the class
	- the goal of __repr__ is to be unambiguous

- '__str__' : The “informal” or nicely printable string representation of an object.
	 This is for the enduser.
	-from (https://dbader.org/blog/python-dunder-methods)



- To iterate over transactions in reversed order you can implement the '__reversed__' special method:

	def __reversed__(self):
    	return self[::-1]

	>>> list(reversed(acc))
	[30, -20, 50, -10, 20]
- Operator Overloading for Merging Accounts: __add__
In Python, everything is an object. We are completely fine adding two integers or two strings with the + (plus) operator, it behaves in expected ways:

>>> 1 + 2
3

>>> 'hello' + ' world'
'hello world'

## Statistics - Probability
- probability is the answer of the question: "what is the chance of an even happening"
- if we use the random method we can calculate the probability of an example a toss coin.. what is the probability 
	of us getting heads or tails?