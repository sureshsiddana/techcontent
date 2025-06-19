# Modules and Packages in Python

Modules are files containing Python code. Packages are collections of modules.

```python
# Importing a module
import math
print(math.sqrt(16))

# Creating a module (my_module.py)
def hello():
    print("Hello from module!")

# Importing from a package
from mypackage import mymodule
```

**Key Points:**
- Use `import` to include modules.
- Packages require an `__init__.py` file.

## Real-time Project Example
Organizing a project with multiple modules:

```
project/
    main.py
    utils/
        __init__.py
        file_ops.py
        math_ops.py
```

## Interview Questions & Answers
**Q1: How do you import a module from another directory?**
A: Use `sys.path.append('path_to_directory')` or install the package.

**Q2: What is the purpose of `__init__.py`?**
A: It marks a directory as a Python package and can execute initialization code for the package.

**Q3: How do you avoid name conflicts between modules?**
A: Use namespaces (packages) and import modules with aliases.

## References
- [Python Modules - W3Schools](https://www.w3schools.com/python/python_modules.asp)
- [Python Packages - Real Python](https://realpython.com/python-modules-packages/)
