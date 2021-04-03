# Variables / Expressions / Statements

## Q1.a

```python
number1 = 13
number2 = 5

# Printing numbers in separate lines
print(number1)
print(number2)

# Printing numbers in a single line
print(number1, number2)
```

## Q1.b

```python
number1 = int(input())
number2 = int(input())

print(number1)
print(number2)
```

## Q1.c

```python
a = int(input())
b = int(input())

print(a + b, a - b, a * b, a ** b, a % b)
```

## Q2.a

```python
number = 5
my_float = 9.8
my_str = "Helloo"

print(type(number))
print(type(my_float))
print(type(my_str))
```

<br>

## Q2.b

```python
number = int(input("Enter an integer: "))
my_float = float(input("Enter a float "))
my_str = input("Please enter third number: ")

print(number, my_float, my_str)
# Same print with + operator (concatenation of strings))
print(str(number) +  " " + str(my_float) + " " + my_str)
```

<br>



## Q3
```python
number1 = int(input("First number: "))
number2 = int(input("Second number: "))
number3 = int(input("Third number: "))

sum = number1 + number2 + number3

print(sum)
print(sum / 3)
print(number1 * number2 * number3)
```

<br>

## Q4
```python
A = int(input("Enter principal amount: "))
i = int(input("Enter interest rate: "))
n = int(input("Enter duration: "))

S = A * (1 + i/100) ** n

print("{:.2f}".format(S))
```

<br>

## Q5
```python
r1 = int(input("First resistance: "))
r2 = int(input("Second resistance: "))

v = int(input("Voltage: "))

print(int(v / r1), int(v / r2))

```

<br>

## Q6
```python
y = int(input("Year: "))
m = int(input("Month: "))
d = int(input("Days: "))
h = int(input("Hours: "))
min = int(input("Minutes: "))

y = y * 365 * 24 * 60 * 60
m = m * 30 * 24 * 60 * 60
d = d * 24 * 60 * 60
h = h * 60 * 60
min = min * 60

sum = y + m + d + h + min

print(sum)
```

Alternative:

```python
y = int(input("Year: "))
m = int(input("Month: "))
d = int(input("Days: "))
h = int(input("Hours: "))
min = int(input("Minutes: "))

sum = (((y * 365 + m * 30 + d) * 24 + h) * 60 + min) * 60

print(sum)
```

<br>
