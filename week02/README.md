## Question 1

Write a program which takes a float and prints **absolute value** of this float **without using abs() function**.

| Input | Output |
| ----- | ------ |
| 5.8   | 5.8    |
| -11.5 | 11.5   |

## Question 2

Write a program which takes two integers and determines **whether the first one is divisible by the second one.** If it's divisible, then the program prints **quotient** of the division; otherwise it prints **remainder** of the division. 

| Input  | Output |
| ------ | ------ |
| 161 11 | 7      |
| 30 6   | 5      |

## Question 3 

Write a program that takes 3 integers from the user and then prints **minimum** and **maximum** of these numbers.

| Input    | Output |
| -------- | ------ |
| 13 27 14 | 13 27  |

## Question 4

Write a program which takes an integer from user and then prints whether this integer is **divisible by 2, 3 and 5.** 

| Input | Output                                                 |
| ----- | ------------------------------------------------------ |
| 8     | Divisible by 2                                         |
| 30    | Divisible by 2<br />Divisible by 3<br />Divisible by 5 |

## Question 5

Write a program which takes the age of the user and give the appropriate output looking the table below.

| Age   | Group    |
| ----- | -------- |
| 0-17  | Child    |
| 18-64 | Can Work |
| 65+   | Retired  |

| Input | Output   |
| ----- | -------- |
| 15    | Child    |
| 28    | Can Work |
| 18    | Can Work |

**Don't forget to test your code on 18 and 65 as inputs.**

## Question 6

Write a program that determines whether a given year is a leap year or not.

- **Multiples of 4 are leap years**
- **Multiples of 100 are *not* leap years**
- **Multiples of 400 are leap years**

| Input | Output          |
| ----- | --------------- |
| 1600  | Leap year       |
| 1700  | Not a leap year |
| 2020  | Leap year       |

## Question 7

Write a program that computes the letter grade of a CMPE150 student with the aid of percentages and catalogue below:

| Type        | Percentage |
| ----------- | ---------- |
| Midterm     | 20         |
| Labs        | 10         |
| Assignments | 15         |
| Project     | 25         |
| Final       | 30         |

| Note   | Letter Grade |
| ------ | ------------ |
| 75-100 | A            |
| 55-75  | B            |
| 35-55  | C            |
| 0-35   | F            |

| Input             | Output |
| ----------------- | ------ |
| 100 100 100 90 80 | A      |
| 60 60 60 80 65    | B      |

## Question 8

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

## Question 9

Write a program which calculates whether any given two numbers are multiples of one another.

| Input | Output       |
| ----- | ------------ |
| 2 4   | Multiple     |
| 4 2   | Multiple     |
| 5 3   | Not Multiple |

## Question 10

Write a program which takes three floats as **a, b, c** and calculates **real roots** for a quadratic equation <img src="https://render.githubusercontent.com/render/math?math=\large ax^{2} %2B bx %2B c"> using the formula <img src="https://render.githubusercontent.com/render/math?math=\large x = -b \pm \sqrt{b^{2} - 4ac} /2a ">

The expression under the square root is known as **the discriminant.** 

* If the discriminant is **negative**, the roots are **imaginary.** 
* If the discriminant is **zero**, there is **only one root.** 
* If the discriminant is **positive**, there are **two roots.**

*Note: Ignore imaginary roots.*

| Input  | Output |
| ------ | ------ |
| 1 5 6  | -3 -2  |
| 1 -4 4 | 2      |

