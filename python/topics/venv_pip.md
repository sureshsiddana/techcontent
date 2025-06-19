# Virtual Environments and pip in Python

Virtual environments isolate project dependencies. `pip` is the package installer for Python.

```bash
# Create a virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Install a package
pip install requests

# Freeze requirements
pip freeze > requirements.txt
```

**Key Points:**
- Use a virtual environment for every project.
- `requirements.txt` helps manage dependencies.

## Real-time Project Example
Setting up a project with dependencies:

```bash
python -m venv venv
venv\Scripts\activate
pip install flask
pip freeze > requirements.txt
```

## Interview Questions & Answers
**Q1: Why are virtual environments important?**  
A: They isolate dependencies for each project, preventing conflicts between packages.

**Q2: How do you install all dependencies from a requirements.txt file?**  
A: Use `pip install -r requirements.txt`.

**Q3: How do you upgrade a package using pip?**  
A: Use `pip install --upgrade package_name`.

## References
- [Python venv - Real Python](https://realpython.com/python-virtual-environments-a-primer/)
- [pip User Guide](https://pip.pypa.io/en/stable/user_guide/)
