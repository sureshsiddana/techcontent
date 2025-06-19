# List Comprehensions in Python

List comprehensions provide a concise way to create lists.

```python
# Create a list of squares
squares = [x**2 for x in range(10)]
print(squares)

# Filter even numbers
evens = [x for x in range(10) if x % 2 == 0]
print(evens)
```

**Key Points:**
- More readable and concise than loops.
- Can include conditions.

## Real-time Project Example
Extracting names from a list of dictionaries:

```python
users = [{"name": "Alice"}, {"name": "Bob"}]
names = [user["name"] for user in users]
print(names)
```

## Interview Questions & Answers
**Q1: What is a list comprehension?**
A: A compact way to process all or part of the elements in a sequence and return a list with the results.

**Q2: Can you use if-else in a list comprehension?**
A: Yes, you can use conditional expressions inside list comprehensions.

**Q3: How do you create a dictionary comprehension?**
A: Use curly braces: `{k: v for k, v in iterable}`.

## References
- [List Comprehensions - Programiz](https://www.programiz.com/python-programming/list-comprehension)
- [List Comprehensions - Real Python](https://realpython.com/list-comprehensions-python/)
