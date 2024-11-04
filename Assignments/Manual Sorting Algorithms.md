#assignment 


In this project, you’ll implement and compare several sorting algorithms to sort lists of integers. You will write your own code for each algorithm using `for` loops and print the sorted lists as well as the number of steps each algorithm took to complete the sort. This will help you understand the mechanics of sorting and practice `for` loop logic.

---
#### Requirements
Write Python functions to implement the following sorting algorithms. Each function should:
1. Take an unsorted list of integers as a parameter.
2. Return the sorted list of integers.
3. Print the number of steps it took to sort.

Each algorithm should be implemented using `for` loops and any required helper functions. 

<span style="position: relative; font-weight: 700;background-color: #C80000; border-bottom: 2px solid #C80000;padding-top:1px; padding-bottom:1px;  padding-left: 11px; padding-right: 7px;border-top: 2px solid #C80000; border-radius:10px 0px 0px 10px;">!</span><span style= "background-color: #520000; margin-left:-14px;padding:3px;padding-left:14px; padding-right:10px;border-right:3px solid #C80000"> Do not use Python’s built-in sort() or sorted() functions.</span>

---
#### Sorting Algorithms to Implement

##### 1. [[Sorting Algorithms#Bubble Sort|Bubble Sort]]
- Use `for` loops to repeatedly compare adjacent elements in the list and swap them if they are in the wrong order.
- Continue looping through the list until it is completely sorted, ensuring no swaps are needed in a final pass.
- Track and print the number of steps the algorithm took to sort the list.

##### 2. [[Sorting Algorithms#Quick Sort|Quick Sort]]
- Choose a "pivot" element, then use `for` loops to partition the list so that elements smaller than the pivot are on one side and elements greater than the pivot are on the other.
- Apply the same steps to the left and right sides of the pivot until the list is sorted.
- Track and print the number of steps needed for sorting

##### 3. [[Sorting Algorithms#Merge Sort|Merge Sort]] (Bonus)
- Write a function to split the list into halves until each half has one element.
- Use `for` loops to merge the split lists back together in sorted order.
- Track and print the number of steps required for merging and splitting.

---
#### Example Workflow

1. **Define a list of integers**: Create a sample list of unsorted integers to test each sorting function. 
2. **Implement each sorting function**: Write and test each sorting algorithm in its own function.
3. **Compare results**: Run each function on the same list, printing the sorted list and the number of steps for each sort.
4. **Analyze**: Think about which sorting method was most efficient in terms of the steps required.

---
#### Example Code Structure

Here's a general outline to help you get started:

```python
# Sample unsorted list
numbers = [34, 7, 23, 32, 5, 62]

def bubble_sort(numbers):
    # Implement bubble sort using for loops
    steps = 0
    # Your code here
    print("Bubble Sort Steps:", steps)
    return sorted_list

def selection_sort(numbers):
    # Implement selection sort using for loops
    steps = 0
    # Your code here
    print("Selection Sort Steps:", steps)
    return sorted_list

def insertion_sort(numbers):
    # Implement insertion sort using for loops
    steps = 0
    # Your code here
    print("Insertion Sort Steps:", steps)
    return sorted_list

# Optional Challenge
def merge_sort(numbers):
    # Implement merge sort (recursively) and use for loops where necessary
    steps = 0
    # Your code here
    print("Merge Sort Steps:", steps)
    return sorted_list
```

---
#### Project Submission
Save your work in a new file in your `assignments` folder named `manualsorting.py` and push to Github
