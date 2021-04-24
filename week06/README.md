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


## Question 4 - Sum Facts

Write a program which takes an integer as input and computes the sum of the factorial of each digit.  For example, assume that the user enters 572 as the input. For each digit of the integer, you will compute the factorial. Then you will compute the sum of these factorials: 5! + 7! + 2! = 120 + 5040 + 2 = 5162.

| Input | Output |
| ----- | ------ |
| 572   | 5162   |
| 27    | 5042   |


## Question 5 - Prime Example

### Question 5a
Write a  program that reads a positive integer number and prints "Prime" to the screen if the entered number is a Prime number, otherwise "Prime Not".

### Question 5b
Write a program which takes an integer as input and prints prime numbers up to that integer.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 11 | 2 3 5 7 11 |
| 15  | 2 3 5 7 11 13 |


## Question 6 - Prime factors

### Question 6a

Write a program that reads an integer N and prints all the numbers that can divide N.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 21  | 1 3 7 21 |
| 30  | 1 2 3 5 6 10 15 30 |

### Question 6b

Write a program that reads an integer N and prints the prime factoriation of N.

Hint: A non-prime number is always composed of prime numbers smaller than it.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 21  | 3 * 7   |
| 60  | 2 * 2 * 3 * 5  |

### Question 6c

Write a program that reads an integer N and prints the prime factorization of N in the form of exponents.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 21  | 3^1 * 7^1   |
| 60  | 2^2 * 3^1 * 5^1  |

## Question 7 - Zzz

Write a program which takes positive integer n greater than 2 and prints letter 'Z' size of n using '*'.

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


## Question 8 - Half-Matrix

### Question 8a

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

### Question 8b

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

## Question 9 - Sore Loser Bob

Bob and Sam are playing a game. They are creating random integers (between 0 and 10) and whoever gets the higher integer gets 1 point. Whoever gains X points wins the game (X will be taken from the user). However, Bob doesn't like lossing so they play the same game until Bob wins.

Write a program that simulates the game and find out how many times Bob and Sam have to replay the game until Bob wins.

|  INPUT  |  OUTPUT |
|:-------:|:-------:|
| 45  | Bob was able to win after 4 iterations!   |
| 12  | Bob was able to win after 1 iterations!  |

<em>Hint: You can use randint to create random numbers.</em>
</br>
<em>Note: The outputs in the examples may vary, since each time the program runs, numbers are generated randomly.</em>


## Question 10 - Palindromic Primes
Palindromic number is a number that remains the same when its digits are reversed. A [palindromic prime](https://en.wikipedia.org/wiki/Palindromic_prime) is a prime number that is also a palindromic number. Write a program that prompts the user for two integers, starting and ending points. Then print out all the palindromic primes between starting and ending points inclusively.


|  INPUT | OUTPUT |
| :------: | :------: |
| 10 150| 11 101 131 |
| 150 350 | 151 181 191 313 |
| 700 800 | 727 757 787 797 |

## Question 11 - Draw a figure
Take an integer from the user as the size, and draw this figure below with the given size in a single nested loop. This figure is an example with size 6 (Height is 6x2=12).
<pre> 
  \     |     / 
   \    |    /  
    \   |   /    
     \  |  /     
      \ | /      
       \|/       
       /|\       
      / | \      
     /  |  \     
    /   |   \    
   /    |    \   
  /     |     \  
 </pre>


      
