# Loops

## Question 1 - Staaaars

### Question 1a
Write a program that prints 1 star ('\*') to the screen.

### Question 1b
Write a program that prints 10 stars ('\*') next to each other to the screen.

### Question 1c
Write a program that reads an integer N and prints N stars ('\*') vertically to the screen.

### Question 1d
Write a program that reads an integer N and prints N stars ('\*') next to each other to the screen.



## Question 2 - Numbeeeers

Write a program that reads an integer N and prints numbers from 1 to N to the screen.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 5  | 1 2 3 4 5   |
| 2  | 1 2  |



## Question 3 - Hooping Numbers

### Question 3a

Write a program that reads 3 integers A, B and t from the user. Then prints numbers from A to B with increment of t. Assume that B > A.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 7 16 3  | 7 10 13 16 |
| 2 30 6  | 2 8 14 20 26 |


### Question 3b

Write a program that reads 3 integers A, B and t from the user. Then prints numbers from B to A with decrement of t. Assume that B > A.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 7 16 3  | 16 13 10 7 |
| 2 30 6  | 30 24 18 12 6 |



## Question 4 - Even Numbeeeers

Write a program that reads two integers A and B. Then prints the sum of even numbers between A and B. Assume that B > A.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 3 8  | 10 |
| 2 13 | 40  |
| 3 5 | 4  |



## Question 5 - Average Team

Write a program that reads a number N, then reads N more numbers. Calculate the average of those N numbers.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 4<br>4 9 5 2  | 5.0 |
| 1<br>8 | 8.0  |


## Question 6 - Boom Boom POW

Write a program that takes 2 integers a and b, then prints the result of a^b (a\*a\*a...\*a\*a). 

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 3 4  | 81 |
| 2 10  | 1024 |


## Question 7 - Factorial

Write a program that takes an integer n and then prints n!.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 5 | 120 |
| 10 | 3628800 |


## Question 8 - Fibonacci

Write a program which reads a positive integer number N , and prints the Nth fibonacci number. *0, 1, 1, 2, 3, 5, ...* 

F_0 = 0, F_1 = 1, F_n = F\_(n-2) + F\_(n-1)

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 2  | 1 |
| 4  | 2 |
| 7  | 8 |


## Question 9 - Second Largest

Write a program that will take nonnegative integers as inputs until the user enters 0. Then prints the difference between of largest two numbers among given inputs.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 12 25 3 8 0 | 13 |
| 15 1 2 3 8 -2 5 0  | 7 |


## Question 10 - Digiiiits

Write a program that takes a number and prints its total digit count and also even digit sum.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 542175 | 6 6 |
| 24680 | 5 20 |
| 135 | 3 0 |


## Question 11 - Positive Mental Attitude

Write a program that will take integers as inputs until the user enters a negative number. Then shows the user the sum of all ODD non-negative numbers that is entered.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 4 7 45 9 2 0 0 5 8 -4  | 66 |
| 1 1 0 1 -1 | 3 |


## Question 12 - NoBig

Write a program that reads numbers until the entered number is greater than the previous entered number. Then print the average of all entered numbers except the last one. (At least two numbers will be entered)

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 5 4 3 3 8 | 3.75 |
| 5 4 3 3 8 7 5 9 | 3.75 |
| 1 2 | 1.0 |
| 100 54 46 2 3 50| 50.5 |


## Question 13 - Guess

Generate a random number between 1 and 100 (including 1 and 100). Ask the user to guess the number, then tell them whether they guessed too low, too high, or exactly right. Also print the number of tries.


| Input | Output          |
| ----- | --------------- |
| 35<br>67<br>73<br>71 | Too low!<br>Too low!<br>Too high!<br>You got it!<br>And it only took you 4 tries! |


## Question 14 - Basic Calculator

Write a simple calculator that takes an integer and then performs + - \* / operations until user enters q. If user enters +-\*/ then take another integer and carry out appropriate calculation. If user enters, q then quit program. If user enters h, then print out these instructions.

Example run

```
Please enter number: 15
Please enter operation: *
Enter another number: 2
Number is 30 now
Enter another operation (h for help): +
Enter another number: 6
Number is 36 now
Enter another operation (h for help): -
Enter another number: 9
Number is 27 now
Enter another operation (h for help): /
Enter another number: 2
Number is 13 now
Enter another operation (h for help): h
q for quit
h for help
+ for addition
- for subtraction
* for multiplication
/ for integer division
Number is 13 now
Enter another operation (h for help): q

Process finished with exit code 0
```

