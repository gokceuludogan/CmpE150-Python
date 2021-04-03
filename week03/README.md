# Variables / Expressions / Statements
continued..

## Question 1

Write a program which takes radius of a circle from user and calculate the perimeter and surface of the defined circle.

**You can get the value of pi from math module (from math import pi)**

| Input | Output                      |
| ----- | --------------------------- |
| 4     | 25.1327412287 50.2654824574 |
| 8     | 50.2654824574 201.06192983  |

<br>

## Question 2

Write a program that calculates the volume of a sphere by taking its radius from user.

| Input | Output        |
| ----- | ------------- |
| 3     | 113.097335529 |
| 6     | 904.778684234 |

<br>

## Question 3

Write a program that takes a positive number from user and calculate the sum from 0 to that positive number.

**You do not need to use any loops or developed coding**

| Input | Output |
| ----- | ------ |
| 10    | 55     |
| 5     | 15     |

<br>

## Question 4

Write a program which replaces the values of two integers.

| Input | Output |
| ----- | ------ |
| 5 10  | 10 5   |

<br>

## Question 5

Write a program which takes a lowercase letter as input and print the uppercase version of the given letter.

| Input | Output |
| ----- | ------ |
| a     | A      |
| b     | B      |

<br>

## Question 6

Write a program that takes 3 integers from the user and then prints the sum of odd numbers.

| INPUT  | OUTPUT |
| ------ | ------ |
| 3 4 5  | 8      |
| 2 2 4  | 0      |
| 1 9 15 | 25     |

<br>

## Question 7

There is a cash machine with an infinite supply of 5tl banknotes and 1tl coins inside it.

Write a program that takes an integer as input representing the amount of money requested by a customer. The program then prints the number of banknotes and coins given to the customer. (Machine must prefer giving away banknotes instead of coins if possible)

| INPUT  | OUTPUT |
| ------ | ------ |
| 57     | 11 2   |
| 269    | 53 4   |

<br>

## Question 8

 Guess the outcome of each statement. Then check the results.

<em> Hint: You can multiply strings with integers. It basically performs the concatenation operation n many times. </em>
<br>

* print(int('6') + int('4'))  <br>
* print('1' + '4')<br>
* print(int(3.9))
* print(str(5.3) + '2.7')<br>
* print(int('5') * str(0.6))<br>
* print(float('3' + '8.6'))<br>
* print(3.5 + 6.7)<br>
* print(2 ** 3 ** 2 / 32)
* print(str(4.4) + str(7.3))<br>
* print(int(6.5) + float('6.5'))<br>
* print(int(4.5 + 3.2))<br>
* print(int(3.2) + int(float(str(3.2))))<br>

<em> Remarks: </em>
<br>
<em>
 * Observe that float-to-int type conversion is not a rounding operation. int(3.9) = 3. To round floats, we will use a built-in function called round(). Stay tuned! <br>
 * As you see, we can multiply strings with integers, but not floats. What does 3.14 times "pi" mean, anyway?  <br>
 * Exponent operator ** has right-to-left associativity. <br>
</em>
<br>

## Question 9

We want to simulate a division operation. In order to do that, write a program to prompt the user for 2 integers, dividend and divisor respectively. Perform the division operation and print out the quotient and the remainder. 

| INPUT  | OUTPUT |
| ------ | ------ |
| 9 2 | quotient =  4  remainder =  1|
| 156 13  | quotient = 12  remainder = 0 |
| 84 16 | quotient = 5  remainder = 4  |

<br>

## Question 10

In mathematics and computer science, the [floor function](https://en.wikipedia.org/wiki/Floor_and_ceiling_functions) is the function that takes as input a real number <code>x</code>, and gives as output the greatest integer less than or equal to <code>x</code>, denoted as  `⌊x⌋`. The fractional part is the sawtooth function, denoted by  `{x}` for real x and defined by the formula `{x} = x - ⌊x⌋`. Write a function that takes 3 positive floats from the input and prints out the fractional part of each value respectively. Do not use float-to-int type casting. There might occur some [floating-point error](https://www.geeksforgeeks.org/floating-point-error-in-python/), you do not have to deal with that. <br>
<em> Hint: Integer division by 1 can be helpful to find </em>`⌊x⌋`<em>. Notice that for negative numbers, we have to perform extra steps to find </em>`⌊x⌋`.

| INPUT  | OUTPUT |
| ------ | ------ |
| 4.8 6.4 3.5|  0.8 0.4 0.5|
| 67.32 23.53 13.98 | 0.32 0.53 0.98 |
| 65.12 49.32 30.09 | 0.12 0.32 0.09 |

<br>

