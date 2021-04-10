## Question 1

Write a program which takes two integer and determines whether the first number is divisible by the second number. If it's not divisible, then the program prints the remainder of the division. 

| Input  | Output          |
| ------ | --------------- |
| 161 11 | Not divisible 7 |
| 121 11 | Divisible       |

## Question 2 

Write a program that takes 3 integers from the user and then prints the min and max of the numbers.

| Input    | Output           |
| -------- | ---------------- |
| 13 27 14 | 13 27 |

## Question 3
Write a program that calculates the body mass index with the given formula and print the appropriate class with the catalogue below.

<img src="https://render.githubusercontent.com/render/math?math=\large BMI= mass / height^{2}">


| Category                              | BMI     |
| ------------------------------------- | ------- |
| Very severely underweight             | -15     |
| Severely underweight                  | 15-16   |
| Underweight                           | 16-18.5 |
| Normal (healthy weight)               | 18.5-25 |
| Overweight                            | 25-30   |
| Obese Class I (Moderately obese)      | 30-35   |
| Obese Class II (Severely obese)       | 35-40   |
| Obese Class III (Very severely obese) | 40+     |

| Input  | Output                            |
| ------ | --------------------------------- |
| 83 174 | 28.7<br />Overweight              |
| 73 174 | 24.1<br />Normal (healthy weight) |

## Question 4
Write a program which calculates whether any given two numbers are multiples of one another.

| Input | Output       |
| ----- | ------------ |
| 2 4   | Multiple     |
| 4 2   | Multiple     |
| 5 3   | Not Multiple |

## Question 5

There is a cash machine with a finite (n) supply of 5tl banknotes and an infinite supply of 1tl coins inside it.

Write a program that takes two integers as input representing the amount of money requested by a customer and the number of 5tl banknotes inside the machine (n). The program should then print the number of banknotes and coins given to the customer. (Machine must prefer giving away banknotes instead of coins if possible)

| Input | Output |
| ----- | ------ |
| 38 4  | 4 18   |
| 30 5  | 5 5    |
| 14 3  | 2 4    |
| 2 5   | 0 2    |

## Question 6

### Question 6a

Write a program that takes 2 integers from the user and then prints these integeres in an ascending order using a single if statement.

| Input | Output |
| ----- | ------ |
| 3 5   | 3 5    |
| 5 3   | 3 5    |

### Question 6b

Write a program that takes 3 integers from the user and then prints these integeres in an ascending order

| Input | Output |
| ----- | ------ |
| 1 3 2 | 1 2 3  |
| 3 2 1 | 1 2 3  |
| 2 3 1 | 1 2 3  |

## Question 7

Consider a classic case of [prisonner's dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma).

Bob and Sam are being interrogated by police as suspects of a theft case. Interrogation process is taking place in two seperate rooms. They can either stay silent about their crime or betray each other by admiting it. The possible outcomes are:
- If Bob and Sam each betray the other, each of them serves two years in prison
- If Bob betrays Sam but Sam remains silent, Bob will be set free and Sam will serve three years in prison
- If Bob remains silent but Sam betrays Bob, Bob will serve three years in prison and Sam will be set free
- If Bob and Sam both remain silent, both of them will serve only one year in prison (on the lesser charge).

Write a program that takes decisions (silence/betrayal) of Bob and Sam as input, then outputs their punishments.

| Input             | Output |
| ----------------- | ------ |
| silence silence   | 1 1    |
| silence betrayal  | 3 0    |
| betrayal betrayal | 2 2    |

## Question 8 

 Write a program to prompt the user for 3 integers x, y and z. Print out true if these integer can constitute the side lengths of a right triangle, False otherwise. Apart from taking the inputs, you should use only one line of code.
 
<em> Hint: 
  * Sum of the squares of the two integers must be equal to the square of the other. 
  * Each integer must be positive.  
 </em>

| INPUT  | OUTPUT |
| ------ | ------ |
| 7 0 7  | False     |
| 9 -12 15   | False     |
| 20 12 16  | True     |

## Question 9

Write a program that takes an integer as an input that takes an integer in the range 0-9999 (inclusive) and prints the sum of this number's digits.

| INPUT  | OUTPUT |
| ------ | ------ |
| 15 | 6  |
| 1234 |  10 |
| 9999 | 36  |
| -5  | Input is not in the interval  |
| 0 | 0 |
| 10000  | Input is not in the interval |

## Question 10

Write a program that prints the physical state of the water for the given *(taken as input)* temperature. 
(Remember that in the phase change temperature, the matter can be in more than one state) 

Ex: in 100°C water can be liquid or gas

<em>(boiling point of water: 100°C and freezing point of water: 0°C )</em>

| INPUT  | OUTPUT |
| ------ | ------ |
| 142 | It is in the gas state. |
| 62 |  It is in the liquid state. |
| -81  | It is in the solid state. |
| 0  | It can be solid or liquid. |
| 100  | It can be liquid or gas. |
