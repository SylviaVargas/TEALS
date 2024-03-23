### Tutorial: Python Lists and Arrays

In Python, a list is a collection of items that are ordered and mutable. An array is a data structure that stores a collection of items, but unlike lists, arrays can only store items of the same data type.

#### Creating Lists and Arrays
You can create a list in Python by enclosing items in square brackets `[]`. Arrays are not built-in data structures in Python and need to be imported from the `array` module.
```python
# Creating a list
my_list = [1, 2, 3, 4, 5]

# Creating an array
from array import array
my_array = array('i', [1, 2, 3, 4, 5])  # 'i' specifies the data type of the array (integer)
```

#### Accessing Elements
You can access elements in a list or array using their index.
```python
print(my_list[0])     # Output: 1
print(my_array[1])    # Output: 2
```

#### Modifying Elements
You can change the value of a specific element in a list or array by accessing it using its index.
```python
my_list[2] = 10
print(my_list)    # Output: [1, 2, 10, 4, 5]

my_array[3] = 15
print(my_array)   # Output: array('i', [1, 2, 3, 15, 5])
```

### Examples:
1. Find the sum of all elements in a list.
   ```python
   numbers = [1, 2, 3, 4, 5]
   total = sum(numbers)
   print(total)   # Output: 15
   ```

2. Convert a list to an array.
   ```python
   from array import array
   numbers = [1, 2, 3, 4, 5]
   my_array = array('i', numbers)
   print(my_array)   # Output: array('i', [1, 2, 3, 4, 5])
   ```
## More Reading
   - https://www.freecodecamp.org/news/how-to-use-lists-in-python/
   
### Quiz: Python Lists and Arrays

1. What is the correct way to access the third element of a list named `my_list`?
   A) my_list[2]  
   B) my_list[3]  
   C) my_list[4]  
   D) my_list[1]

2. Which module needs to be imported to work with arrays in Python?
   A) list  
   B) array  
   C) numpy  
   D) pandas

3. How do you change the value of the second element in an array named `my_array` to 10?
   A) `my_array[2] = 10`  
   B) `my_array[1] = 10`  
   C) `my_array[0] = 10`  
   D) `my_array[3] = 10`

### Python Assignment: List Manipulation

Write a Python program that takes a list of numbers and returns a new list with only the even numbers from the original list.

### Answer Key:

1. A) my_list[2]  
2. B) array  
3. B) `my_array[1] = 10`  