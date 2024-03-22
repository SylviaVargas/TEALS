### Tutorial: Basic Search in Python

Searching in Python involves looking for a specific element or value in a collection of data. Two common methods for basic search are linear search and binary search.

#### Linear Search
Linear search is a simple method for finding a target value within a list. It checks each element in the list sequentially until a match is found or the whole list has been searched.
```python
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1

# Example usage
numbers = [2, 5, 8, 10, 13]
index = linear_search(numbers, 8)
print(index)  # Output: 2
```

#### Binary Search
Binary search is a more efficient method for finding a target value in a sorted list. It works by repeatedly dividing the list in half and narrowing down the search range.
```python
def binary_search(arr, target):
    low = 0
    high = len(arr) - 1
    while low <= high:
        mid = (low + high) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return -1

# Example usage
numbers = [2, 5, 8, 10, 13, 17, 20]
index = binary_search(numbers, 13)
print(index)  # Output: 4
```

### Examples:
1. Linear search to find the index of a value in a list.
2. Binary search to find the index of a value in a sorted list.

### Quiz: Basic Search in Python

1. What is the time complexity of linear search?
   A) O(1)  
   B) O(log n)  
   C) O(n)  
   D) O(n^2)

2. Which type of search requires the list to be sorted?
   A) Linear search  
   B) Binary search  
   C) Both  
   D) Neither

3. What is the output of the following code using linear search?
   ```python
   numbers = [4, 6, 8, 10, 12]
   index = linear_search(numbers, 5)
   print(index)
   ```
   A) 0  
   B) 1  
   C) 2  
   D) -1

### Python Assignment: Search and Replace

Write a Python program that takes a list of strings and a target string. The program should search for the target string in the list and replace it with a new string if found. Return the modified list.

### Answer Key:

1. C) O(n)  
2. B) Binary search  
3. D) -1