### Tutorial: Python Variables

Variables in Python are used to store data values. Unlike other programming languages, Python has no command for declaring a variable. A variable is created the moment you first assign a value to it. Here are some examples of using variables in Python:

#### 1. Assigning a value to a variable
```python
x = 5
y = "Hello, World!"
```

#### 2. Printing the value of a variable
```python
print(x)  # Output: 5
print(y)  # Output: Hello, World!
```

#### 3. Changing the value of a variable
```python
x = 10
print(x)  # Output: 10
```

#### 4. Variable naming rules
- Variable names are case-sensitive (`age`, `Age`, and `AGE` are three different variables).
- Variable names must start with a letter or an underscore (`_`), and can only contain letters, numbers, and underscores.
- Variable names cannot start with a number.

#### 5. Assigning multiple variables
```python
a, b, c = 1, 2, 3
print(a)  # Output: 1
print(b)  # Output: 2
print(c)  # Output: 3
```

#### 6. Global vs. local variables
- Global variables are declared outside of functions and can be accessed by any function.
- Local variables are declared inside functions and can only be accessed within those functions.

#### 7. Using global keyword to modify a global variable inside a function
```python
x = 5

def my_func():
    global x
    x = 10

my_func()
print(x)  # Output: 10
```

#### 8. Deleting a variable
```python
x = 5
del x
print(x)  # This will raise an error because x is no longer defined
```

#### 9. Type casting
```python
x = "10"
y = int(x)
print(y)  # Output: 10
```

#### 10. Variable scope
Variables in Python have either local or global scope. A local variable is defined inside a function and can only be accessed within that function. A global variable is defined outside of any function and can be accessed by any function.

### Quiz: Python Variables

1. What is the output of the following code?
   ```python
   x = 5
   print("x is", x)
   ```
   A) x is 5  
   B) 5  
   C) x is  
   D) Syntax error

2. Which of the following is a valid variable name in Python?
   A) my_variable  
   B) 123variable  
   C) my variable  
   D) _my_variable

3. What is the output of the following code?
   ```python
   a = 5
   b = 3
   a, b = b, a
   print(a, b)
   ```
   A) 5 3  
   B) 3 5  
   C) 3 3  
   D) 5 5

### Python Assignment: Swap Variables

Write a Python program that takes two variables and swaps their values without using a temporary variable.

### Answer Key:

1. A) x is 5  
2. A) my_variable  
3. B) 3 5