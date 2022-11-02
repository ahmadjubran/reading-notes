# Hash Table

A hash table is an implementation of an associative array, a list of key-value pairs that allow you to retrieve a value via a key. Internally a hash table utilizes a hash function to transform a key value into an index that points to where the value is stored in memory.

    Hash tables have fast lookups, fast inserts, and fast deletes. They are commonly used to implement associative arrays, database indexes, caches, and sets.

The Hash table data structure stores elements in key-value pairs where

- **_Key_**- unique integer that is used for indexing the values
- **_Value_** - data that are associated with keys.

## Hashing

In a hash table, a new index is processed using the keys. The index is then used to store the value in the hash table. The process of generating an index from a key is called **hashing**.

### Hash Collision

When two keys are hashed to the same index, a collision occurs. There are two ways to handle collisions:

- **Separate Chaining** - each index of the array contains a reference to another data structure. This data structure is often a linked list, but it could be any data structure. When a new key is inserted, the key is hashed to an index and the key is added to the data structure at that index.

- **Open Addressing** - when a new key is inserted, the key is hashed to an index. If the index is empty, the key is inserted. If the index is occupied, a different index is found. There are several methods for finding a different index:

  - **_Linear Probing_** - find the next empty index in the array.
  - **_Quadratic Probing_** - find the next index by squaring the attempt number.
  - **_Double Hashing_** - use a second hash function to find the next index.

## Hash Table Implementation in JavaScript

- Using the **Object** Data Type

  The simplest way to implement a hash table is to use a JavaScript object. The keys are strings and the values can be any JavaScript data type.

  ```js
  let hash = new Object();
  hash["name"] = "Ahmad";
  hash["age"] = 24;
  hash["city"] = "Amman";
  ```

- Using a **Map** Object

  The Map object is a simple key/value map. Any value (both objects and primitive values) may be used as either a key or a value.

  ```js
  let hash = new Map();
  hash.set("name", "Ahmad");
  hash.set("age", 24);
  hash.set("city", "Amman");
  ```

## Applications of Hash Table

- constant time lookup and insertion is required
- cryptographic applications
- indexing data is required
