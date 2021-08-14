# Read: 13 - Local Storage
## HTML5 Storage
- is also called **web Storage**
- some call it local storage or DOM storage
	- link : http://diveinto.html5doctor.com/storage.html
- **HTML5 storage** is a way for wen pages to store named key/value
	pairs locally. like cookies and sessions
		- link:http://diveinto.html5doctor.com/storage.html
- this storage doesn't transmit data to the remote web server(like cookies)
- although it is possible to transmit it if wanted
- you store the data by naming a key, and retrieve it with that key
- the key is a string, but the data is any type that javascript supports
- the data is always stored as a string no matter what the type is it's called **caveat**
	- you'll have to use parseInt for an int
	- and parseFloat for a floating number
- you can set items, remove items or clear items
- HTML5 allows you to save your changes locally without losing your progress.