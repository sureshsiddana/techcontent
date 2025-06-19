# Lists, Tuples, and Dictionaries in Python

These are built-in data structures for storing collections of items.

```python
# List
fruits = ["apple", "banana", "cherry"]
# Tuple
coordinates = (10.0, 20.0)
# Dictionary
student = {"name": "Alice", "age": 22}
```

**Key Points:**
- Lists are mutable, tuples are immutable, dictionaries store key-value pairs.
- Use list comprehensions for concise list creation.

## Real-time Project Example
In a contact management app, you can use a dictionary to store contact details:

```python
contact = {"name": "Bob", "phone": "123-456-7890"}
contacts = [contact]
```

## Interview Questions & Answers
**Q1: What is the difference between a list and a tuple?**  
A: Lists are mutable (can be changed), while tuples are immutable (cannot be changed).

**Q2: How do you remove duplicates from a list?**  
A: Convert the list to a set and back to a list: `list(set(my_list))`.

**Q3: How do you access values in a dictionary?**  
A: Use the key inside square brackets or the `get()` method: `student['name']` or `student.get('name')`.


## References
- [Python Lists - Programiz](https://www.programiz.com/python-programming/list)
- [Python Dictionaries - Real Python](https://realpython.com/python-dicts/)
