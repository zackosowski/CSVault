Sorting [[algorithms]] are essential tools in computer science for arranging data in a specific order. Let's explore three common sorting algorithms in detail:

#### Bubble Sort
<hr>
Bubble sort is one of the simplest sorting algorithms. It works by repeatedly stepping through the list, comparing adjacent elements, and swapping them if they are in the wrong order.

**Execution**:
    1. Start at the beginning of the list.
    2. Compare the first two elements. If the first element is greater than the second, swap them.
    3. Move to the next pair of elements and repeat the comparison and swap process until the end of the list is reached.
    4. Repeat steps 1-3 until no swaps are needed, indicating that the list is sorted.
    
**Example**:
	Imagine sorting a deck of cards by comparing adjacent cards and swapping them if they are out of order. Repeat this process until the deck is sorted from lowest to highest card.

#### Merge Sort
<hr>
    
Merge sort is a divide-and-conquer algorithm that divides the input list into smaller sublists, sorts each sublist recursively, and then merges them back together in sorted order.

**Execution**:
    1. Divide the unsorted list into n sublists, each containing one element.
    2. Merge adjacent sublists pairwise to produce new sorted sublists until there is only one sublist remaining.
    3. Repeat the merging process until all sublists are merged into a single sorted list.
**Example**:
	Divide the deck of cards into smaller piles, sort each pile individually, and then merge the sorted piles back together until you have a single sorted deck.

#### Quick Sort
<hr>

Quick sort is a divide-and-conquer algorithm that works by selecting a 'pivot' element from the list and partitioning the other elements into two sublists according to whether they are less than or greater than the pivot. The sublists are then sorted recursively.
**Execution**:
    1. Choose a pivot element from the list.
    2. Partition the list into two sublists: one containing elements less than the pivot and the other containing elements greater than the pivot.
    3. Recursively apply quick sort to the two sublists.
    4. Combine the sorted sublists and the pivot to form a fully sorted list.

**Example**: 
	Select a card from the deck as the pivot, then divide the deck into two piles: one with cards lower than the pivot and the other with cards higher than the pivot. Repeat this process for each pile until the entire deck is sorted.



<hr>

###### <span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

Working with a partner, use the three sorting algorithms above to sort 10 playing cards form lowest to highest value (Aces high).

Start each algorithm by placing all 10 cards face up in a random order on the table before executing the sort.

When done with all three, prepare to answer these three questions:
* Which algorithm was the fastest?
* Which was the slowest?
* Which one felt the most natural?

#### Related Articles
<hr>

[[Algorithms]]