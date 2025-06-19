# Exception Handling in Python

Exception handling lets you manage errors gracefully.

```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error: {e}")
finally:
    print("This runs no matter what.")
```

**Key Points:**
- Use `try`, `except`, `finally`, and `else` blocks.
- Catch specific exceptions for better error handling.

## Real-time Project Example
Handling file not found errors:

```python
try:
    with open('data.txt') as f:
        data = f.read()
except FileNotFoundError:
    print("File not found!")
```

## Interview Questions & Answers
**Q1: What is the difference between 'except Exception' and 'except'?**
A: 'except Exception' catches most built-in exceptions, while a bare 'except' catches all exceptions, including system-exiting ones (not recommended).

**Q2: How do you raise a custom exception?**
A: Use the `raise` statement with an exception class: `raise ValueError('message')`.

**Q3: What is the purpose of the 'finally' block?**
A: Code in the 'finally' block always runs, regardless of whether an exception was raised.

## References
- [Python Exceptions - Programiz](https://www.programiz.com/python-programming/exception-handling)
- [Python Exception Handling - Real Python](https://realpython.com/python-exceptions/)
