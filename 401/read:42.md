# Read: Class 42 Pythonisms

## Dunder Methods
- Dunder methods are easy to indentify because they start and end with 2 underscores.
- Sometimes are called magic methods.
- Object Initialization: __init__

- Object Representation: __str__, __repr__
	1. __repr__: The “official” string representation of an object. This is how you would make an object of the class. The goal of __repr__ is to be unambiguous.
	2. __str__: The “informal” or nicely printable string representation of an object. This is for the enduser.

- Iteration: __len__, __getitem__, __reversed__

- Operator Overloading for Comparing Accounts: __eq__, __lt__

- Operator Overloading for Merging Accounts: __add__

- Callable Python Objects: __call__

- Context Manager Support and the With Statement: __enter__, __exit__

- Source from (https://dbader.org/blog/python-dunder-methods)

## Iterators
- __iter__ and __next__ dunder methods automatically work with for-in loops.


- Source from (https://dbader.org/blog/python-iterators)



## Generators
- Generator functions are syntactic sugar for writing objects that support the iterator protocol. 
- Generators abstract away much of the boilerplate code needed when writing class-based iterators.
- Generators start raising StopIteration exceptions after control flow leaves the generator function by any means other than a yield statement.
- The yield statement allows you to temporarily suspend execution of a generator function and to pass back values from it.
- yield is what makes a generator.
- yield is a keyword in python used to return from a function without destroying the states of its local variable, and when the function is called, the execution starts from the last yield statement.


- Source from (https://dbader.org/blog/python-generators)