# Object-Oriented Programming (OOP) in Python

OOP is a programming paradigm based on objects and classes.

```python
class Dog:
    def __init__(self, name):
        self.name = name
    def bark(self):
        print(f"{self.name} says woof!")

my_dog = Dog("Buddy")
my_dog.bark()
```

**Key Points:**
- Supports inheritance, encapsulation, and polymorphism.
- Use `self` to access instance variables.

## Real-time Project Example
Modeling a bank account:

```python
class BankAccount:
    def __init__(self, owner, balance=0):
        self.owner = owner
        self.balance = balance
    def deposit(self, amount):
        self.balance += amount
    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
        else:
            print("Insufficient funds")
```

## Advanced OOP Topics
### 1. Multiple Inheritance
Python supports multiple inheritance, where a class can inherit from more than one parent class.

```python
class A:
    def foo(self):
        print("A")
class B:
    def foo(self):
        print("B")
class C(A, B):
    pass
c = C()
c.foo()  # Output: A (MRO applies)
```

### 2. Method Resolution Order (MRO)
Determines the order in which base classes are searched when executing a method.

### 3. Abstract Base Classes (ABC)
Use the `abc` module to define abstract classes and methods.

```python
from abc import ABC, abstractmethod
class Animal(ABC):
    @abstractmethod
    def speak(self):
        pass
```

### 4. Dunder (Magic) Methods
Special methods like `__str__`, `__repr__`, `__eq__`, `__add__` allow operator overloading and custom behavior.

```python
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    def __add__(self, other):
        return Point(self.x + other.x, self.y + other.y)
```

### 5. Composition vs Inheritance
Composition involves building classes using other classes as components, while inheritance derives new classes from existing ones.

## Advanced Interview Questions
**Q1: What is the diamond problem in multiple inheritance?**  
A: It occurs when two parent classes have a method with the same name, and a child class inherits from both. Python uses MRO to resolve this.

**Q2: How do you implement an interface in Python?**  
A: Use abstract base classes with abstract methods.

**Q3: What are dunder methods? Give examples.**  
A: Dunder (double underscore) methods are special methods like `__init__`, `__str__`, `__add__` that enable operator overloading and custom object behavior.

## References
- [Python OOP Advanced - Real Python](https://realpython.com/python3-object-oriented-programming/)
- [Abstract Base Classes - Python Docs](https://docs.python.org/3/library/abc.html)
