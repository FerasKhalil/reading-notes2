# Read: Class 10 In memory storage

### Understanding the JavaScript Call Stack
1. What is a ‘call’?
	- a data structure that uses the Last In, First Out (LIFO) principle to temporarily 
	 store and manage function invocation (call).
- from (https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

2. How many ‘calls’ can happen at once?
	- only one at a time

3. What does LIFO mean?
	- last in first out

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
	- function firstFunction(){
 	 console.log("Hello from firstFunction");
	}

	function secondFunction(){
 	 firstFunction();
	  console.log("The end from secondFunction");
	}

	secondFunction();
- from (https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

5. What causes a Stack Overflow?
	- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. 
	 The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.
- from (https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)


### JavaScript error messages 

1. What is a ‘refrence error’?
	- an object represents an error when a non-existent variable is referenced
- from (https://www.google.com/search?q=what+is+a+reference+error+in+javascript&oq=what+is+a+reference+error+in+&aqs=chrome.0.0i20i263j0j69i57j0i22i30l4.6916j0j7&sourceid=chrome&ie=UTF-8)

2. What is a ‘syntax error’?
	- An exception caused by the incorrect use of a pre-defined syntax
- from (https://www.google.com/search?q=what+is+a+syntax+error+in+javascript&sxsrf=ALeKk01jP8NQabDr-hVzSfMUVybhNf97OQ%3A1622050366207&ei=PoauYMn7C-iL9u8P28yTgAI&oq=what+is+a+syntax+error+in+javascr&gs_lcp=Cgdnd3Mtd2l6EAMYADICCAA6BAgjECc6BAgAEEM6BwgAEIcCEBQ6BQgAEMsBOgcIABBGEPkBOgUIABCRAjoGCAAQFhAeUInqAVjYlQJg6JwCaABwAngAgAHvBIgB6zGSAQwwLjI4LjEuMi4wLjKYAQCgAQGqAQdnd3Mtd2l6wAEB&sclient=gws-wiz)

3. What is a ‘range error’?
	- A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value. 
	 This can be encountered when: passing a value that is not one of the allowed string values to String
- from (https://www.google.com/search?q=what+is+a+range+error+in+javascript&sxsrf=ALeKk01aOgpludqEMY2VYHYxOsCYxs2oNg%3A1622050403729&ei=Y4auYOzhK6OFlQein5v4Cg&oq=what+is+a+range+error+in+javascript&gs_lcp=Cgdnd3Mtd2l6EAM6BwgAEEcQsANQwrsFWI7ABWCUwQVoAXACeACAAawBiAHOBZIBAzAuNZgBAKABAaoBB2d3cy13aXrIAQjAAQE&sclient=gws-wiz&ved=0ahUKEwisn_zQ8OfwAhWjQuUKHaLPBq8Q4dUDCA4&uact=5)

4. What is a ‘type error’?
	- Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, 
	 like accessing a property in an undefined type of variable.
- from (https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

5. What is a breakpoint?
	- At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values. After examining values, you can resume the execution
	  of code (typically with a play button)
- from (https://www.google.com/search?q=what+is+a+breakpoint+in+javascript&sxsrf=ALeKk03HQpeWCMhBbdWbdKapaN4o31ryiQ%3A1622050617514&ei=OYeuYO_VHq-D9u8P7I6QwAg&oq=what+is+a+breakpoint&gs_lcp=Cgdnd3Mtd2l6EAMYADIHCAAQhwIQFDICCAAyAggAMgIIADICCAAyAggAMgIIADICCAAyAggAMgIIADoECCMQJzoECAAQQzoCCC5Qg_MFWLCIBmCTkAZoAHABeACAAdACiAGvHpIBCDAuMTUuNS4xmAEAoAEBqgEHZ3dzLXdpesABAQ&sclient=gws-wiz)

6. What does the word ‘debugger’ do in your code?
	- The debugger statement stops the execution of JavaScript, and calls (if available) the debugging function. Using the debugger statement has
	  the same function as setting a breakpoint in the code.
- from (https://www.google.com/search?q=what+does+the+word+debugger+do+in+javascript&sxsrf=ALeKk02T1ptznUoHxg9IuZC6V0jQoycKPg%3A1622050719084&ei=n4euYK3RBIKA9u8P8ZWzqAQ&oq=what+does+the+word+debugger+do+in&gs_lcp=Cgdnd3Mtd2l6EAMYADIICCEQFhAdEB4yCAghEBYQHRAeOgQIIxAnOgUIABCRAjoCCAA6BAgAEEM6BQgAEMsBOgIILjoGCAAQFhAeOgkIABANEEYQ-QE6BggAEA0QHjoICAAQFhAKEB46BQghEKABUJ_qAljTlQNglZ4DaABwAngCgAHXAogB8C6SAQgwLjI2LjYuMpgBAKABAaoBB2d3cy13aXrAAQE&sclient=gws-wiz)# Read: Class 10 In memory storage

### Understanding the JavaScript Call Stack
1. What is a ‘call’?
	- a data structure that uses the Last In, First Out (LIFO) principle to temporarily 
	 store and manage function invocation (call).
- from (https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

2. How many ‘calls’ can happen at once?
	- only one at a time

3. What does LIFO mean?
	- last in first out

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
	- function firstFunction(){
 	 console.log("Hello from firstFunction");
	}

	function secondFunction(){
 	 firstFunction();
	  console.log("The end from secondFunction");
	}

	secondFunction();
- from (https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

5. What causes a Stack Overflow?
	- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. 
	 The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.
- from (https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)


### JavaScript error messages 

1. What is a ‘refrence error’?
	- an object represents an error when a non-existent variable is referenced
- from (https://www.google.com/search?q=what+is+a+reference+error+in+javascript&oq=what+is+a+reference+error+in+&aqs=chrome.0.0i20i263j0j69i57j0i22i30l4.6916j0j7&sourceid=chrome&ie=UTF-8)

2. What is a ‘syntax error’?
	- An exception caused by the incorrect use of a pre-defined syntax
- from (https://www.google.com/search?q=what+is+a+syntax+error+in+javascript&sxsrf=ALeKk01jP8NQabDr-hVzSfMUVybhNf97OQ%3A1622050366207&ei=PoauYMn7C-iL9u8P28yTgAI&oq=what+is+a+syntax+error+in+javascr&gs_lcp=Cgdnd3Mtd2l6EAMYADICCAA6BAgjECc6BAgAEEM6BwgAEIcCEBQ6BQgAEMsBOgcIABBGEPkBOgUIABCRAjoGCAAQFhAeUInqAVjYlQJg6JwCaABwAngAgAHvBIgB6zGSAQwwLjI4LjEuMi4wLjKYAQCgAQGqAQdnd3Mtd2l6wAEB&sclient=gws-wiz)

3. What is a ‘range error’?
	- A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value. 
	 This can be encountered when: passing a value that is not one of the allowed string values to String
- from (https://www.google.com/search?q=what+is+a+range+error+in+javascript&sxsrf=ALeKk01aOgpludqEMY2VYHYxOsCYxs2oNg%3A1622050403729&ei=Y4auYOzhK6OFlQein5v4Cg&oq=what+is+a+range+error+in+javascript&gs_lcp=Cgdnd3Mtd2l6EAM6BwgAEEcQsANQwrsFWI7ABWCUwQVoAXACeACAAawBiAHOBZIBAzAuNZgBAKABAaoBB2d3cy13aXrIAQjAAQE&sclient=gws-wiz&ved=0ahUKEwisn_zQ8OfwAhWjQuUKHaLPBq8Q4dUDCA4&uact=5)

4. What is a ‘type error’?
	- Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, 
	 like accessing a property in an undefined type of variable.
- from (https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

5. What is a breakpoint?
	- At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values. After examining values, you can resume the execution
	  of code (typically with a play button)
- from (https://www.google.com/search?q=what+is+a+breakpoint+in+javascript&sxsrf=ALeKk03HQpeWCMhBbdWbdKapaN4o31ryiQ%3A1622050617514&ei=OYeuYO_VHq-D9u8P7I6QwAg&oq=what+is+a+breakpoint&gs_lcp=Cgdnd3Mtd2l6EAMYADIHCAAQhwIQFDICCAAyAggAMgIIADICCAAyAggAMgIIADICCAAyAggAMgIIADoECCMQJzoECAAQQzoCCC5Qg_MFWLCIBmCTkAZoAHABeACAAdACiAGvHpIBCDAuMTUuNS4xmAEAoAEBqgEHZ3dzLXdpesABAQ&sclient=gws-wiz)

6. What does the word ‘debugger’ do in your code?
	- The debugger statement stops the execution of JavaScript, and calls (if available) the debugging function. Using the debugger statement has
	  the same function as setting a breakpoint in the code.
- from (https://www.google.com/search?q=what+does+the+word+debugger+do+in+javascript&sxsrf=ALeKk02T1ptznUoHxg9IuZC6V0jQoycKPg%3A1622050719084&ei=n4euYK3RBIKA9u8P8ZWzqAQ&oq=what+does+the+word+debugger+do+in&gs_lcp=Cgdnd3Mtd2l6EAMYADIICCEQFhAdEB4yCAghEBYQHRAeOgQIIxAnOgUIABCRAjoCCAA6BAgAEEM6BQgAEMsBOgIILjoGCAAQFhAeOgkIABANEEYQ-QE6BggAEA0QHjoICAAQFhAKEB46BQghEKABUJ_qAljTlQNglZ4DaABwAngCgAHXAogB8C6SAQgwLjI2LjYuMpgBAKABAaoBB2d3cy13aXrAAQE&sclient=gws-wiz)
## Things I want to know more about
- i want to know more about LIFO
- 





<!-- as;lfklfkdsfl;dsldf;lsdkfsl;kfdslkdfl;ks >