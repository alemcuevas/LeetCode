# Data Structures & Algorithms
All the problems I've solved from https://leetcode.com

Friendly reminder to use this as a last resource, always try to work the problem on your own first.

Concepts that are used over the different coding exercises.

### Arrays

You know the address for every item in the array. 
Arrays start at index zero.
All elements are stored next to each other.
All elements should be of the same type (int, doubles, ...)
Reading O(1)
Insertion O(n)
Deletion O(n)

### Linked Lists

Useful if you want to insert or delete an elements in the middle.
Each item stores the address of the next item in the list.
Elements are stored all over, and element stores the address of the next one.
O(n) time means you touch every element in the list once.
Reading O(n)
Insertion O(1)
Deletion O(1)

### Stack

This is a simple data structure. When you insert an item, it gets added to the top of the list. When you read an item, you only read the topmost item, and it's taken off the list. So the list has only two actions: push (insert) and pop (remove and read)
push = add new item to the top
pop = remove the topmost item and read it
LIFO data structure = Last In, First Out

### Queues

Works like a queue in real life and are also similar to stacks. 
You can't access random elements in the queue. 
If you enqueue two items to the list, the first item you added will be dequeued before the second item.
FIFO data structure = First In, First Out

### Selection sort

To find the highest value you have to check each item in the list. This takes O(n) time and you have to do that n times.
This takes O(n x n) or O(n^2)

### Quicksort

Faster than Selection Sort, it only takes O(n log n)
Worst case = O(n^2)
His the average case more times than the worst case.
It uses Divide & Conquer
1. Pick a pivot
2. Partition the array into two sub-arrays: elements less than the pivot and elements greater than the pivot.
3. Call quicksort recursively on the two sub-arrays
The performance of quicksort depends heavily on the pivot you choose.
Choose a random element as the pivot. The average runtime of quicksort if O(n log n)!

###### Divide & Conquer

Works by breaking a problem down into smaller and smaller pieces.
1. Figure out the base case, should be the simplest possible case.
2. Divide or decrease your problem until it becomes the base case. Figure out how to reduce your problem and get to the base case.

###### Inductive Proofs

It is a way to prove that your algorithm works. Each inductive proof has two steps: the base case and the inductive case. 
For example with quicksort:
In the base case the algorithm works for the base case: arrays of size 0 and 1.
In the inductive case, if quicksort works for an array of size 1, it will work for an array of size 2.
If it works for an array of size 2, it will work for an array of size 3 and so on.

### Recursion

Used when it makes the solution clearer. There is no performance benefit to using recursion, loops are sometimes better for performance.
###### Base case and recursive case
A recursive function calls itself, that is why it's easier to incorrectly write a function that ends up in an infinite loop. You have to tell when to stop recursing.
Recursive case = the function calls itself
Base case = when the function doesn't call itself again, so it doesn't go into an infinite loop.

### Merge Sort

O(n log n)
Slower than quicksort, this is because the constant in Big O can matter sometimes.


### Binary Search

O(log n)

### Simple Search

O(n)

### The Traveling Salesman

O(n!)

### Recommended books

Grokking Algorithms
https://www.oreilly.com/library/view/grokking-algorithms/9781617292231/
