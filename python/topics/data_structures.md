# Basic Data Structures in Python

Python provides built-in and standard library data structures.

```python
# Stack using list
stack = []
stack.append(1)
stack.append(2)
print(stack.pop())  # 2

# Queue using collections.deque
from collections import deque
queue = deque([1, 2, 3])
queue.append(4)
print(queue.popleft())  # 1
```

**Key Points:**
- Use lists for stacks, `deque` for queues.
- Sets are for unique items.

## Real-time Project Example
Task scheduling with a queue:

```python
from collections import deque
tasks = deque(["task1", "task2"])
tasks.append("task3")
while tasks:
    print(f"Processing {tasks.popleft()}")
```

## Advanced Data Structures
### 1. Heap (Priority Queue)
Use `heapq` for efficient priority queues.

```python
import heapq
heap = []
heapq.heappush(heap, 3)
heapq.heappush(heap, 1)
heapq.heappush(heap, 2)
print(heapq.heappop(heap))  # 1
```

### 2. Linked List
Python does not have a built-in linked list, but you can implement one using classes.

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
```

### 3. Hash Table
Dictionaries in Python are implemented as hash tables.

### 4. Tree (Binary Tree Example)

```python
class TreeNode:
    def __init__(self, val):
        self.val = val
        self.left = None
        self.right = None
```

### 5. Graph (Adjacency List)

```python
graph = {
    'A': ['B', 'C'],
    'B': ['A', 'D'],
    'C': ['A', 'D'],
    'D': ['B', 'C']
}
```

## Interview Questions & Answers
**Q1: How do you implement a stack in Python?**
A: Use a list and its `append()` and `pop()` methods.

**Q2: How do you implement a queue in Python?**
A: Use `collections.deque` for efficient appends and pops from both ends.

**Q3: What is the difference between a set and a list?**
A: A set is unordered and contains only unique elements, while a list is ordered and can contain duplicates.

**Q4: How do you implement a priority queue in Python?**
A: Use the `heapq` module for a min-heap implementation.

**Q5: How would you detect a cycle in a linked list?**
A: Use Floyd’s Tortoise and Hare algorithm (two pointers).

**Q6: What is the time complexity of searching in a hash table?**
A: Average case is O(1), worst case is O(n).

## References
- [Python Data Structures - Programiz](https://www.programiz.com/python-programming/data-structure)
- [Data Structures - Real Python](https://realpython.com/python-data-structures/)
- [heapq — Heap queue algorithm - Python Docs](https://docs.python.org/3/library/heapq.html)
