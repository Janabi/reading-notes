# Hash Table

## Terminology 
- **_Hash_** is a way to convert a string into a encoded value that will make it much secure. For example, it commonly used in the determination of the index of array.
- **_Buckets_** is the index of array and it mainly contains a key/value if the collision occurs.
- **_Collision_** is a way where more than one key is getting hashed at the same location of the hashtable.

## Explanation
**Data would be include a key/value structure in the hash table. Therefore, once you would like to get the index or location of any key within an array by using the hash functionality. If another key has the same index of the previous key, then the collision will occur and the chaining will be linked between the two keys. So it is possible to have more than one keys at the same location or index of the array.**
**Hash implementation is so powerful and useful because it will take a small amount of space memroy as a big (O) notation.**

![Hash Table](https://he-s3.s3.amazonaws.com/media/uploads/2cabd32.jpg)

**As we can see in the image above, the key are unique and then we can get a value from the bucket array at their index or location. Also, we can noticed that the both keys 'Code Monk' and 'Hashing' are at the index 2 which also abviously they share the same value..**