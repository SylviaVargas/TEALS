- Sequential Sort Algorithm
This lesson covers a well-known algorithm called the linear search.  A linear search involves scanning a list, with a loop, and testing each item in turn to see if the list contains the target value.  You will learn how to write code for a linear search using a while loop.  You will also learn how to perform the same task using an if statement with the in operator.  This lesson mentions how a list is stored in the computer’s memory, and the impact of this on the efficiency of a linear search compared with retrieving an individual item in a list if its index number is known.


Another Python Editor
- https://www.online-python.com/

References:
- https://www.programiz.com/python-programming/list
- https://www.w3resource.com/python-exercises/data-structures-and-algorithms/python-search-and-sorting-exercise-2.php
- https://www.geeksforgeeks.org/linear-search/

Videos:
- https://www.youtube.com/watch?v=6spy23DRYIU
- https://www.youtube.com/shorts/FteB3gE7U9M - Quick overview
- https://www.youtube.com/watch?v=u46nNK4lmeE - Best example
- https://www.youtube.com/watch?v=I-CIYnyAFzQ - Linear Search Algorithm - Python Example and Code 
- https://www.youtube.com/watch?v=9KBwdDEwal8 - QuickSort (Too advanced for student)

## Part 1
1. What does the following do?

``` python
numbers = [8, 6, 7, 5, 3, 0, 9]
states =  ["Michigan", "California",
    "Missouri", "Washington",
    "Illinois", "Georgia"
]
print("Numbers:")
print(numbers)
print("States:")
print(states)

```

## Part 2
``` python
def number_search(needle: number, haystack: List[number]):
    return -1
```


# Part 3
``` python
def array_search(array: List[any], search_term: any):
    return -1

```

# Part 4 Sorting
``` python
def compare_numbers(value1: number, value2: number):
    if (value1 < value2):
        return -1
    elif (value1 == value2):
        return 0
    else:
        return 1

def compare_numbers(value1: number, value2: number):
    return value1 - value2
```


## Another example - Searching 
- Video: https://www.youtube.com/watch?v=6spy23DRYIU
``` python
# Variables
cities =["London","New York", "Paris", "Munich", "Tokyo", "Mumbai", "Amsterdam", "Seattle"]
i = 0 
found = False

# Program
print("Running Linear Search" )
while i < len(citied):
    if cities[i] == "Tokyo"
        found = True
        break
    i = i +1

if found == "True"
    print("The city is found in the list!")
else:
    print("The city is NOT found in the list!")
```

### Another example: continued

``` python
print("Another example!")
if "Tokyo" in cities:
    print("The city is found in the list!")
else:
    print("The city is NOT found in the list!")
```


Another Sorting example:
- https://makecode.com/_c587Uj0tp0vk - Python 3.4 - Example 