# Regular Expressions (Regex) in Python

Regular expressions are used for pattern matching in strings.

```python
import re
pattern = r'\d+'
text = 'There are 24 apples and 42 oranges.'
result = re.findall(pattern, text)
print(result)  # ['24', '42']
```

**Key Points:**
- Use the `re` module for regex operations.
- Common methods: `search`, `match`, `findall`, `sub`.

## Real-time Project Example
Extracting email addresses from text:

```python
import re
text = 'Contact: alice@example.com, bob@test.org'
emails = re.findall(r'[\w\.-]+@[\w\.-]+', text)
print(emails)
```

## Interview Questions & Answers
**Q1: What is the purpose of the `re` module?**
A: It provides functions for working with regular expressions in Python.

**Q2: How do you match a pattern at the start of a string?**
A: Use `re.match()`.

**Q3: How do you replace all occurrences of a pattern?**
A: Use `re.sub(pattern, replacement, string)`.

## References
- [Python Regex - W3Schools](https://www.w3schools.com/python/python_regex.asp)
- [Regular Expressions - Real Python](https://realpython.com/regex-python/)
