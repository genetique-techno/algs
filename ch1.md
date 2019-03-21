# Chapter 1: Introduction to Algorithms

Big O Notation: the running time of an algorithm
Algorithm: a set of instructions for accomplishing a task

# Binary Search Pseudocode
1. use `low` and `high` to keep track of what part of the list you are searching
  2. while low is lower than high, keep guessing
  3. set mid to high - low and round down
  4. check if mid = the item you're searching for
  5. if mid is greater than the item, set high to mid and repeat
  6. if mid is less than the item, set low to mid and repeat
  7. if you don't find it, do something


Exercises:
1.1  For a list of 128 sorted names, the max number of steps it would take with a binary search is log2(128), or 7 steps.

1.2  If the list is doubled, it takes only 1 more step because the steps are now log2(256), or 2^8, or 8 steps

# Running Time

Linear Time: the time to completion scales linearly with the size of the dataset
Logarithmic Time: time to completion scales logarithmically with size of dataset

O(n) <- linear time
O(log n) <- logarithmic time

# Big O Notation
Algorithm running times scale at different rates
- it's not sufficient to know how fast or slow an algorithm is--you have to know how its running time scales with dataset size
- big "O": Operations.  Tells you how fast an algorithm grows in operations

Examples from fastest to slowest:
O(log n) "logarithmic time"
O(n) "linear time"
O(n log n)
O(n^2)
O(n!) "factorial time"

Exercises:
Give the big o notation for the following
1.3 Find a person's name in the phone book: O(log n) (binary search)

1.4 With the phone number only:  O(n)  (simple search, phone book isn't sorted by phone number)

1.5 You want to read the number of every person in the phone book:  O(n) because you have to scan through the entire book

1.6 You want to read the numbers of just the A's in the phone book:  O(log n) to find the last A, then O(n) to scan the numbers

# Traveling Saleperson algorithm
For a salesperson trying to take the shortest distance to travel to 5 cities you must measure the distance to travel every possible permutation of the 5 cities and take the smallest.  It ends up being O(n!), and the rate that it grows in operations is DRASTIC.  For 5 cities it's 120 operations, for 6: 720, for 7: 5040...for 15 cities: 1.3 trillion operations!!!



