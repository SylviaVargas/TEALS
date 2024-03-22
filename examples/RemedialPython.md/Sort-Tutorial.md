### Tutorial: Python Sorting

Sorting in Python refers to arranging elements in a particular order. Python provides several methods for sorting lists and other iterable objects. Here are some examples of sorting in Python:

#### 1. Sorting a list of numbers
```python
numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
numbers.sort()
print(numbers)  # Output: [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]
```

#### 2. Sorting a list of strings
```python
fruits = ["apple", "banana", "orange", "cherry"]
fruits.sort()
print(fruits)  # Output: ['apple', 'banana', 'cherry', 'orange']
```

#### 3. Sorting in reverse order
```python
numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
numbers.sort(reverse=True)
print(numbers)  # Output: [9, 6, 5, 5, 5, 4, 3, 3, 2, 1, 1]
```

#### 4. Sorting a list without modifying the original list
```python
numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
sorted_numbers = sorted(numbers)
print(sorted_numbers)  # Output: [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]
print(numbers)         # Output: [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
```

#### 5. Sorting a dictionary by value
```python
my_dict = {"apple": 5, "banana": 2, "orange": 8, "cherry": 1}
sorted_dict = {k: v for k, v in sorted(my_dict.items(), key=lambda item: item[1])}
print(sorted_dict)  # Output: {'cherry': 1, 'banana': 2, 'apple': 5, 'orange': 8}
```

#### 6. Sorting a list of tuples by the second element
```python
tuples = [(1, 'one'), (3, 'three'), (2, 'two')]
tuples.sort(key=lambda x: x[1])
print(tuples)  # Output: [(1, 'one'), (2, 'two'), (3, 'three')]
```

#### 7. Sorting a list of objects by an attribute
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

people = [Person("Alice", 25), Person("Bob", 30), Person("Charlie", 20)]
people.sort(key=lambda x: x.age)
for person in people:
    print(person.name, person.age)
```

#### 8. Sorting with a custom comparison function
```python
def custom_sort(x):
    return x % 3

numbers = [9, 5, 7, 2, 4, 1, 6, 8, 3]
numbers.sort(key=custom_sort)
print(numbers)  # Output: [9, 6, 3, 1, 4, 7, 5, 2, 8]
```

#### 9. Sorting with a key function and reverse order
```python
numbers = [9, 5, 7, 2, 4, 1, 6, 8, 3]
sorted_numbers = sorted(numbers, key=lambda x: -x)
print(sorted_numbers)  # Output: [9, 8, 7, 6, 5, 4, 3, 2, 1]
```

#### 10. Sorting a list of strings ignoring case
```python
fruits = ["Apple", "banana", "Orange", "cherry"]
sorted_fruits = sorted(fruits, key=lambda x: x.lower())
print(sorted_fruits)  # Output: ['Apple', 'banana', 'cherry', 'Orange']
```

### Quiz: Python Sorting

1. What is the output of the following code?
   ```python
   numbers = [5, 2, 8, 1, 6]
   sorted_numbers = sorted(numbers)
   print(sorted_numbers)
   ```
   A) [5, 2, 8, 1, 6]  
   B) [1, 2, 5, 6, 8]  
   C) [8, 6, 5, 2, 1]  
   D) [1, 2, 8, 5, 6]

2. How can you sort a list of strings in reverse alphabetical order?
   A) Use `sort()` method with `reverse=True`  
   B) Use `sorted()` function with `reverse=True`  
   C) Use `sort()` method with a custom comparison function  
   D) Use `sorted()` function with a custom comparison function

3. What is the output of the following code?
   ```python
   numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
   numbers.sort()
   print(numbers)
   ```
   A) [9, 6, 5, 5, 5, 4, 3, 3, 2, 1, 1]  
   B) [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]  
   C) [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]  
   D) [9, 6, 5, 3, 3, 4, 2, 1, 1, 5, 5]

### Python Assignment: Sorting Names

Write a Python program that takes a list of names and sorts them in alphabetical order. Ignore case while sorting.

### Answer Key:

1. B) [1, 2, 5, 6, 8]  
2. B) Use `sorted()` function with `reverse=True`  
3. B) [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]