### Tutorial: Python Variables

Variables in Python are used to store data values. Unlike other programming languages, Python has no command for declaring a variable. A variable is created the moment you first assign a value to it. 

The following tutorials should be completed using the online Python editor https://www.online-python.com/.  
Follow the tutorial below and save the link to solution in Google Classroom for review and grading.

Here are some examples of using variables in Python:

#### 1. Assigning a value to a variable
```python
# 1 - Assigning a variable
x = 5
y = "Hello, World!"
```

#### 2. Printing the value of a variable
```python
# 2 - Printing the value of a variable
print(x)  # Output: 5
print(y)  # Output: Hello, World!
```

#### 3. Changing the value of a variable
```python
# 3 - Changing the values of a variable
x = 10
print(x)  # Output: 10
```

#### 4. Variable naming rules
- Variable names are case-sensitive (`age`, `Age`, and `AGE` are three different variables).
- Variable names must start with a letter or an underscore (`_`), and can only contain letters, numbers, and underscores.
- Variable names cannot start with a number.

```python
# 4 - Variable naming rules
age = 10
Age = 20 
AGE = 30 
print(age)  # Output: 1
print(Age)  # Output: 2
print(AGE)  # Output: 3
```

#### 5. Assigning multiple variables
```python
# 5 - Assigning multiple variables
a, b, c = 1, 2, 3
print(a)  # Output: 1
print(b)  # Output: 2
print(c)  # Output: 3
```

#### 6. Global vs. local variables
Variables in Python have either local or global scope. A local variable is defined inside a function and can only be accessed within that function. A global variable is defined outside of any function and can be accessed by any function.
- Global variables are declared outside of functions and can be accessed by any function.
- Local variables are declared inside functions and can only be accessed within those functions.

#### 7. Using global keyword to modify a global variable inside a function
```python
#  7 - Using a global variables
x = 5

def my_func():
    global x
    x = 10

my_func()
print(x)  # Output: 10
```

#### 8. Deleting a variable
```python
#  8 - Deleting a variable
x = 5
del x
print(x)  # This will raise an error because x is no longer defined
```

#### 9. Type casting
Casting in python is done using constructor functions:

- int() - constructs an integer number from an integer literal, a float literal (by removing all decimals), or a string literal (providing the string represents a whole number)
- float() - constructs a float number from an integer literal, a float literal or a string literal (providing the string represents a float or an integer)
- str() - constructs a string from a wide variety of data types, including strings, integer literals and float literals
```python
#  9 - Type Casting
x = "10"
y = int(x)
print(y)  # Output: 10
```



### 10 Python Assignment: Swap Variables

Write a Python program that takes two variables and swaps their values without using a temporary variable.