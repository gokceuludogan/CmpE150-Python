## Question 1 - All the Same

Write a function that checks if all items in the following tuple are the same

| INPUT            | OUTPUT |
| ---------------- | ------ |
| 4<br>45 45 45 45 | True   |
| 3<br>12 34 12    | False  |

## Question 2 - Filter Even Numbers

Write a function that takes a list then returns it without even numbers.

| Input           | Output       |
| --------------- | ------------ |
| [1,2,3,4,5,6,7] | [1, 3, 5, 7] |
| [2,4,6,8]       | [ ]          |

## Question 3 - List Comprehension

#### Question 3a - Even Sum

Write a function which takes a list of integers and returns the sum of the even integers in this list using list comprehension. 

| Input           | Output |
| --------------- | ------ |
| [1, 2, 3, 4, 5] | 6      |
| [1, 3, 5, 7]    | 0      |

#### Question 3b - Odd Sum

Write a function which takes a list of integers and returns the sum of the odd integers in this list using list comprehension. 

| Input           | Output |
| --------------- | ------ |
| [1, 2, 3, 4, 5] | 9      |
| [2, 18, 6, 0]   | 0      |

## Question 4 - Remove Duplicates

Write a function that takes a list of integers then returns without all duplicates.

| Input                                   | Output          |
| --------------------------------------- | --------------- |
| [1, 1, 1, 1, 1, 2, 2, 2, 3, 2, 2, 4, 5] | [1, 2, 3, 4, 5] |
| [0,0,0,0,0,0,0]                         | [0]             |

## Question 5 - Remove Consecutive Duplicates

Write a function that takes a list of integers then returns without consecutive duplicates.

| Input                                   | Output             |
| --------------------------------------- | ------------------ |
| [1, 1, 1, 1, 1, 2, 2, 2, 3, 2, 2, 4, 5] | [1, 2, 3, 2, 4, 5] |
| [0,0,0,0,0,0,0]                         | [0]                |

## Question 6 - Odd Occurrences

Write a function that takes a list and prints the elements that occur 2n+1 times. If there is no element with odd number of occurrences then it should not print anything.

| Input                                           | Output    |
| ----------------------------------------------- | --------- |
| [1, 1, 2, 3, 4, 2, 'apple', 'banana', 'banana'] | 3 4 apple |
| [2, 2, 3, 3, 2]                                 | 2         |
| [ 'a' , 'b' , 'c' , 'c' , 'b' , 'a' ]           |           |

## Question 7 - Neighbors

Write a program which takes a list of integer and creates a new list with same number of elements as given list such that each integer in the new list is the sum of its neighbors and itself in given list.

| Input                | Output                |
| -------------------- | --------------------- |
| [10, 20, 30, 40, 50] | [30, 60, 90, 120, 90] |

## Question 8 - Circulation

#### Question 8a - To the left

Write a function which takes a list of numbers and an integer k and shifts the numbers to the left circularly by *k* and return the shifted list.

| Input             | Output          |
| ----------------- | --------------- |
| [1, 2, 3, 4, 5] 2 | [3, 4, 5, 1, 2] |
| [2, 18, 6, 0] 3   | [0, 2, 18, 6]   |

#### Question 8b - Left or right?

Write a function which takes a list of numbers and an integer *k* and a boolean *is_left* specifying the shift direction and shifts the numbers to the left or right circularly by *k* and return the shifted list.

| Input                  | Output          |
| ---------------------- | --------------- |
| [1, 2, 3, 4, 5] 2 True | [3, 4, 5, 1, 2] |
| [2, 18, 6, 0] 3 False  | [18, 6, 0, 2]     |

## Question 9 - Points

Points can be expressed as as tuple: (x, y).

#### Question 9a - Distance

Write a function  **distance** which takes two tuples (points) and returns Euclidian distance between these points. 

| Input           | Output |
| --------------- | ------ |
| (3, 0) (0, 4)   | 5.0    |
| (5, 8) (10, 20) | 13.0   |

#### Question 9b - Closest

Write a function which takes two tuples (points) and returns the point closest to the origin. *Use the distance function.*

| Input          | Output |
| -------------- | ------ |
| (3, 0) (0, 4)  | (3, 0) |
| (11, 7) (6, 8) | (6, 8) |

#### Question 9c - Farthest

Write a program which takes an integer N and reads N points (given by their x and y coordinates) and determines the pair that is the farthest apart.

| Input                                       | Output              |
| ------------------------------------------- | ------------------- |
| 3<br/>3 0<br/>0 0<br/>0 4                   | (0, 4)<br/>(3, 0)   |
| 5<br/>10 5<br/>4 8<br/>0 8<br/>4 5<br/>-1 2 | (-1, 2)<br/>(10, 5) |

## Question 10 - Fractions

Fractions can be expressed as as tuple: (numerator, denominator).

#### Question 10a - Addition

Write a function that adds two fractions that are passed as tuples.

| Input         | Output   |
| ------------- | -------- |
| (1, 3) (4, 5) | (17, 15) |
| (3, 5) (1, 2) | (11, 10) |

#### Question 10b - Multiplication

Write a function that adds two fractions that are passed as tuples.

| Input         | Output  |
| ------------- | ------- |
| (1, 3) (4, 5) | (4, 15) |
| (3, 5) (1, 3) | (1, 5)  |

## Question 11 - Tuples/Lists

#### Question 11a - Lists inside Tuple

Write a function which takes a tuple of lists and a number and replaces last item of lists in the tuple with given number and returns modified tuple.

| Input                                          | Output                                        |
| ---------------------------------------------- | --------------------------------------------- |
| ([10, 20, 40], [40, 50, 60], [70, 80, 90]) 100 | ([10, 20, 100], [40, 50, 100], [70, 80, 100]) |
| ([10, 20], [40, 50], [70, 80]) 30              | ([10, 30], [40, 30], [70, 30])                |

#### Question 11b - Tuples inside List

Write a function which takes a list of tuples and a number and replaces last value of tuples in the list with given number and returns modified list.

| Input                                          | Output                                        |
| ---------------------------------------------- | --------------------------------------------- |
| [(10, 20, 40), (40, 50, 60), (70, 80, 90)] 100 | [(10, 20, 100), (40, 50, 100), (70, 80, 100)] |
| [(10, 20), (40, 50), (70, 80)] 30              | [(10, 30), (40, 30), (70, 30)]                |

## Question 12 - Tuple Sort Tuple

Write a function that sorts a tuple of tuples by 2nd item.

| INPUT                                     | OUTPUT                                       |
| ----------------------------------------- | -------------------------------------------- |
| (('a', 23),('b', 37),('c', 11), ('d',29)) | (('c', 11), ('a', 23), ('d', 29), ('b', 37)) |

