# Read 30: Hash Tables
- Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.
- The main idea of hashtables is to store the key in data structure and quickly retrieve the value.
- A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.
- A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
- A hash code turns a key into an integer.
- A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
- A collision is what happens when more than one key gets hashed to the same location of the hashtable.
- Hash codes should never have randomness to them.
- The same key should always produce the same hash code.
- hash codes are deterministic: their output is determined only by their input. 
	- Source from (https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- Why we use them: 
	1. Hold unique values
	2. Dictionary
	3. Library


- Internal Methods:
1. Add()
	1. send the key to the GetHash method.
	2. Once you determine the index of where it should be placed, go to that index
	3. Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
	4. If something does exist, add the new key/value pair to the data structure within that bucket.
2. Find()
	- The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, 
	it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.


3. Contains()
- The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have 
	the contains call the GetHash and check the hashtable if the key exists in the table given the index returned.

4. GetHash()
- The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.
