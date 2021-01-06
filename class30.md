# summery 
## Hash Tables
![image](https://i.imgur.com/2ON8Kt5.jpg)
### Hash tables are used to implement map and set data structures in most common programming languages. Python have builtin dictionaries and maps. A hash table is an unordered collection of key-value pairs, where each key is unique.
## Hash Tables are used for:
1. Hold unique values
2. Dictionary
3. Library
## Creating a Hash
### A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a possible suggestion:

- Add or multiply all the ASCII values together.
- Multiply it by a prime number such as 599.
- Use modulo to get the remainder of the result, when divided by the total size of the array.
- Insert into the array at that index.
```
Key = "Cat"
Value = "Josie"
67 + 97 + 116 = 280
280 * 599 = 69648
69648 % 1024 = 16
Key gets placed in index of 16. 

```
##  information 
### Arrays actually have fast access. If we know the index of the information we want we can access that information in O(1) time. The reason why searching for a piece of data in a collection is O(N) isn’t because the array is slow, it’s just that we have to look through all N things in the collection.

### Hash maps take advantage of an array’s O(1) read access. Instead of adding elements to an array from beginning to end, a hash map uses a “hash function” to place each item at a precise index location, based off it’s key.

### Basically, the hash function takes a key and returns an integer. We use the integer to determine where the key/value pair should be placed in the array. The hash code is calculated in constant time and writing to an array at one index is O(1) so the hash map has O(1) access.

### The hash code is used again to read something from the hash map. Take the key, run it through the hash code to get a number, use that number to index the array. Calculating the hash code and reading an array at that index is all constant time to the hash map has O(1) read access!

