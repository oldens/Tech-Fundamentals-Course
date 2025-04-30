# Lesson 9: Data Collections: Dictionaries and Sets

## Topics
- Dictionaries: key-value pairs, methods
- Sets: unique elements, operations

## Notes
Dictionaries and sets are essential data structures in Python that allow for efficient data storage and manipulation.

### Dictionaries
Dictionaries are collections of key-value pairs, where each key is unique. They are useful for storing and retrieving data based on a unique identifier.

#### Creating a Dictionary
```python
my_dict = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}
```

#### Accessing Values
You can access the values in a dictionary using their keys:
```python
print(my_dict["name"])  # Output: Alice
```

#### Adding and Updating Entries
You can add new key-value pairs or update existing ones:
```python
my_dict["email"] = "alice@example.com"
my_dict["age"] = 26
```

#### Removing Entries
You can remove key-value pairs using the `del` keyword or the `pop()` method:
```python
del my_dict["city"]
email = my_dict.pop("email")
```

#### Dictionary Methods
Dictionaries have several useful methods, such as `keys()`, `values()`, and `items()`:
```python
print(my_dict.keys())    # Output: dict_keys(['name', 'age'])
print(my_dict.values())  # Output: dict_values(['Alice', 26])
print(my_dict.items())   # Output: dict_items([('name', 'Alice'), ('age', 26)])
```

### Sets
Sets are collections of unique elements. They are useful for storing items without duplicates and performing set operations.

#### Creating a Set
You can create a set using curly braces or the `set()` function:
```python
my_set = {1, 2, 3, 4, 5}
another_set = set([3, 4, 5, 6, 7])
```

#### Adding and Removing Elements
You can add elements to a set using the `add()` method and remove elements using the `remove()` or `discard()` methods:
```python
my_set.add(6)
my_set.remove(1)
my_set.discard(2)
```

#### Set Operations
Sets support various operations, such as union, intersection, and difference:
```python
union_set = my_set.union(another_set)
intersection_set = my_set.intersection(another_set)
difference_set = my_set.difference(another_set)
```

By understanding dictionaries and sets, you can efficiently store and manipulate data in your Python programs.
