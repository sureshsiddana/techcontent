# Context Managers in Python

Context managers handle setup and cleanup actions, commonly used with the `with` statement.

```python
with open('file.txt', 'r') as f:
    data = f.read()

# Custom context manager
class MyContext:
    def __enter__(self):
        print('Entering context')
        return self
    def __exit__(self, exc_type, exc_val, exc_tb):
        print('Exiting context')

with MyContext():
    print('Inside context')
```

**Key Points:**
- Use `__enter__` and `__exit__` methods for custom managers.
- Ensures resources are released properly.

## Real-time Project Example
Managing database connections:

```python
class DBConnection:
    def __enter__(self):
        print('Connect to DB')
        return self
    def __exit__(self, exc_type, exc_val, exc_tb):
        print('Disconnect from DB')

with DBConnection():
    print('Querying DB')
```

## Interview Questions & Answers
**Q1: What is a context manager?**
A: An object that defines the runtime context to be established when executing a `with` statement.

**Q2: How do you create a custom context manager?**
A: By defining `__enter__` and `__exit__` methods in a class or using the `contextlib` module.

**Q3: What is the advantage of using context managers?**
A: They ensure resources are properly managed and released, even if errors occur.

## References
- [Context Managers - Real Python](https://realpython.com/python-with-statement/)
- [Python Context Managers - Programiz](https://www.programiz.com/python-programming/context-manager)
