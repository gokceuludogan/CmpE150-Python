## Question 1 - Leap year

A leap year in the Gregorian calendar system is a year that’s divisible by 4 but not by 100, unless it is also divisible by 400. Write a function that takes in a year as input and returns True or False indicating whether it’s a leap year (or not). For example, 1896, 1904, and 2000 were leap years but 1900 was not. Then, call this function with following inputs and print corresponding outputs depending on the function's result. 

| Input | Output          |
| ----- | --------------- |
| 1904  | leap year       |
| 1900  | not a leap year |
| 2000  | leap year       |

## Question 2 - Discount

Suppose you are purchasing a premium membership for a digital music service. If you are a student,  you get a 50% discount.

Write a function that takes as input the membership cost that you are purchasing and a Boolean variable indicating whether you are a student (or not), applies the discounts appropriately, and returns the final discounted value of the item.

| Input    | Output |
| -------- | ------ |
| 10 True  | 5      |
| 10 False | 10     |

## Question 3 - Power

###  Question 3a 

Write a function called `power` that takes a required integer parameter as **number** and an optional integer parameter as **n**. The default value for **n** should be 2. The function should return the **nth** power of **number**.

| Input | Output |
| ----- | ------ |
| 5     | 25     |
| 3 2   | 9      |
| 4 3   | 64     |

### Question 3b 

Write a function which takes a number and prints the first 6 powers of the number using **power()** function from previous question. 

| Input | Output                                     |
| ----- | ------------------------------------------ |
| 2     | 2<br />4<br />8<br />16<br />32<br />64    |
| 3     | 3<br />9<br />27<br />81<br />243<br />729 |

## Question 4 - Is Prime?

Write a function called `is_prime` which takes a number as a parameter and returns True or False indicating whether this number is prime or not. 

| Input | Output |
| ----- | ------ |
| 7     | True   |
| 12    | False  |

## Question 5 - Suuuper Number

**A suuuper number** is a number whose all divisors are prime except 1. 

Write a function called `is_super` which takes a number as a parameter and prints whether this number is suuuper or not. 

**Example**: 15 is a suuuper number since its divisors except 1 (3 and 5) are prime. However, 12 is not a suuuper number since it is divisible by 4 and 6 and those are not prime.

| Input | Output  |
| ----- | ------- |
| 15    | Suuuper |
| 12    | :(      |

## Question 6 - Abundant Number

An **abundant number** or **excessive number** is a **number** that is smaller than the sum of its proper divisors. 

Write a function which takes two integers and finds the abundant numbers between those numbers (including them). If there are abundant numbers in the range, the function prints these numbers; otherwise, prints no abundant number.  

**Example:** The integer 12 is the first **abundant number**. Its proper divisors are 1, 2, 3, 4 and 6 for a total of 16. The amount by which the sum exceeds the **number** is the **abundance**.

| Input | Output               |
| ----- | -------------------- |
| 20 35 | 20 24 30             |
| 10 40 | 12 18 20 24 30 36 40 |
| 3 10  | no abundant number   |


## Question 7 - Relatively Prime

Two integers are relatively prime if they have no common positive divisor except 1.

Write a function which takes two positive integers and prints "Relatively Prime" if they are relatively prime numbers, otherwise prints "Not Relatively Prime".

| Input | Output               |
| ----- | -------------------- |
| 2 5   | Relatively Prime     |
| 12 8  | Not Relatively Prime |
| 8 9   | Relatively Prime     |
| 15 30 | Not Relatively Prime |

## Question 8 - Elementary Number Theory

### Question 8a - Modulus

Using only addition, subtraction and a ``while`` loop, write a function that takes two numbers ``A``, ``B`` and returns ``A % B``.

| Input | Output |
| ----- | ------ |
| 17 3  | 2      |
| 27 5  | 2      |
| 11 17 | 11     |

### Question 8b - GCD

The **greatest common divisor** or **GCD** of two integers is the largest number that divides both integers.

Write a function which takes two positive integers and returns their GCD. 

Hint: Implement [Euler's method](https://www.khanacademy.org/computing/computer-science/cryptography/modarithmetic/a/the-euclidean-algorithm).

| Input | Output |
| ----- | ------ |
| 2 5   | 1      |
| 12 8  | 4      |
| 8 9   | 1      |
| 15 30 | 15     |

### Question 8c - LCM

The **lowest common multiple** or **LCM** of two integers is the smallest number that is a multiple of both numbers

Write a function which takes two positive integers and returns their LCM.

Hint: GCD(a,b) * LCM(a,b) = a*b

| Input | Output |
| ----- | ------ |
| 2 5   | 10     |
| 12 8  | 24     |
| 8 9   | 72     |
| 15 30 | 30     |

## Question 9 - You're a Square!
When you multiply a number by itself, the result is a square number.

Write a function that takes an integer and determines whether it is a square number or not.

| Input | Output |
| ----- | ------ |
| 25    | True   |
| 23    | False  |
| 0     | True   |
| -1    | False  |

## Question 10 - Multiply

Write a function that takes variable number of integers and returns multiply of them.

| Input           | Output |
| --------------- | ------ |
| multiply(2,5,3) | 30     |
| multiply(7,2)   | 14     |
| multiply(7)     | 7      |
| multiply(42,96) | 4032   |


