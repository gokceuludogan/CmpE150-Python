# Variables / Expressions / Statements

## Q1

```python
num1 = int(input("Please enter first number: "))
num2 = int(input("Please enter second number: "))
num3 = int(input("Please enter third number: "))

print("Sum is: " + str(num1+num2+num3))
print("Mean is: %.2f" % ((num1+num2+num3)/3))
print("Multiple is: %d" % (num1*num2*num3))
```

<br>

## Q2
```python
A = int(input("Plese enter the principal amount: "))
i = int(input("Plese enter the interest rate per month: "))
n = int(input("Plese enter the duration in months: "))

print("Final amount is: " + str(A*(1+i/100)**n))
```

<br>

## Q3
```python
from math import pi

r = int(input("Plese enter a radius: "))

print("The perimeter of the circle with given radius is: " + str(2*pi*r))
print("The surface of the circle with given radius is: " + str(pi*r**2))
```

<br>

## Q4
```python
n = int(input("Plese enter a number: "))

print("The sum till the given number is: " + str((n*(n+1))/2))

```

<br>

## Q5
```python
r1 = int(input("Plese enter the value of first resistance in OHMs: "))
r2 = int(input("Plese enter the value of first resistance in OHMs: "))
v = int(input("Plese enter the value of tension voltage in volts: "))

print("The current in R1 is: " + str(v/r1))
print("The current in R2 is: " + str(v/r2))
```

<br>

## Q6
```python
a = int(input("Plese enter the first number: "))
b = int(input("Plese enter the second number: "))

# Version 1 (Classic Swap):
temp = a
a = b
b = temp

# Version 2 (Without using extra variable):
# a = a + b
# b = a - b
# a = a - b

# Version 3 (Python Variation):
# a, b = b, a

print("Here they are inversed: " + str(a) + " " + str(b))
```

<br>

## Q7
```python
ch = (input("Enter a character: "))

print("The ascii value of " + ch + " is: " + str(ord(ch)))
```

<br>

## Q8
```python
ll = input("Plese enter a lowercase letter: ")

ul = chr(ord(ll) + ord("A") - ord("a"))

print("Here is the upparcase version: " + ul)
```

<br>

## Q9
```python
import math

r = int(input("Plese enter a radius: "))

print("The volume of the sphere with the given radius is: " + str(4.0/3*math.pi*math.pow(r,3)))
```

<br>

## Q10
```python
y = int(input("Plese enter the amount of years: "))
mo = int(input("Plese enter the amount of months: "))
d = int(input("Plese enter the amount of days: "))
h = int(input("Plese enter the amount of hours: "))
mi = int(input("Plese enter the amount of minutes: "))

summ = 0

summ += y * 365 * 24 * 60 * 60
summ += mo * 30 * 24 * 60 * 60
summ += d * 24 * 60 * 60
summ += h * 60 * 60
summ += mi * 60

print("Given duration is: " + str(summ)+" seconds.")
```

<br>

## Q11
```python
a = int(input("Please enter the first number: "))
b = int(input("Please enter the second number: "))
c = int(input("Please enter the third number: "))

print(a * (a % 2) + b * (b % 2) + c * (c % 2))
```
