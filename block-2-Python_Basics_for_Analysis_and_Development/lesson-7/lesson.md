# Lesson 7: Program Logic: Conditions and Loops

## Topics
- Conditional constructs (if/elif/else)
- Loops while/for
- break/continue
- range()

## Notes
Program logic is the sequence of instructions that a computer follows to perform a specific task. In Python, conditional constructs and loops are used to control the flow of the program.

### Conditional Constructs (if/elif/else)
Conditional constructs allow you to execute different blocks of code based on certain conditions. The `if` statement is used to test a condition, and if the condition is true, the code block inside the `if` statement is executed. The `elif` (else if) statement is used to test additional conditions if the previous conditions are false. The `else` statement is used to execute a block of code if all the previous conditions are false.

Example:
```python
x = 10
if x > 0:
    print("x is positive")
elif x == 0:
    print("x is zero")
else:
    print("x is negative")
```

### Loops (while/for)
Loops are used to execute a block of code repeatedly as long as a certain condition is met. Python supports two types of loops: `while` loops and `for` loops.

#### while Loop
The `while` loop continues to execute a block of code as long as the condition is true.

Example:
```python
i = 1
while i <= 5:
    print(i)
    i += 1
```

#### for Loop
The `for` loop is used to iterate over a sequence (such as a list, tuple, or string) and execute a block of code for each item in the sequence.

Example:
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

### break/continue
The `break` statement is used to exit a loop prematurely, while the `continue` statement is used to skip the current iteration and continue with the next iteration of the loop.

Example:
```python
for i in range(1, 6):
    if i == 3:
        break
    print(i)
```

Example:
```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

### range()
The `range()` function is used to generate a sequence of numbers. It is commonly used in `for` loops to specify the number of iterations.

Example:
```python
for i in range(5):
    print(i)
```

By understanding and using conditional constructs and loops, you can control the flow of your Python programs and perform repetitive tasks efficiently.
