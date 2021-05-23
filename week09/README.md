## Question 1 - All the Same

Write a function that checks if all items in the following tuple are the same

| Input            | Output |
| ---------------- | ------ |
| 4<br>45 45 45 45 | True   |
| 3<br>12 34 12    | False  |

## Question 2 - Fractions

Fractions can be expressed as as tuple: (numerator, denominator).

Write a function that adds two fractions that are passed as tuples.

| Input         | Output   |
| ------------- | -------- |
| (1, 3) (4, 5) | (17, 15) |
| (3, 5) (1, 2) | (11, 10) |

## Question 3 - Tuples/Lists

#### Question 3a - Lists inside Tuple

Write a function which takes a tuple of lists and a number and replaces last item of lists in the tuple with given
number and returns modified tuple.

| Input                                          | Output                                        |
| ---------------------------------------------- | --------------------------------------------- |
| ([10, 20, 40], [40, 50, 60], [70, 80, 90]) 100 | ([10, 20, 100], [40, 50, 100], [70, 80, 100]) |
| ([10, 20], [40, 50], [70, 80]) 30              | ([10, 30], [40, 30], [70, 30])                |

#### Question 3b - Tuples inside List

Write a function which takes a list of tuples and a number and replaces last value of tuples in the list with given
number and returns modified list.

| Input                                          | Output                                        |
| ---------------------------------------------- | --------------------------------------------- |
| [(10, 20, 40), (40, 50, 60), (70, 80, 90)] 100 | [(10, 20, 100), (40, 50, 100), (70, 80, 100)] |
| [(10, 20), (40, 50), (70, 80)] 30              | [(10, 30), (40, 30), (70, 30)]                |

## Question 4 - Neighbors

Write a program which takes a list of integer and creates a new list with same number of elements as given list such
that each integer in the new list is the sum of its neighbors and itself in given list.

| Input                | Output                |
| -------------------- | --------------------- |
| [10, 20, 30, 40, 50] | [30, 60, 90, 120, 90] |

## Question 5 - Points

Points can be expressed as as tuple: (x, y).

#### Question 5a - Distance

Write a function  **distance** which takes two tuples (points) and returns Euclidian distance between these points.

| Input           | Output |
| --------------- | ------ |
| (3, 0) (0, 4)   | 5.0    |
| (5, 8) (10, 20) | 13.0   |

#### Question 5b - Closest

Write a function which takes two tuples (points) and returns the point closest to the origin. *Use the distance
function.*

| Input          | Output |
| -------------- | ------ |
| (3, 0) (0, 4)  | (3, 0) |
| (11, 7) (6, 8) | (6, 8) |

#### Question 5c - Farthest

Write a program which takes an integer N and reads N points (given by their x and y coordinates) and determines the pair
that is the farthest apart.

| Input                                       | Output              |
| ------------------------------------------- | ------------------- |
| 3<br/>3 0<br/>0 0<br/>0 4                   | (0, 4)<br/>(3, 0)   |
| 5<br/>10 5<br/>4 8<br/>0 8<br/>4 5<br/>-1 2 | (-1, 2)<br/>(10, 5) |

## Question 6 - Insertion

Write a program that creates a list and takes 5 integers from the input. If an integer is bigger than or equal to the last element in the list, add it. If not, do not add it to the list. Then print out the list. (Add the very first integer without any condition check.) Extra: You can print out the elements of a list without brackets or commas, simply putting "*" in front of the list variable. 
* print(mylist) --> [1, 2, 3]
* print(*mylist) --> 1 2 3

| Input       | Output    |
| ----------- | --------- |
| -5 3 25 8 0 | -5 3 25   |
| 6 4 2 8 14  | 6 8 14    |
| 0 1 2 3 3   | 0 1 2 3 3 |

## Question 7

Create a function that returns the majority vote in a list. A majority vote is an element that occurs > N/2 times in a list (where N is the length of the list).<br>

| Input                          | Output |
| ------------------------------ | ------ |
| ["A", "A", "B"]                | "A"    |
| ["A", "A", "A", "B", "C", "A"] | "A"    |
| ["A", "B", "B", "A", "C", "C"] | None   |


**Notes:**<br>
The frequency of the majority element must be strictly greater than 1/2.<br>
If there is no majority element, return None.<br>
If the list is empty, return None.<br>

## Question 8

Write a function which takes a list of integers and an integer n. This function will 'slice' the initial list into smaller lists such that individual sums of elements in each smaller list exceed n the first time while reading the elements of the list from left to right.

**Example:** 
| Input                                               | Output                                              |
| --------------------------------------------------- | --------------------------------------------------- |
| sliceList([5, 3, 2, 1 ,4 ,51, 2, 1, 3, 5, 3, 5], 4) | [[5], [3, 2], [1, 4], [51], [2, 1, 3], [5], [3, 5]] |

## Question 9

Write a function which takes a list of strings. The input list has even number of elements. Your function is supposed to pair the first element with the last, the second element with the second last and so on. The function will return these pairs as tuples inside a list.

**Example:** 
| Input                                                        | Output                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| reversePair(['Krillson', 'Fisherman', 'Chris', 'Wilson', 'Jack', 'The Handsome']) | [('Krillson', 'The Handsome'), ('Fisherman', 'Jack'), ('Chris', 'Wilson')] |

## Question 10

Write a function which takes a list and shuffles in a specific way and then return it. The shuffle is as follows: odd number indexed elements are moved to the end of the list with their respective order. If you are confused, here is an example.

**Example:** 
| Input                                      | Output                      |
| ------------------------------------------ | --------------------------- |
| shuffleDouble([1, 2, 3, 4, 5, 6, 7, 8, 9]) | [1, 3, 5, 7, 9, 2, 4, 6, 8] |


## Question 11
 A list of tuples with integers are given. However, there are some strings pretending to be integers in the tuples. Write a program that returns a list with tuples including only integers.

<em> Hint: You can check the types with type() function. </em>

| Input                                                        | Output                                      |
| ------------------------------------------------------------ | ------------------------------------------- |
| [("1", 2), (3, 4), (5, "6"), (7, 5, 8), ("9", 10)]           | [(3, 4), (7, 5,  8)]                        |
| [(15, 23), (46, 80), (9, 36, 19), ("60", "25"), ("43", 96, 81, 10), ("2", 56, 17), (17, 17) ] | [(15, 23), (46, 80), (9, 36, 19), (17, 17)] |
| [("1", "11", 3), ("87", 74), (0, "99")]                      | []                                          |

## Question 12
Given a list of tuples (each tuple consists of two integer elements), write a program that constructs a new list from the given list, only consisting of tuples whose elements are in descending order.

<em> Extra: Define a function named descending() that returns True if our tuple satisfies the condition and try to construct desired output using list comprehension. </em>

| Input                                                        | Output                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------- |
| [(10, 9), (240, 240, 240), (55, -43), (34, 71), (283, 16)]   | [(10, 9), (55, -43), (283, 16)]                         |
| [(114, 18, 9, 1), (21, 30), (46, 25, 8), (154, -32), (345, 267), (456, 775), (102, 1345)] | [(114, 18, 9, 1),  (46, 25, 8), (154, -32), (345, 267)] |
| [(1, 1, 1, 2), (3, 0, 4), (5, 6, 7, 8), (7, 8), (9, 10)]     | []                                                      |

## Question 13
 A list of tuples is given. Each tuple consists of 2 elements: Student ID and grade. Write a program that sorts these tuples according to the grades in ascending order. If two students have the same grade, do not swap them.

<em> Hint: You can use sort() method of the lists, you should define a lambda function to sort according to the grades. </em>

| Input                                                        | Output                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [(2030432, 67), (2030564, 85), (2140315, 75), (2165970, 81)] | [(2030432, 67), (2140315, 75), (2165970, 81), (2030564, 85)] |
| [(1990234, 45), (1976435, 78), (1980543, 60), (2054670, 55), (2456790, 78)] | [(1990234, 45), (2054670, 55), (1980543, 60), (1976435, 78), (2456790, 78)] |
| [(2121777, 86), (2120654, 90), (1990650, 83), (2298755, 86)] | [(1990650, 83), (2121777, 86), (2298755, 86), (2120654, 90)] |

## Question 14

Write the `odd_parity_checker(signal, target)` function.<br>
signal is ensured to be a tuple that has a boolean value as its first element which we will call **parity**. <br>
The rest of the signal is called **information**. <br>
signal has at least 2 elements. <br>
Inside the function you should check whether target appears odd many times in signal's information part. <br>
If the truth value of your check is the same as parity, the function should return true, else return false.

| Input                                                     | Output          |
| --------------------------------------------------------- | --------------- |
| (True, False, True, True, True, False, False, True), True | Signal faulty.  |
| (True, 14, True, 21, 14, False, "Hello", True), 14        | Signal faulty.  |
| (True, 14, True, 21, 14, False, "Hello", True), 21        | Signal correct. |

