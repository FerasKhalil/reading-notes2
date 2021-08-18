# Read: Class 19 Automation

### Python Regular Expressions Tutorial
- To  be able to use regular expressions in python you need to import it first by:
	- import re
- ordinary characters:
	- pattern = r"Cookie"
	 sequence = "Cookie"
	 if re.match(pattern, sequence):
    		 print("Match!")
	 else: print("Not a match!")
	- this will give us the output of Match!

- re.search(r'Co.k.e', 'Cookie').group()
	- output is 'Cookie'
#### Repetitions
- >>re.search(r'Co+kie', 'Cooookie').group()
	<< 'Cooookie'

- >> re.search(r'Ca*o*kie', 'Cookie').group()
<< 'Cookie'

- >>re.search(r'Colou?r', 'Color').group()
	<<'Color'

- >> re.search(r'\d{9,10}', '0987654321').group()
<< '0987654321'



-  ' . ' : A period. Matches any single character except the newline character.
- ' ^ ' A caret. Matches a pattern at the start of the string.
- ' [ ]' Matches the set of characters you specify within it.

- [source from](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)



### shutil
- Copying Files
	- copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.
- The copy() function interprets the output name like the Unix command line tool cp. If the named destination refers to a directory instead of a file, a new file is created in the directory using the base name of the source.
- copy2() works like copy(), but includes the access and modification times in the metadata copied to the new file.

- Copying File Metadata
	- By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

- To copy other metadata about the file use copystat().


- Working With Directory Trees
	- shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

- To remove a directory and its contents, use rmtree().

- To move a file or directory from one place to another, use move().

- Finding Files
	- The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

- File System Space
	- disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.
	- It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. 

- [click to go to soruce](https://pymotw.com/3/shutil/)