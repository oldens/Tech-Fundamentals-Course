# Lesson 10: Functions: Basics of Modularity

## Topics
- Definition (def)
- Parameters/arguments
- Return
- Scope

## Notes
Functions are a fundamental building block in Python programming. They allow you to encapsulate code into reusable blocks, making your programs more modular and easier to maintain.

### Definition (def)
In Python, you define a function using the `def` keyword followed by the function name and parentheses. The function body is indented.

Example:
```python
def greet():
    print("Hello, world!")
```

### Parameters/Arguments
Functions can accept parameters (also known as arguments) to make them more flexible. Parameters are specified within the parentheses in the function definition.

Example:
```python
def greet(name):
    print("Hello, " + name + "!")
```

### Return
Functions can return a value using the `return` keyword. This allows you to capture the result of a function and use it elsewhere in your program.

Example:
```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

### Scope
Scope refers to the visibility of variables within different parts of your program. Variables defined inside a function are local to that function and cannot be accessed outside of it.

Example:
```python
def my_function():
    x = 10  # Local variable
    print(x)

my_function()
print(x)  # This will raise an error because x is not defined outside the function
```

By understanding these basic concepts, you can start writing more modular and reusable code in Python.
