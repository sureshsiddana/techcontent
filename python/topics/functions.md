# Functions in Python

Functions are reusable blocks of code that perform a specific task.

```python
def greet(name):
    """This function greets the person passed in as a parameter."""
    print(f"Hello, {name}!")

greet("Alice")
```

**Key Points:**
- Use `def` to define a function.
- Use `return` to return a value from a function.
- Functions can have default, keyword, and variable-length arguments.

## Real-time Project Example
In an e-commerce app, you can use a function to calculate the total price:

```python
def calculate_total(price, quantity, tax=0.05):
    return price * quantity * (1 + tax)

total = calculate_total(100, 2)
print(f"Total: {total}")
```

## Interview Questions & Answers
**Q1: What are *args and **kwargs?**
A: *args allows a function to accept any number of positional arguments, while **kwargs allows it to accept any number of keyword arguments.

**Q2: What is a lambda function?**
A: A lambda function is an anonymous, single-expression function defined with the `lambda` keyword.

**Q3: Can you return multiple values from a function?**
A: Yes, by returning a tuple (e.g., `return a, b`).

## References
- [Python Functions - W3Schools](https://www.w3schools.com/python/python_functions.asp)
- [Defining Your Own Python Function - Real Python](https://realpython.com/defining-your-own-python-function/)
