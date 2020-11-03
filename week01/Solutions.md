# Variables / Expressions / Statements

## Q1

```python
num1 = int(input("Please enter first number: "))
num2 = int(input("Please enter second number: "))
num3 = int(input("Please enter third number: "))

print("Sum is: " + str(num1+num2+num3))
print("Mean is: " + str((num1+num2+num3)/3))
print("Multiple is: " + str(num1*num2*num3))
```

## Q2
```python
A = int(input("Plese enter the principal amount: "))
i = int(input("Plese enter the interest rate per month: "))
n = int(input("Plese enter the duration in months: "))

print("Final amount is: " + str(A*(1+i/100)**n))
```

## Q3
```python
import math

r = int(input("Plese enter a radius: "))

print("The perimeter of the circle with given radius is: " + str(2*math.pi*r))
print("The surface of the circle with given radius is: " + str(math.pi*r**2))
```

## Q4
```python
n = int(input("Plese enter a number: "))

print("The sum till the given number is: " + str((n*(n+1))/2))

```

## Q5
```python
r1 = int(input("Plese enter the value of first resistance in OHMs: "))
r2 = int(input("Plese enter the value of first resistance in OHMs: "))
v = int(input("Plese enter the value of tension voltage in volts: "))

print("The current in R1 is: " + str(v/r1))
print("The current in R2 is: " + str(v/r2))
```

## Q6
```python
a = int(input("Plese enter the first number: "))
b = int(input("Plese enter the second number: "))

a = a + b
b = a - b
a = a - b

print("Here they are inversed: " + str(a) + " " + str(b))
```

## Q7
```python
ch = (input("Enter a character: "))

print("The ascii value of " + ch + " is: " + str(ord(ch)))
```

## Q8
```python
ll = input("Plese enter a lowercase letter: ")

ul = chr(ord(ll) + ord("A") - ord("a"))

print("Here is the upparcase version: " + ul)
```

## Q9
```python
import math

r = int(input("Plese enter a radius: "))

print("The volume of the sphere with the given radius is: " + str(4.0/3*math.pi*math.pow(r,3)))
```

## Q10
```python
y = int(input("Plese enter the amount of years: "))
mo = int(input("Plese enter the amount of months: "))
d = int(input("Plese enter the amount of days: "))
h = int(input("Plese enter the amount of hours: "))
mi = int(input("Plese enter the amount of minutes: "))

print("Given duration is: " + str(y*31556926+mo*2629743.83+d*86400+h*3600+mi*60 )+" seconds.")
```


## Q11
```python
a = int(input("Please enter the first number: "))
b = int(input("Please enter the second number: "))
c = int(input("Please enter the third number: "))

print(a * (a % 2) + b * (b % 2) + c * (c % 2))
```

















