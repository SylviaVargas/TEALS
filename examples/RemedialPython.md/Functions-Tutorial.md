### Tutorial: Functions in Python

Functions are a way to group code that performs a specific task, making your code more modular and easier to read. Here's a tutorial on how to define and use functions in Python:

#### Defining a Function
You define a function using the `def` keyword, followed by the function name and parentheses. Any arguments the function takes are placed within the parentheses.
```python
def greet(name):
    print("Hello, " + name + "!")
```

#### Calling a Function
To call a function, simply write its name followed by parentheses, optionally passing in any required arguments.
```python
greet("Alice")  # Output: Hello, Alice!
greet("Bob")    # Output: Hello, Bob!
```

#### Return Statement
Functions can return a value using the `return` statement. This allows you to use the result of a function call in other parts of your code.
```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

- [Activity: Function - Return Values](https://arcade.makecode.com/courses/csintro3/functions/returns)

#### Default Arguments
You can provide default values for function arguments. If the caller doesn't specify a value for an argument, the default value is used.
```python
def greet(name="World"):
    print("Hello, " + name + "!")

greet()         # Output: Hello, World!
greet("Alice")  # Output: Hello, Alice!
```

### Quiz: Functions in Python

1. What keyword is used to define a function in Python?
   - A) func
   - B) define
   - C) def
   - D) function

2. How do you call a function named `my_function`?
   - A) call my_function()
   - B) my_function.call()
   - C) my_function()
   - D) call function my_function

3. What is the purpose of the return statement in a function?
   - A) It defines the function's name.
   - B) It calls another function.
   - C) It specifies the arguments of the function.
   - D) It specifies the value to be returned by the function.

4. Can a function in Python have multiple return statements?
   - A) Yes
   - B) No

5. What is the output of the following code?
   ```python
   def multiply(a, b):
       return a * b

   result = multiply(4, 5)
   print(result)
   ```
   - A) 20
   - B) 9
   - C) 45
   - D) 54

### Answers:
1. C) def
2. C) my_function()
3. D) It specifies the value to be returned by the function.
4. A) Yes
5. A) 20