# Tutorial: Functions in Python

Functions are a way to group code that performs a specific task, making your code more modular and easier to read. 

The follow along the videos and the tutorials using the online Python editor https://www.online-python.com/.  

Videos: 
- Python Functions -  https://www.youtube.com/watch?v=eOEp5YrL6v0
- Functions and Parameters - https://www.youtube.com/watch?v=6SI2RZ1gTcA
- Functions and Return Values - https://www.youtube.com/watch?v=oS70q9nuL-E

Here's a tutorial on how to define and use functions in Python:

## Defining a Function
You define a function using the `def` keyword, followed by the function name and parentheses. Any arguments the function takes are placed within the parentheses.
```python
def greet(name):
    print("Hello, " + name + "!")
```

## Calling a Function
To call a function, simply write its name followed by parentheses, optionally passing in any required arguments.
```python
greet("Alice")  # Output: Hello, Alice!
greet("Bob")    # Output: Hello, Bob!
```

## Return Statement
Functions can return a value using the `return` statement. This allows you to use the result of a function call in other parts of your code.
```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

- [Activity: Function - Return Values](https://arcade.makecode.com/courses/csintro3/functions/returns)

## Default Arguments
You can provide default values for function arguments. If the caller doesn't specify a value for an argument, the default value is used.
```python
def greet(name="World"):
    print("Hello, " + name + "!")

greet()         # Output: Hello, World!
greet("Alice")  # Output: Hello, Alice!
```

## More Tutorial Resouces
Want to learn more?  Checkout the following with examples to work.
- https://www.w3schools.com/python/python_functions.asp
