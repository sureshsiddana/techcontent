# Generators in Python

Generators are iterators that yield items one at a time using the `yield` keyword.

```python
def count_up_to(n):
    count = 1
    while count <= n:
        yield count
        count += 1

for num in count_up_to(3):
    print(num)
```

**Key Points:**
- Use `yield` instead of `return` to create a generator.
- Generators are memory efficient for large data sets.

## Real-time Project Example
Reading large files line by line:

```python
def read_large_file(file_path):
    with open(file_path) as f:
        for line in f:
            yield line
```

## Interview Questions & Answers
**Q1: What is the difference between a generator and a normal function?**
A: A generator uses `yield` and returns an iterator, while a normal function uses `return` and returns a single value.

**Q2: How do you create a generator expression?**
A: Use parentheses: `(x*x for x in range(5))`.

**Q3: What are the advantages of generators?**
A: They are memory efficient and allow lazy evaluation of large data sets.

## References
- [Python Generators - Programiz](https://www.programiz.com/python-programming/generator)
- [Generators - Real Python](https://realpython.com/introduction-to-python-generators/)
