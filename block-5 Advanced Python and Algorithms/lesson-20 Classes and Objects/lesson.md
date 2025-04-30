# Lesson 20: OOP in Python: Classes and Objects

## Topics
- OOP concepts
- class
- __init__
- attributes
- methods

## Notes
Object-Oriented Programming (OOP) is a programming paradigm that uses objects and classes to structure and organize code. It allows for better code reusability, modularity, and maintainability.

### OOP Concepts
1. **Class**: A blueprint for creating objects. It defines a set of attributes and methods that the objects created from the class will have.
2. **Object**: An instance of a class. It represents a specific entity with its own set of attributes and methods.
3. **Attributes**: Variables that store the state or properties of an object.
4. **Methods**: Functions that define the behavior or actions of an object.

### Class
A class is defined using the `class` keyword followed by the class name. The class can have attributes and methods defined within it. For example:

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        return f"{self.name} is barking."

# Creating an object of the Dog class
my_dog = Dog("Buddy", 3)
print(my_dog.bark())  # Output: Buddy is barking.
```

### __init__
The `__init__` method is a special method in Python classes. It is called when an object is created from the class and allows the class to initialize the object's attributes. It is also known as the constructor method. For example:

```python
class Car:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year

    def get_info(self):
        return f"{self.year} {self.make} {self.model}"

# Creating an object of the Car class
my_car = Car("Toyota", "Camry", 2020)
print(my_car.get_info())  # Output: 2020 Toyota Camry
```

### Attributes
Attributes are variables that store the state or properties of an object. They are defined within the class and can be accessed using the `self` keyword. For example:

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def introduce(self):
        return f"Hi, my name is {self.name} and I am {self.age} years old."

# Creating an object of the Person class
person1 = Person("Alice", 25)
print(person1.introduce())  # Output: Hi, my name is Alice and I am 25 years old.
```

### Methods
Methods are functions that define the behavior or actions of an object. They are defined within the class and can be called on the object. For example:

```python
class Calculator:
    def add(self, a, b):
        return a + b

    def subtract(self, a, b):
        return a - b

# Creating an object of the Calculator class
calc = Calculator()
print(calc.add(5, 3))  # Output: 8
print(calc.subtract(5, 3))  # Output: 2
```

By understanding the concepts of classes, objects, attributes, and methods, we can effectively use OOP to create well-structured and maintainable code in Python.
