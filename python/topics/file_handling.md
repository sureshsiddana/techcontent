# File Handling in Python

Python makes it easy to read and write files.

```python
# Writing to a file
with open('output.txt', 'w') as f:
    f.write('Hello, file!')

# Reading from a file
with open('output.txt', 'r') as f:
    content = f.read()
    print(content)
```

**Key Points:**
- Always use `with` to handle files safely.
- Modes: 'r' (read), 'w' (write), 'a' (append), 'b' (binary).

## Real-time Project Example
Saving user logs to a file:

```python
user = 'alice'
with open('user_logs.txt', 'a') as log:
    log.write(f'{user} logged in\n')
```

## Interview Questions & Answers
**Q1: What is the difference between 'w' and 'a' modes in file handling?**
A: 'w' mode overwrites the file if it exists, while 'a' mode appends to the file.

**Q2: How do you read a file line by line in Python?**
A: Use a for loop: `for line in open('file.txt'): `

**Q3: What is the use of the 'with' statement in file handling?**
A: It ensures the file is properly closed after its suite finishes, even if an exception is raised.

## References
- [Python File Handling - W3Schools](https://www.w3schools.com/python/python_file_handling.asp)
- [Reading and Writing Files - Real Python](https://realpython.com/read-write-files-python/)
