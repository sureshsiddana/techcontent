# Working with JSON and CSV in Python

Python provides built-in modules for handling JSON and CSV data.

```python
import json
import csv

# JSON
person = {"name": "Alice", "age": 25}
json_str = json.dumps(person)
print(json_str)

# CSV
with open('data.csv', 'w', newline='') as f:
    writer = csv.writer(f)
    writer.writerow(['name', 'age'])
    writer.writerow(['Bob', 30])
```

**Key Points:**
- Use `json` for JSON data, `csv` for CSV files.
- Always handle file operations with `with`.

## Real-time Project Example
Reading user data from a CSV file:

```python
import csv
with open('users.csv') as f:
    reader = csv.DictReader(f)
    for row in reader:
        print(row['email'])
```

## Interview Questions & Answers
**Q1: How do you convert a Python dictionary to a JSON string?**  
A: Use `json.dumps(dictionary)`.

**Q2: How do you read a CSV file as a list of dictionaries?**  
A: Use `csv.DictReader(file)`.

**Q3: What is the difference between JSON and CSV?**  
A: JSON is used for hierarchical data, CSV is for tabular data.

## References
- [Python JSON - Programiz](https://www.programiz.com/python-programming/json)
- [Python CSV - Real Python](https://realpython.com/python-csv/)
