# Type Annotations in Python 3

This repository provides an overview of type annotations in Python 3 and how they can be used to specify function signatures and variable types. It also covers the concept of duck typing and introduces mypy, a static type checker for Python.

## Table of Contents

- [What are Type Annotations?](#what-are-type-annotations)
- [Using Type Annotations for Functions and Variables](#using-type-annotations-for-functions-and-variables)
- [Duck Typing](#duck-typing)
- [Validating Code with mypy](#validating-code-with-mypy)
- [Conclusion](#conclusion)

## What are Type Annotations?

Type annotations in Python are a way to add explicit type hints to your code. They allow you to specify the expected types of function parameters, return values, and variables. While Python is a dynamically typed language, type annotations provide a way to add static typing-like behavior to your code, enabling better code understanding, documentation, and tooling support.

Type annotations are optional and do not affect the runtime behavior of the code. They are primarily used for documentation purposes and can be ignored by the interpreter. However, they can be leveraged by tools like mypy for static type checking.

## Using Type Annotations for Functions and Variables

To specify type annotations, you can use the `->` syntax to indicate the expected return type of a function. For example:

```python
def add_numbers(a: int, b: int) -> int:
    return a + b
```

In this example, `a` and `b` are annotated as integers (`int`), and the return type of the function is also specified as an integer.

You can also annotate variables using the colon (`:`) syntax:

```python
age: int = 25
```

Here, the `age` variable is annotated as an integer with an initial value of `25`.

Type annotations support a wide range of types, including built-in types (e.g., `str`, `int`, `float`, `bool`), collections (e.g., `list`, `tuple`, `dict`), user-defined classes, and more.

## Duck Typing

Python follows the principle of "duck typing," which means that the type of an object is determined by its behavior rather than its explicit type. Duck typing allows you to focus on the object's behavior and capabilities rather than its specific type.

Type annotations do not impose strict type checks during runtime but can be used as hints for static type checkers like mypy. Duck typing remains a fundamental concept in Python, allowing flexibility and easy interoperability.

## Validating Code with mypy

[mypy](https://mypy-lang.org/) is a static type checker for Python that uses type annotations to detect and report type errors. It analyzes the code statically and provides feedback on potential type-related issues, helping to catch errors before runtime.

To use mypy, you can install it using `pip`:

```bash
pip install mypy
```

Once installed, you can run mypy on your Python code by executing:

```bash
mypy your_code.py
```

Mypy will analyze the code, check for type inconsistencies, and display any detected errors or warnings.

## Conclusion

Type annotations in Python 3 allow you to add explicit type hints to your code for better code understanding and documentation. While they are optional and do not affect runtime behavior, they can be used by tools like mypy to perform static type checking and catch potential errors.

This repository provides an introduction to type annotations, how to use them for functions and variables, and the concept of duck typing. It also highlights the usage of mypy for validating code and catching type-related issues.

Feel free to explore
