# Read: Class 05 Putting it all together

### React Docs - thinking in React

- How would you break a mock into a component heirarchy?
	- first thing is to draw boxes around every component (and subcomponent)
 	in the mock and give them all names - from (https://reactjs.org/docs/thinking-in-react.html)
	then use the single responsibility principle technique  for deciding if i should create a function or an object
	if the model was built correctly, the user interface will map nicely 
	- from (https://reactjs.org/docs/thinking-in-react.html)


- What is the single responsibility principle and how does it apply to components?
	- it's a technique for deciding if one should use a function or an object

- What does it mean to build a ‘static’ version of your application?
	- it renders the data model and the user interface and has no interactivity

- Once you have a static application, what do you need to add?
	- an inverse data flow

- What are the three questions you can ask to determine if something is state?
	1. Is it passed in from a parent via props? If so, it probably isn’t state.
	2. Does it remain unchanged over time? If so, it probably isn’t state.
	3. Can you compute it based on any other state or props in your component? If so, it isn’t state.
	- from (https://reactjs.org/docs/thinking-in-react.html)

- How can you identify where state needs to live?
	- Identify every component that renders something based on that state.
	- Find a common owner component (a single component above all the components that need the state in the hierarchy).
	- Either the common owner or another component higher up in the hierarchy should own the state.
	- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
	- from (https://reactjs.org/docs/thinking-in-react.html)


## Things I want to know more about 
- all of these. i want to see how it works and see someone building it infront of me so i can get the whole picture


