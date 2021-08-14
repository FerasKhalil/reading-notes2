# Read: Class 04 
### Classes and Objects
- Objects are an encapsulation of variables and functions into a single entity. Objects get their variables
	 and functions from classes. Classes are essentially a template to create your objects.
		- from (https://www.learnpython.org/en/Classes_and_Objects)
- we can access variables that are in a class this way by creating a variable and assigning it a value of the <class name>()
	then we use <name of variable>.<name of class variable>
- we can also access functions just like we access variables (explained top)

### Thinking Recursively
- an iterative algorithm is when you do a task finish it then go to the next one.
- all recursive functions share a common structure which are:
	1. base case 2. recursive case
- each recursive case has its own execution context. so to maintain state during recursion we can either 
	1. Thread the state through each recursive call so that the current state is part of the current call’s execution context
	2. Keep the state in global scope
		-from (https://realpython.com/python-thinking-recursively/)
- List is not the only recursive data structure. Other examples include set, tree, dictionary, etc.
	-from (https://realpython.com/python-thinking-recursively/) 
- we can use the recursive function to calculate fibonacci number
	code : def fibonacci_recursive(n):
    print("Calculating F", "(", n, ")", sep="", end=", ")

    #### Base case
    if n == 0:
        return 0
    elif n == 1:
        return 1

    #### Recursive case
    else:
        return fibonacci_recursive(n-1) + fibonacci_recursive(n-2)

	- from (https://realpython.com/python-thinking-recursively/)