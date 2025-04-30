# Lesson 21: OOP in Python: Inheritance and Files

## Topics
- Inheritance
- super()
- Working with files
- Exception handling (try/except)

## Notes
Inheritance is a fundamental concept in object-oriented programming (OOP) that allows a class to inherit attributes and methods from another class. This promotes code reusability and hierarchical classification.

### Inheritance
Inheritance enables a new class (child class) to inherit attributes and methods from an existing class (parent class). The child class can also have its own attributes and methods. For example:

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        return f"{self.name} makes a sound."

class Dog(Animal):
    def speak(self):
        return f"{self.name} barks."

# Creating an object of the Dog class
my_dog = Dog("Buddy")
print(my_dog.speak())  # Output: Buddy barks.
```

### super()
The `super()` function is used to call a method from the parent class in the child class. It is commonly used to extend or modify the behavior of inherited methods. For example:

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        return f"{self.name} makes a sound."

class Dog(Animal):
    def __init__(self, name, breed):
        super().__init__(name)
        self.breed = breed

    def speak(self):
        return f"{self.name} barks."

# Creating an object of the Dog class
my_dog = Dog("Buddy", "Golden Retriever")
print(my_dog.speak())  # Output: Buddy barks.
```

### Working with Files
Python provides built-in functions to work with files, such as reading from and writing to files. The `open()` function is used to open a file, and the `with` statement ensures that the file is properly closed after its suite finishes. For example:

```python
# Writing to a file
with open("example.txt", "w") as file:
    file.write("Hello, world!")

# Reading from a file
with open("example.txt", "r") as file:
    content = file.read()
    print(content)  # Output: Hello, world!
```

### Exception Handling (try/except)
Exception handling is a mechanism to handle runtime errors in a program. The `try` block contains the code that may raise an exception, and the `except` block contains the code to handle the exception. For example:

```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Error: Division by zero is not allowed.")
```

By understanding inheritance, the `super()` function, working with files, and exception handling, we can create more robust and maintainable code in Python.
