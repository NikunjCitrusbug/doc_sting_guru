# Docstring Guide

This guide provides examples and best practices for writing docstrings in Python. Docstrings are essential for creating understandable and maintainable code, enabling others (and your future self) to understand the purpose and usage of your functions, classes, and modules.

## Table of Contents
- [General Guidelines](#general-guidelines)
- [Module Docstrings](#module-docstrings)
- [Class Docstrings](#class-docstrings)
- [Method and Function Docstrings](#method-and-function-docstrings)
- [Example Docstrings](#example-docstrings)
  - [Google Style](#google-style)

## General Guidelines
1. **Triple quotes**: Use triple double quotes (`"""`) for docstrings.
2. **Brief summary**: Start with a one-line summary that describes the object’s purpose.
3. **Detailed description**: Provide additional details if necessary, separated by a blank line from the summary.
4. **Parameters and Returns**: Document the parameters and return values, including types, in a consistent format.
5. **Consistency**: Follow the same style and format throughout your codebase.

## Module Docstrings
Each module should have a docstring at the top of the file that describes the module's purpose and contents.

```python
"""
This module provides utility functions for mathematical operations.

It includes functions for addition, subtraction, multiplication, and division.
"""
```

## Class Docstrings
Class docstrings should describe the purpose of the class and provide a brief overview of its methods and attributes.

```python
class Calculator:
    """
    A simple calculator class to perform basic arithmetic operations.

    Methods:
        add(a, b): Returns the sum of a and b.
        subtract(a, b): Returns the difference between a and b.
        multiply(a, b): Returns the product of a and b.
        divide(a, b): Returns the quotient of a and b.
    """
```

## Method and Function Docstrings
Method and function docstrings should describe the purpose of the method or function, its parameters, and its return value.

```python
def add(a, b):
    """
    Adds two numbers and returns the result.

    Args:
        a (int): The first number.
        b (int): The second number.

    Returns:
        int: The sum of a and b.
    """
    return a + b
```

## Example Docstrings

### Google Style
The Google style guide is a popular format for writing docstrings. Here are examples for functions and classes using this style.

**Function Example:**

```python
def multiply(a, b):
    """
    Multiplies two numbers and returns the result.

    Args:
        a (int): The first number.
        b (int): The second number.

    Returns:
        int: The product of a and b.
    """
    return a * b
```

**Class Example:**

```python
class Person:
    """
    Represents a person with a name and age.

    Attributes:
        name (str): The person's name.
        age (int): The person's age.
    """

    def __init__(self, name, age):
        """
        Initializes a new Person instance.

        Args:
            name (str): The person's name.
            age (int): The person's age.
        """
        self.name = name
        self.age = age

    def greet(self):
        """
        Greets the person with their name.

        Returns:
            str: A greeting message.
        """
        return f"Hello, my name is {self.name}."
```

## Conclusion
Following these guidelines will help ensure that your code is well-documented, making it easier to understand and maintain. Consistent and clear docstrings are a critical part of writing professional-level code.

For more detailed information on docstring conventions, refer to the [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html).
