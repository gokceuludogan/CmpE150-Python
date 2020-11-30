# Nested Loops

## Question 1 - R\*\*\*tangle

### Question 1a
Write a program which takes two positive integers as N and M then prints a rectangle with size NxM. 

| Input | Output                               |
| :---: | ------------------------------------ |
|  3 4  | \*\*\*\*<br />\*\*\*\*<br />\*\*\*\* |
|  2 6  | \*\*\*\*\*\*<br />\*\*\*\*\*\*        |


### Question 1b
Write a program which takes two positive integers as N and M then prints a rectangle with size NxM which has stars (\*) at borders, and lines (-) inside.

| Input | Output                                              |
| :---: | --------------------------------------------------- |
|  3 3  | \*\*\*<br />\*-\*<br />\*\*\*                       |
|  4 5  | \*\*\*\*\*<br />\*---\*<br />\*---\*<br />\*\*\*\*\* |


## Question 2 - TriNumber

### Question 2a
Write a program to display a right angle triangle using the number N, which will repeat the number for that row, like below.

| Input | Output                                  |
| :---: | --------------------------------------- |
|   3   | 1<br />22<br />333                      |
|   5   | 1<br />22<br />333<br />4444<br />55555 |


### Question 2b
Write a program to display a right angle triangle with N number of rows, like below.

| Input | Output                                  |
| :---: | --------------------------------------- |
|   3   | 1<br />12<br />123                      |
|   5   | 1<br />12<br />123<br />1234<br />12345 |

<details><summary>Hint</summary> At each row, we iterate from 1 to the row number.</details>


### Question 2c
Write a program which takes two integer as N and x and display a right angle triangle with N number of rows formed by powers of x as follows:

| Input | Output                                |
| :---: | ------------------------------------- |
|  3 4  | 4<br />4 16 <br />4 16 64             |
|  4 3  | 3<br />3 9<br />3 9 27<br />3 9 27 81 |

<details><summary>Hint</summary> At each row, we take power of input integer from once to the row number times.</details>


## Question 3 - TriHard

Write a program which takes an integer N as input and prints a right triangle which consists of N many lines.

```
Input:
3

Output:
--*
-**
***

Input:
5

Output:
----*
---**
--***
-****
*****
```

### Question 4 - Zzz

Write a program which takes positive integer n greater than 2 and prints letter 'Z' size of n using '\*'.

```
Input:
3

Output:
***
 * 
***

Input:
6

Output:
******
    * 
   *  
  *   
 *    
******
```


## Question 5 - Sum Facts

Write a program which takes an integer as input and computes the sum of the factorial of each digit.  For example, assume that the user enters 572 as the input. For each digit of the integer, you will compute the factorial. Then you will compute the sum of these factorials: 5! + 7! + 2! = 120 + 5040 + 2 = 5162.

| Input | Output |
| ----- | ------ |
| 572   | 5162   |
| 27    | 5042   |


## Question 6 - Sum of Digits

Write a program that takes an integer n and calculates sum of all digits. If the result has more than one digit, continue to calculate in this way until a single digit number is produced.

```
16  -->  1 + 6 = 7
942  -->  9 + 4 + 2 = 15  -->  1 + 5 = 6
```

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 942 | 6 |
| 17703 | 9 |


## Question 7 - Prime Example

### Question 7a
Write a  program that reads a positive integer number and prints "Prime" to the screen if the entered number is a Prime number, otherwise "Prime Not".

### Question 7b
Write a program which takes an integer as input and prints prime numbers up to that integer.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 11 | 2 3 5 7 11 |
| 15  | 2 3 5 7 11 13 |


## Question 8 - Prime factors

### Question 8a

Write a program that reads an integer N and prints all the numbers that can divide N.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 21  | 1 3 7 21 |
| 30  | 1 2 3 5 6 10 15 30 |

### Question 8b

Write a program that reads an integer N and prints the prime factoriation of N.

Hint: A non-prime number is always composed of prime numbers smaller than it.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 21  | 3 * 7   |
| 60  | 2 * 2 * 3 * 5  |

### Question 8c

Write a program that reads an integer N and prints the prime factorization of N in the form of exponents.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 21  | 3^1 * 7^1   |
| 60  | 2^2 * 3^1 * 5^1  |



## Question 9 - Pascal's Triangle

The entry in the nth row and kth column of Pascal's triangle is denoted C(n,k). For example, the entry in the topmost row is C(0,0)=1.
Write a program which takes positive integer n and prints the first n line of Pascal's Triangle. You can use math module to compute factorial. (import math and use math.factorial)

```
Input:
3

Output:
1 
1 1 
1 2 1 

Input:
8

Output:
1 
1 1 
1 2 1 
1 3 3 1 
1 4 6 4 1 
1 5 10 10 5 1 
1 6 15 20 15 6 1 
1 7 21 35 35 21 7 1 
```


## Question 10 - Half-Matrix

### Question 10a

Write a program which takes an integer N as input and prints the half matrix of N * N with its indices.
Indices increasing in the horizontal direction

```

Input:
3

Output:
0 
1 2 
3 4 5 

Input:
5

Output:

0
1 2 
3 4 5 
6 7 8 9 
10 11 12 13 14 

```

### Question 10b

Write a program which takes an integer N as input and prints the half matrix of N * N with its indices.
Indices increasing in the vertical direction

```

Input:
3

Output:
0 
1 3 
2 4 5 

Input:
5

Output:

0
1 5 
2 6 9 
3 7 10 12 
4 8 11 13 14 

```