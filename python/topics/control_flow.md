# Control Flow in Python

Control flow statements manage the order in which code executes.

```python
# if-elif-else
score = 85
if score >= 90:
    print("Excellent")
elif score >= 60:
    print("Pass")
else:
    print("Fail")

# for loop
for i in range(3):
    print(i)

# while loop
count = 0
while count < 3:
    print(count)
    count += 1
```

**Key Points:**
- Use indentation to define code blocks.
- Use break, continue, and pass for loop control.

## Real-time Project Example
In a login system, you can use control flow to validate user credentials:

```python
username = input("Enter username: ")
if username == "admin":
    print("Access granted")
else:
    print("Access denied")
```

## Advanced Control Flow Topics
### 1. Comprehensions with Conditionals
List, set, and dictionary comprehensions can include if/else logic.

```python
nums = [1, 2, 3, 4, 5]
even_or_odd = ["even" if x % 2 == 0 else "odd" for x in nums]
```

### 2. Exception Handling in Control Flow
Combine try/except with control flow for robust programs.

```python
try:
    x = int(input("Enter a number: "))
    print(10 / x)
except ZeroDivisionError:
    print("Cannot divide by zero!")
```

### 3. Loop Else Clause
The else block after a loop runs only if the loop wasn't terminated by break.

```python
for n in range(2, 10):
    for x in range(2, n):
        if n % x == 0:
            break
    else:
        print(f"{n} is a prime number")
```

### 4. Pattern Matching (Python 3.10+)
Use match-case for structural pattern matching.

```python
value = 42
match value:
    case 1:
        print("One")
    case 42:
        print("The answer")
    case _:
        print("Something else")
```

## Interview Questions & Answers
**Q1: What is the difference between 'break' and 'continue'?**
A: 'break' exits the nearest enclosing loop, while 'continue' skips the rest of the current loop iteration and continues with the next iteration.

**Q2: How does the 'else' clause work with loops in Python?**
A: The 'else' block after a loop executes only if the loop completes normally (not terminated by 'break').

**Q3: What is the use of 'pass' statement?**
A: 'pass' is a null operation; it is used as a placeholder when a statement is syntactically required but no action is needed.

**Q4: What is pattern matching in Python?**
A: Pattern matching (match-case) is a feature introduced in Python 3.10 for matching data structures against patterns.

**Q5: How do you handle exceptions inside loops?**
A: Use try/except blocks inside the loop to handle errors for each iteration.

## References
- [Python Control Flow - Real Python](https://realpython.com/python-conditional-statements/)
- [Pattern Matching - Python Docs](https://docs.python.org/3/reference/compound_stmts.html#the-match-statement)
