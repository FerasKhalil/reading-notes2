# Read: Class 07 Game of Greed 2.
### Python Scope
- scope means how the variables and names are looked up inside the code.
- 2 types of scopes:
	1. Global scope: 
	2. Local scope 


### LEGB rule
-LEGB is a shortcut for teh following words : " Local, Enclosing, Global, and Built-in."


- Local (or function) scope is the code block or body of any Python function or lambda expression. 
This Python scope contains the names that you define inside the function. These names will only be visible 
from the code of the function. It’s created at function call, not at function definition, so you’ll have as 
many different local scopes as function calls. This is true even if you call the same function multiple times, 
or recursively. Each call will result in a new local scope being created.

- Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an 
inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains 
the names that you define in the enclosing function. The names in the enclosing scope are visible from the 
code of the inner and enclosing functions.

- Global (or module) scope is the top-most scope in a Python program, script, or module. This Python scope contains all 
of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

- Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. 
This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. 
Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.


	- from (https://realpython.com/python-scope-legb-rule/)
- By default, parameters and names that you assign inside a function exist only within the function or local scope associated with the function call
	- from (https://realpython.com/python-scope-legb-rule/)


-example on nested functions: 
- >>> def outer_func():
...     # This block is the Local scope of outer_func()
...     var = 100  # A nonlocal var
...     # It's also the enclosing scope of inner_func()
...     def inner_func():
...         # This block is the Local scope of inner_func()
...         print(f"Printing var from inner_func(): {var}")
...
...     inner_func()
...     print(f"Printing var from outer_func(): {var}")
...
>>> outer_func()
Printing var from inner_func(): 100
Printing var from outer_func(): 100
>>> inner_func()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'inner_func' is not defined

 - https://realpython.com/python-scope-legb-rule/