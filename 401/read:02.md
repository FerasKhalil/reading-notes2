# Testing and Modules
### In Tests We Trust - TDD with Python
- **TDD** is short for **test driven development**
	- test name should start with "test_name.extension" it should start with the "test_"
- we should also consider the structure and the best one is **Arrange,Act,Assert** **"AAA"**
	- Arrange: is to organize the inputs
	- Act: execute the code being tested
	- Assert: make sure after testing that the result meets the output expectation

 
### If name equals main
- If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 
	- from (https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

### Recursion 
- Recursion is when a function calls itself either directly or indirectly