[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15305403&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python: High-level, interpreted language known for readability and versatility.

## Key Features:

- Readable syntax
- Interpreted
- Dynamic typing
- Extensive libraries
- Cross-platform
- Strong community

** Use Cases: Web development (Django), data science (Pandas), automation, machine learning (TensorFlow).

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

## Windows:

- Download from python.org.
- Run installer, check "Add Python to PATH," and follow instructions.

## Verify Installation:
python --version
## Virtual Environment:
python -m venv myenv
source myenv/bin/activate  # On Windows: myenv\Scripts\activate

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")
'print' outputs text to console; "Hello, World!" is a string.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

- Basic Data Types: 'int', 'float', 'str', 'bool'
## Example script

age = 25             # int
height = 5.9         # float
name = "Alice"       # str
is_student = True    # bool

print(age, height, name, is_student)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

## Conditional statement:

x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is 5 or less")

## loop

for i in range(5):
    print(i)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions: Reusable blocks of code.

Example Function:

def add(a, b):
    return a + b

result = add(3, 5)
print(result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Lists: Ordered collections.
Dictionaries: Key-value pairs.

Example Script:

numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers)

person = {"name": "Alice", "age": 25}
person["city"] = "New York"
print(person)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.


## Example

try:
    x = 1 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("Execution completed")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.


## Importing a module:

import math
print(math.sqrt(16))

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

## Reading from a file:

with open('file.txt', 'r') as file:
    content = file.read()
    print(content)

## Writing to a file:

lines = ["First line", "Second line", "Third line"]
with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")
