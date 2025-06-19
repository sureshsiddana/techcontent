# String Manipulation in Python

Strings are sequences of characters. Python provides many methods for string manipulation.

```python
text = "Hello, World!"
print(text.lower())      # hello, world!
print(text.upper())      # HELLO, WORLD!
print(text.replace("World", "Python"))  # Hello, Python!
print(text[0:5])         # Hello
```

**Key Points:**
- Strings are immutable.
- Use slicing and built-in methods for manipulation.

## Real-time Project Example
Extracting domain names from email addresses:

```python
emails = ["alice@example.com", "bob@test.org"]
domains = [email.split('@')[1] for email in emails]
print(domains)  # ['example.com', 'test.org']
```

## Interview Questions & Answers
**Q1: How do you reverse a string in Python?**
A: Use slicing: `reversed_str = my_str[::-1]`.

**Q2: What is string immutability?**
A: Once created, a string cannot be changed. Any operation that modifies a string returns a new string.

**Q3: How do you check if a substring exists in a string?**
A: Use the `in` keyword: `'abc' in 'abcdef'` returns `True`.

## References
- [Python Strings - W3Schools](https://www.w3schools.com/python/python_strings.asp)
- [String Methods - Programiz](https://www.programiz.com/python-programming/methods/string)
