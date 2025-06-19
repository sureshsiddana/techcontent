# Decorators in Python

Decorators are functions that modify the behavior of other functions.

```python
def my_decorator(func):
    def wrapper():
        print("Before function call")
        func()
        print("After function call")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
```

**Key Points:**
- Use `@decorator_name` syntax.
- Useful for logging, authentication, etc.

## Real-time Project Example
Logging function calls in a web app:

```python
def log_access(func):
    def wrapper(*args, **kwargs):
        print(f"Accessing {func.__name__}")
        return func(*args, **kwargs)
    return wrapper

@log_access
def get_user():
    print("User data")

get_user()
```

## Interview Questions & Answers
**Q1: What is a decorator in Python?**  
A: A decorator is a function that takes another function and extends its behavior without explicitly modifying it.

**Q2: How do you write a decorator that accepts arguments?**  
A: Use an extra wrapper function to accept arguments and return the actual decorator.

**Q3: What are some common use cases for decorators?**  
A: Logging, access control, memoization, and timing functions.

## References
- [Python Decorators - Real Python](https://realpython.com/primer-on-python-decorators/)
- [Decorators - Programiz](https://www.programiz.com/python-programming/decorator)
