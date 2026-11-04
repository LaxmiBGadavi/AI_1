# Day 010 – Python Functions and Classes for Agentic AI

## Concepts Learned

### 1. Python Functions
- Defining functions
- Function parameters and arguments
- Return statements
- Reusable functions
- Default arguments

### 2. *args
- Passing multiple positional arguments
- Handling variable-length arguments
- Using `*args` inside functions

Example:
```python
def add_numbers(*args):
    return sum(args)

print(add_numbers(10, 20, 30))
```

### 3. **kwargs
- Passing multiple keyword arguments
- Handling variable-length keyword arguments
- Working with key-value pairs

Example:
```python
def student_details(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

student_details(name="Laxmi", skill="Python")
```

### 4. Python Classes and Objects
- Understanding classes
- Creating objects
- Class attributes
- Instance attributes
- Constructor using `__init__()`
- Instance methods

Example:
```python
class Agent:
    def __init__(self, name, role):
        self.name = name
        self.role = role

    def display(self):
        print(f"Agent: {self.name}, Role: {self.role}")

agent = Agent("AI Assistant", "Research")
agent.display()
```

### 5. Dataclasses
- Introduction to dataclasses
- Using the `@dataclass` decorator
- Automatically generating constructors
- Storing structured data

Example:
```python
from dataclasses import dataclass

@dataclass
class User:
    name: str
    age: int

user = User("Laxmi", 22)
print(user)
```

### 6. Type Hints
- Understanding type annotations
- Specifying parameter types
- Specifying return types
- Improving code readability

Example:
```python
def calculate_sum(a: int, b: int) -> int:
    return a + b

print(calculate_sum(10, 20))
```

## Connection to Agentic AI

These Python concepts are useful for:
- Creating reusable AI agent functions.
- Passing flexible inputs to functions.
- Structuring agent classes.
- Managing structured agent data.
- Improving code readability and maintainability.
- Defining input and output types for agent workflows.

## Learning Outcome

Learned Python functions, `*args`, `**kwargs`, classes, objects, dataclasses and type hints as foundations for developing structured and reusable Agentic AI applications.

