# read: Class 01 Readings: Introduction to React and Components
## Component Based Architecture
- it's basically a communication interface that has methods, events and properties.
- it abstracts and divides the problem to smaller problems 
- the main objective is to ensure component reusability
## component
- A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.
	from (https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)
What is a component?
	- a component is a software object it's main purpose is to interact with other components
- it has a defined interface

- a component has 3 views
	1. object-oriented view
	2. conventional view
	3. process-related view
What are the charactistics of a component?
	- a component is reusable, replaceable, not context specific, extensible, encapsulated and independent



What are the advantages of using component based architecture?
	- easy to deploy
	- reduced cost
	- reusable
	- modified the complexity
	- reliability
	- easy to change and update the implementation without affecting the rest of the system
		from (tutorialspoint.com/software_architecture_design/component_based_architecture.htm)
	-independent

## What is Props and How to Use it in React
What is props short for?
	- "props" is a short word for "properties" 
How are props used in React?
	1. define an attribute with a value
	2. pass to child components by using props
	3. render the props data
What is the flow of props?
	- flows make sure that you are using the component in the right way

## react
- react is a declarative, efficient, and flexible JavaScript library for building user interfaces. 
	It lets you compose complex UIs from small and isolated pieces of code called “components”.
		from (https://reactjs.org/tutorial/tutorial.html)
- an example of react code that prints "Hello, world"
	ReactDOM.render(
 	 <h1>Hello, world!</h1>,
  	document.getElementById('root')
	);

	from (https://reactjs.org/docs/hello-world.html)
- JSX is a syntax extension to JS 
	- it is mainly used with react to describe what the user interface should look like.
		from (https://reactjs.org/docs/introducing-jsx.html)
- an **"Element"** describes what you want to see on the screen.
	- react elements are plain objects, and are cheap to create.
		from (https://reactjs.org/docs/rendering-elements.html)
- can render elements and update the rendered elements
- **"Components"** let you split the user interface into independent reusable pieces. will make them smaller to 
	to be able to think about each piece alone and in isolation
- you can declare a component as a function or class.
- **props** are read  only
	- they dont chane the inputs and return the same result for the inputs
		from (https://reactjs.org/docs/components-and-props.html)



