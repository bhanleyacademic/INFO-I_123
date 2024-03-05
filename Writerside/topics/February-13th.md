# February 13th

## Canvas
INTRODUCTION

What is an algorithm? Is it a complex mathematical formula or a dense chunk of computer code? At its core, an algorithm is much simpler than this. An algorithm is a recurring problem that is solved through a series of well-defined steps. A good algorithm is a powerful tool because it can be used by many different people in many different situations to reliably solve a problem. Understanding algorithms will help you think about how to use and analyze data, but it will also help you think more critically about problem solving in general.

Icons-Gray_target.png  LEARNING OBJECTIVES

Students will be able to:

1) Define what an algorithm is

2) Write an algorithm to solve a problem in everyday life

3) Explain the steps of simple, classic algorithms

4) Identify the efficiency of an algorithm

5) Identify greedy algorithms

6) Critique how well-written an algorithm is



OFFICE HOURS

Joshua Nunley (joshnunl@iu.edu): Wednesdays, 5-6 pm on Zoom or email for appointment

Staša Milojević (smilojev@indiana.edu): Thursdays, 3-4 pm, Luddy Center for Artificial Intelligence (1015 E. 11th St.) 2032 or email for appointment

Devin Wright  (devrwrig@iu.edu): Fridays 11am-12pm, Zoom

Links to an external site.Links to an external site. or email for appointment

Icons-Gray_clipboard.png  TO-DO

1) Watch all of the video below (in the Resources - Videos section) prior to coming to class. Be sure to take notes as you watch.

2) Join us in class on Tuesday to expand your understanding of these concepts and practice applying them.



RESOURCES - VIDEOS

https://youtu.be/fkIvmfqX-t0

RESOURCES - MAJOR CONCEPTS

An algorithm is a finite set of precise instructions for performing a computation or solving a problem.

Directions need to be specific and unambiguous

Individual steps need to be broken down as completely as possible

Individual steps are not themselves complex tasks

Input – An algorithm has input values from a specified set.

Output – From each set of input values an algorithm produces output values from a specified set. The output values are the solution to the problem.

Search – finding a target element within a list

     Linear / Sequential Search

     Binary Search (Used for the lists with terms occurring in order of increasing size)

Sort – given a list, produce the same list sorted

     Bubble Sort (flip pairs if they’re in the wrong order, multiple passes)

     Insertion sort (better (simpler) than bubble sort, but still far from optimal (number of comparisons).

Greedy algorithms take the ‘cheapest’ choice in every decision.

Greedy algorithms frequently find good solutions, but they may miss the optimal (best) solution.

RESOURCES - OPTIONAL

Want to see searching and sorting algorithms in action? Check out these videos where dancers enact these classic algorithms!

"AlgoRythmics" Playlist (Linear Search, Binary Search, Insert Sort, Bubble Sort):

https://youtu.be/-PuqKbu9K3U?list=PLaagToR1Z6nYCYw_-xTWVvSBmRD4fY0BR

## Lecture
### Using Psuedo Code
Useful to solving the problem before going to code.
### Bad Algorithms
- **Assume the solution**
- **Assume things about the data**
- **Steps that that are too complicated**

### Worksheet Problem 1
Array (8,6,7,5,3,0,9,2)
1. Let length = the number of items in the array
2. Let position = 0
3. Let total = 0
4. If position is less than length: Add number at position to total, and add 1 to position. Return to Step 4.
5. If position is not less than length, return total divided by length
```Python
array = [8,6,7,5,3,0,9,2]
length = len(array)
position = 0
total = 0
if position < length:
    total += array[position]
    position += 1
print(total/length) 
```

### Worksheet Problem 3
Input "Bunny"
1. Set length = the number of letters in the word
2. Set position = 0
3. If position is less than length, check if the letter at position is "y." If it is "y", return TRUE and stop computing. If it is not "y", add 1 to position and go back to Step 3.
4. If position is NOT less than length, return FALSE.
```Python
input = "bunny"
length = len(input)
position = 0
if position < length:
    if input[position] == "y":
        return True
    else:
        return False 
```
### Search algorithms
#### Linear Search
- slow
- goes in order
#### Binary Search
- Can't use binary search in unsorted data

Where is 5 in

|0|3|5|6|7|8|9|Array|
|---|--|--|--|--|--|--|
|0 | 1|2|3|4|5|6|Position|

1. Set min = first position. Set max = last position.
2. Otherwise, set position to the average. If min>max, return "TARGET not in list." of min and max (rounding down to a whole number).
3. Check number at position:
   * If too high: set max to current position -1 and go back to step 2.
   * If too low: set min to current position +1 and go back to step 2.
   * If number = target, return position

### Sorting Algorithms
#### Bubble Sort
- focus on pairs
#### Insertion Sort O(n)
- Simpler than bubble sort, but still far from optimal
#### Greedy Algorithm
- Chooses locally optimal choice
- Misses optimal solution
- Computationally cheaper
- Easy to write
- Frequently find good solutions
### Time complexity
Time to solve a problem depends on:
- The machine running the algorithm
- The number of elementary operations performed by the algorithm 
