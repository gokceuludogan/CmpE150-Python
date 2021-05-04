# Functions

## Question 1

Write a function called `power` that takes a required integer parameter as **number** and an optional integer parameter as **n**. The default value for **n** should be 2. The function should return the **nth** power of **number**.

| Input | Output |
| ----- | ------ |
| 5     | 25     |
| 3 2   | 9      |
| 4 3   | 64     |

## Question 2

Write a function which takes a number and prints the first 6 powers of the number using **power()** function from previous question. 

| Input | Output                                     |
| ----- | ------------------------------------------ |
| 2     | 2<br />4<br />8<br />16<br />32<br />64    |
| 3     | 3<br />9<br />27<br />81<br />243<br />729 |

## Question 3

An **abundant number** or **excessive number** is a **number** that is smaller than the sum of its proper divisors. 

Write a function which takes two integers and finds the abundant numbers between those numbers (including them). If there are abundant numbers in the range, the function prints these numbers; otherwise, prints no abundant number.  

**Example:** The integer 12 is the first **abundant number**. Its proper divisors are 1, 2, 3, 4 and 6 for a total of 16. The amount by which the sum exceeds the **number** is the **abundance**.

| Input | Output               |
| ----- | -------------------- |
| 20 35 | 20 24 30             |
| 10 40 | 12 18 20 24 30 36 40 |
| 3 10  | no abundant number   |

## Question 4 - Elementary Number Theory

### Question 4a - Modulus

Using only addition, subtraction and a ``while`` loop, write a function that takes two numbers ``A``, ``B`` and returns ``A % B``.

| Input | Output |
| ----- | ------ |
| 17 3 | 2 |
| 27 5 | 2 |
| 11 17 | 11 |

### Question 4b - GCD

The **greatest common divisor** or **GCD** of two integers is the largest number that divides both integers.

Write a function which takes two positive integers and returns their GCD. 

Hint: Implement [Euler's method](https://www.khanacademy.org/computing/computer-science/cryptography/modarithmetic/a/the-euclidean-algorithm).

| Input | Output |
| ----- | ------ |
| 2 5   | 1   |
| 12 8  | 4 |
| 8 9   | 1   |
| 15 30 | 15 |

### Question 4c - LCM

The **lowest common multiple** or **LCM** of two integers is the smallest number that is a multiple of both numbers

Write a function which takes two positive integers and returns their LCM.

Hint: GCD(a,b) * LCM(a,b) = a*b

| Input | Output |
| ----- | ------ |
| 2 5   | 10   |
| 12 8  | 24 |
| 8 9   | 72   |
| 15 30 | 30 |

## Question 5 - Think

Write a function that takes an integer and thinks that much. Default value is 1.

| Input | Output |
| ----- | ------ |
| think()  |  hm  |
| think(2)  | hmm |
| think(5)   | hmmmmm |

## Question 6 - You're a Square!
When you multiply a number by itself, the result is a square number.

Write a function that takes an integer and determines whether it is a square number or not.

| Input | Output |
| ----- | ------ |
| 25  |  True  |
| 23  | False |
| 0 | True |
|-1 | False|

## Question 7

Write a floor function. If the input is anything other than integer or float, print a warning to the console that the input is invalid.

| PARAMETER | RETURN |
| - | - |
| 123 | 123 |
| 123.7 | 123 |
| Hi! | Invalid input: Hi! |

<em>Hint: You can use type(var) function to get the type of var</em>


## Question 8 - Points


#### Question 8a - Distance

Write a function  **distance** which takes the coordinates of two points (x1, y1, x2, y2) and returns Euclidian distance between these points.

| Input           | Output |
| --------------- | ------ |
| 3, 0, 0, 4   | 5.0    |
| 5, 8, 10, 20 | 13.0   |


#### Question 8b - Closest

Write a function which takes the coordinates of two points (x1, y1, x2, y2)  and returns the point closest to the origin. *Use the distance
function.*

| Input          | Output |
| -------------- | ------ |
| 3, 0, 0, 4  | 3, 0 |
| 11, 7, 6, 8 | 6, 8 |

#### Question 8c - Valid Triangle

Write a function that takes three vertices of a triangle (x1, y1, x2, y2, x3, y3), and returns True if it is a valid triangle, False otherwise. If the distance between any two points is zero, raise ZeroDivisionError.

| Input          | Output |
| -------------- | ------ |
| 3, 0, 0, 4, 1, 1  | True |
| 11, 7, 6, 8, 11, 7| ZeroDivisionError |
| 0, 0, 0, 1, 0, 2 | False |

#### Question 8d - Perimeter

Write a function that takes three vertices of a triangle (x1, y1, x2, y2, x3, y3), and returns the perimeter (sum of edges). If the distance between any two points is zero, raise ZeroDivisionError. If the triangle is invalid, raise ValueError. 

| Input          | Output |
| -------------- | ------ |
| 3, 0, 0, 4, 1, 1  | 10.39834563766817 |
| 11, 7, 6, 8, 11, 7| ZeroDivisionError |
| 0, 0, 0, 1, 0, 2 | ValueError |

#### Question 8e - Area

Write a function that takes three vertices of a triangle (x1, y1, x2, y2, x3, y3), and returns the area. If the distance between any two points is zero, return -1. If the triangle is invalid, return 0. 

| Input          | Output |
| -------------- | ------ |
| 3, 0, 0, 4, 1, 1  | 2.5 |
| 11, 7, 6, 8, 11, 7| -1 |
| 0, 0, 0, 1, 0, 2 | 0 |


#### Question 8f - Point in Triangle

Write a function that takes three vertices of a triangle (x1, y1, x2, y2, x3, y3), and coordinates of a point. Return True if the point is inside the triangle, False otherwise. 

| Input          | Output |
| -------------- | ------ |
| -3, 5, 9, 1, -6, -7, -2, 0  | True |
| -3, 5, 9, 1, -6, -7, 9, 1| True |
| -3, 5, 9, 1, -6, -7, 12, 1 | False |



