# Advanced Python

This module covers advanced Python topics.

## Code Example

```python
def decorator_func(func):
    def wrapper():
        print("Before function")
        func()
        print("After function")
    return wrapper
```

## Concepts

- Decorators
- Generators
- Context Managers
