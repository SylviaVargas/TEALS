### Tutorial: Python Loops

Loops are used in Python to execute a block of code repeatedly. There are two main types of loops in Python: `while` and `for` loops.

#### While Loop
A `while` loop repeats a block of code as long as a specified condition is true.
```python
count = 0
while count < 5:
    print("Count is:", count)
    count += 1
```
Output:
```
Count is: 0
Count is: 1
Count is: 2
Count is: 3
Count is: 4
```

#### For Loop
A `for` loop iterates over a sequence (such as a list, tuple, string, or range) and executes the block of code for each item in the sequence.
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print("I love", fruit)
```
Output:
```
I love apple
I love banana
I love cherry
```

### Quiz: Python Loops

1. What is the output of the following `while` loop?
   ```python
   x = 0
   while x < 3:
       print("Hello")
       x += 1
   ```
   A) Hello  
   B) Hello Hello  
   C) Hello Hello Hello  
   D) Hello Hello Hello Hello

2. How many times will the `for` loop below execute?
   ```python
   for i in range(5):
       print("Iteration", i)
   ```
   A) 4  
   B) 5  
   C) 6  
   D) 7

3. What will be the output of the following code?
   ```python
   word = "Python"
   for letter in word:
       print(letter, end=" ")
   ```
   A) P y t h o n  
   B) Python  
   C) P, y, t, h, o, n  
   D) P, y, t, h, o, n,

### Python Assignment: Sum of Numbers

Write a Python program that calculates the sum of all numbers from 1 to 100 using a `for` loop.

### Answer Key:

1. C) Hello Hello Hello  
2. B) 5  
3. A) P y t h o n  