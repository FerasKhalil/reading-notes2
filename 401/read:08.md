# Read: Class 08 Game of Greed 3

### List Comprehension
- the code we do like this: 
	new_list = []
	for i in old_list:
    		if filter(i):
        	new_list.append(expressions(i))
- from (https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
 with list comprehension it will look like this: 
	new_list = [expression(i) for i in old_list if filter(i)]
- we don't have to use an append method in this code!

- the list comprehension starts and ends with brackets '[' ']' 

- this is what it looks like: *result* = [*transform* *iteration* *filter* ]

- example: 
	x = [i for i in range(10)]
	print x

	# This will give the output:
	[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
	- from (https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

- can multiply items :
	list1 = [3,4,5]
 
	multiplied = [item*3 for item in list1] 
 
	print multiplied 
	[9,12,15]
	- from (https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
- code to show the first letter of each word in a list::
	listOfWords = ["this","is","a","list","of","words"]
	items = [ word[0] for word in listOfWords ]
	print items
	- from (https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

- code : squares = [x**2 for x in range(10)]
	- this code will print a list of squares for all numbers in range 10
	- output: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

	- from (https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)