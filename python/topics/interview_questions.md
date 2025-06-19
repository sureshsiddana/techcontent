# Real-time Python Interview Questions

This section contains real-time interview questions for freshers, covering both basic and advanced Python topics. Each question is designed to test practical knowledge and problem-solving skills.

## Sample Questions

1. **What is the difference between a list and a tuple in Python?**
2. **How do you handle exceptions in Python? Give an example.**
3. **Write a function to reverse a string in Python.**
4. **How do you remove duplicates from a list?**
5. **Explain the use of decorators with an example.**
6. **What is a lambda function? Where would you use it?**
7. **How do you read and write files in Python?**
8. **What is the purpose of the 'with' statement in file handling?**
9. **How do you implement a queue using collections.deque?**
10. **What is the Global Interpreter Lock (GIL)?**

## Real-time Project Example
Suppose you are asked to process a CSV file and extract unique email addresses:

```python
import csv

emails = set()
with open('users.csv', 'r') as file:
    reader = csv.DictReader(file)
    for row in reader:
        emails.add(row['email'])
print(emails)
```

## References
- [Top Python Interview Questions - GeeksforGeeks](https://www.geeksforgeeks.org/python-interview-questions/)
- [Python Interview Questions - Real Python](https://realpython.com/interview-questions-python/)
