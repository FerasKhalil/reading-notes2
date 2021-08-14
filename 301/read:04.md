# Read: Class 04 React and Forms

### React Docs - Forms

- What is a ‘Controlled Component’?
	- it's an input form element whose value is controlled by React
		from (https://reactjs.org/docs/forms.html)
- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
	- it will be updated as the user types. because we need to get the value from user

- How do we target what the user is entering if we have an event handler on an input field?
	- by resetting the value

### The Conditional (Ternary) Operator Explained

- Why would we use a ternary operator?
	- to have less lines of code

- Rewrite the following statement using a ternary statement:
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }

- x === y? console.log(true) : console.log(fals);