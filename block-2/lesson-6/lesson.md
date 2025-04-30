# Lesson 6: Operators and Working with Strings

## Topics
- Arithmetic, comparison, logical operators
- Strings: indexing, slicing, methods, formatting

## Notes
Operators are special symbols in Python that perform operations on variables and values. Python supports various types of operators, including arithmetic, comparison, and logical operators.

### Arithmetic Operators
1. **Addition (+)**: Adds two operands.
2. **Subtraction (-)**: Subtracts the second operand from the first.
3. **Multiplication (*)**: Multiplies two operands.
4. **Division (/)**: Divides the first operand by the second.
5. **Modulus (%)**: Returns the remainder of the division.
6. **Exponentiation (**)**: Raises the first operand to the power of the second.
7. **Floor Division (//)**: Returns the largest integer less than or equal to the division result.

### Comparison Operators
1. **Equal (==)**: Checks if two operands are equal.
2. **Not Equal (!=)**: Checks if two operands are not equal.
3. **Greater Than (>)**: Checks if the first operand is greater than the second.
4. **Less Than (<)**: Checks if the first operand is less than the second.
5. **Greater Than or Equal To (>=)**: Checks if the first operand is greater than or equal to the second.
6. **Less Than or Equal To (<=)**: Checks if the first operand is less than or equal to the second.

### Logical Operators
1. **AND (and)**: Returns True if both operands are true.
2. **OR (or)**: Returns True if at least one of the operands is true.
3. **NOT (not)**: Returns True if the operand is false.

### Strings
Strings are sequences of characters enclosed in single or double quotes. Python provides various methods to work with strings.

#### Indexing
Indexing allows you to access individual characters in a string. The index starts from 0 for the first character and -1 for the last character.

#### Slicing
Slicing allows you to extract a substring from a string. It is done using the colon (:) operator. For example:
```python
s = "Hello, world!"
print(s[0:5])  # Output: Hello
```

#### Methods
Python provides several built-in methods to manipulate strings. Some common methods include:
1. **upper()**: Converts all characters in the string to uppercase.
2. **lower()**: Converts all characters in the string to lowercase.
3. **strip()**: Removes leading and trailing whitespace from the string.
4. **replace(old, new)**: Replaces all occurrences of the old substring with the new substring.
5. **split(delimiter)**: Splits the string into a list of substrings based on the specified delimiter.

#### Formatting
String formatting allows you to create formatted strings by embedding values within the string. Python supports various ways to format strings, including the `format()` method and f-strings.

Using the `format()` method:
```python
name = "Alice"
age = 25
print("My name is {} and I am {} years old.".format(name, age))
```

Using f-strings:
```python
name = "Alice"
age = 25
print(f"My name is {name} and I am {age} years old.")
```

By understanding and using these operators and string methods, you can perform various operations and manipulations on data in Python.
