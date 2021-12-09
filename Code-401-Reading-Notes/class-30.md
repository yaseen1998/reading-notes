# class_30
### What is a Hashtable?
Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose.
<br>
### Why do we use them?
* Hold unique values
* Dictionary
* Library

### What Are they
The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.
<br>
<br>
the hash function takes a key and returns an integer. We use the integer to determine where the key/value pair should be placed in the array. The hash code is calculated in constant time and writing to an array at one index is O(1) so the hash map has O(1) access.
<br>
### Structure
#### Creating a Hash
A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a possible suggestion:

* Add or multiply all the ASCII values together.
* Multiply it by a prime number such as 599.
* Use modulo to get the remainder of the result, when divided by the total size of the array.
* Insert into the array at that index.

#### Collisions
A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. 
<br>
Collisions are solved by changing the initial state of the buckets. Instead of starting them all as null we can initialize a LinkedList in each one! Now if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list. 
<br>
<br>
**Hash maps do this to store values:**

* accept a key
* calculate the hash of the key
* use modulus to convert the hash into an array index
* store the key with the value by appending both to the end of a linked list


**Hash maps do this to read value:**

* accept a key
* calculate the hash of the key
* use modulus to convert the hash into an array index
* use the array index to access the short LinkedList representing a bucket
* search through the bucket looking for a node with a key/value pair

#### Internal Methods
**1-Add()**

* send the key to the GetHash method.
* Once you determine the index of where it should be placed, go to that index
* Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
* If something does exist, add the new key/value pair 

**2-Find()**:
The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, 
<br>
**3-Contains()**:
The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. 
<br>
**4-GETHash()**:
The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.
