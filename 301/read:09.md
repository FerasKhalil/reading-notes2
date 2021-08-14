# Read: Class 09 FUNCTIONAL PROGRAMMING

### Functional Programming Concepts 
1. What is functional programming?
	- Functional programming is a programming paradigm — a style of building the structure and 
	 elements of computer programs — that treats computation as the evaluation of mathematical functions 
	 and avoids changing-state and mutable data
	- from (https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

2. What is a pure function and how do we know if something is a pure function?
	-  functions that accept an input and returns a value without modifying any data outside its scope 
	- from (https://www.google.com/search?q=what+is+a+pure+function+in+javascript&oq=what+is+a+pure+function+in+java&aqs=chrome.0.0i20i263j0j0i22i30l3.9163j0j7&sourceid=chrome&ie=UTF-8)
	- 2 ways to know if a function is pure 
	1. It returns the same result if given the same arguments (it is also referred as deterministic)
	2. It does not cause any observable side effects

3. What are the benefits of a pure function?
	- The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts

4. What is immutability?
	- Unchanging over time or unable to be changed.
	- from (https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

5. What is Referential transparency?
	- Basically, if a function consistently yields the same result for the same input, it is referentially transparent
	- from (https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)



### Node JS Tutorial for Beginners #6 - Modules and require()

1. What is a module?
	- a javascript file

2. What does the word ‘require’ do?
	- it is similar to import in react

3. How do we bring another module into the file the we are working in?
	- at first at has to be available
	- after doing require with the file name that   has the module in it

4. What do we have to do to make a module available?
	- module.exports = 'function name' ;




## Things I want to know more about
- i want to learn more about Node JS it looks interesting