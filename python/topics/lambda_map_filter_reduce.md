# Lambda, Map, Filter, and Reduce in Python

These are functional programming tools for concise operations.

```python
# Lambda function
double = lambda x: x * 2
print(double(5))

# Map
nums = [1, 2, 3]
doubled = list(map(lambda x: x * 2, nums))
print(doubled)

# Filter
evens = list(filter(lambda x: x % 2 == 0, nums))
print(evens)

# Reduce
from functools import reduce
sum_all = reduce(lambda x, y: x + y, nums)
print(sum_all)
```

**Key Points:**
- Use `lambda` for small anonymous functions.
- `map`, `filter`, and `reduce` operate on iterables.

## Real-time Project Example
Calculating total price from a list of orders:

```python
orders = [100, 200, 300]
total = reduce(lambda x, y: x + y, orders)
print(total)
```

## Interview Questions & Answers
**Q1: What is a lambda function?**
A: An anonymous function defined with the `lambda` keyword.

**Q2: How do you use map, filter, and reduce?**
A: `map` applies a function to all items, `filter` selects items based on a condition, `reduce` applies a rolling computation.

**Q3: When would you use a lambda function?**
A: When you need a small, throwaway function for a short period, often as an argument to higher-order functions.

## References
- [Lambda, Map, Filter, Reduce - Programiz](https://www.programiz.com/python-programming/anonymous-function)
- [Functional Programming - Real Python](https://realpython.com/python-functional-programming/)
