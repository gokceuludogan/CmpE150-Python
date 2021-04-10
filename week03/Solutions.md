# Variables / Expressions / Statements

You may clean strings in input and print functions.

## Q1
```python
from math import pi

r = int(input("Plese enter a radius: "))

print("The perimeter of the circle with given radius is: " + str(2*pi*r))
print("The surface of the circle with given radius is: " + str(pi*r**2))
```

<br>

## Q2
```python
import math

r = int(input("Plese enter a radius: "))

print("The volume of the sphere with the given radius is: " + str(4.0/3*math.pi*math.pow(r,3)))
```

<br>

## Q3
```python
n = int(input("Plese enter a number: "))

print("The sum till the given number is: " + str((n*(n+1))/2))

```

<br>

## Q4
```python
a = int(input("Plese enter the first number: "))
b = int(input("Plese enter the second number: "))

# Version 0 (Easy Swap):
original_a = a
original_b = b
a = original_b
b = original_a

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

## Q5
```python
ll = input("Plese enter a lowercase letter: ")

ul = chr(ord(ll) + ord("A") - ord("a"))

print("Here is the upparcase version: " + ul)

# Built-in function
# print(ll.upper())
```

<br>


## Q6
```python
a = int(input("Please enter the first number: "))
b = int(input("Please enter the second number: "))
c = int(input("Please enter the third number: "))

print(a * (a % 2) + b * (b % 2) + c * (c % 2))
```

<br>

## Q7
```python
amount = int(input("Please enter the amount of  money requested by the customer: "))

print("Number of 5tl banknotes: %d" % (amount//5))
print("Number of 1tl coins: %d" % (amount%5))
```

<br>

## Q8

```python
 print(int('6') + int('4'))               10 
 print('1' + '4')                         14
 print(int(3.9))                          3
 print(str(5.3) + '2.7')                  5.32.7 
 print(int('5') * str(0.6))               0.60.60.60.60.6
 print(float('3' + '8.6'))                38.6 
 print(3.5 + 6.7)                         10.2 
 print(2 ** 3 ** 2 / 32)                  16.0  
 print(str(4.4) + str(7.3))               4.47.3 
 print(int(6.5) + float('6.5'))           12.5 
 print(int(4.5 + 3.2))                    7
 print(int(3.2) + int(float(str(3.2))))   6 
```

<br>

## Q9
```python
dividend = int(input())
divisor = int(input())

quotient = dividend // divisor
remainder = dividend % divisor
# remainder = dividend - (quotient * divisor)

print("quotient =", str(quotient), "remainder =", str(remainder))
```

<br>

## Q10
```python
a = float(input())
b = float(input())
c = float(input())

floor_a = a // 1
floor_b = b // 1
floor_c = c // 1

fraction_a = a - floor_a
fraction_b = b - floor_b
fraction_c = c - floor_c

# print(str(fraction_a), str(fraction_b), str(fraction_c))
print("%.2f %.2f %.2f" % (fraction_a, fraction_b, fraction_c))

```

<br>
