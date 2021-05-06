## Question 1

```python
def power(number, n=2):
    result = 1
    for i in range(n):
        result *= number
    return result
print(power(5))
print(power(3, 2))
print(power(4, 3))
```


## Question 2

```python
def print_powers(number):
    for i in range(6):
        print(power(number, i+1)) 
print_powers(3)        
```


## Question 3

```python
def abundant_number(number):
    sum_divisors = 0
    for i in range(1, number):
        if number % i == 0:
            sum_divisors += i
    if sum_divisors > number:
        return True
    else:
        return False
    
def numbers_in_range(lower, upper):
    flag = 1
    for i in range(lower, upper + 1):
        if abundant_number(i):
            flag = 0
            print(i, end=' ')
    if flag: 
        print('no abundant number')
        
numbers_in_range(3, 10)        
numbers_in_range(10, 40)  
```


## Question 4

### Question 4a

```python
def modulus(a, b):
    while a > b:
        a -= b
    return a

print(modulus(17, 3))
print(modulus(27, 5))
```

### Question 4b and 4c

```python
def gcd(a, b):
    if a < b:
        temp = a
        a = b
        b = temp
    while b != 0:
        mod = a % b #  You may use modulus function
        a = b
        b = mod
    return a

def lcm(a, b):
    return a * b // gcd(a, b)

print(gcd(2, 5))  # 1
print(gcd(12, 8))  # 4

print(lcm(2, 5))  # 10
print(lcm(12, 8))  # 24
```


## Question 5 Think

```python
def think(size=1):
    thought = "h"
    if size > 0:
        thought += "m"*size
    return thought

print(think(5))

#  OR
def think(n=1):
    print("h" + "m" * n)
```


## Question 6 You're a Square!

```python
def square(n):
    if n < 0:
        return False
    if n == 0:
        return True
    for i in range(1, n + 1):
        if i ** 2 == n:
            return True
    return False
    

n = int(input())
print(square(n))
```


## Question 7

```python
def floor(n):
    try:
        n = int(n)
        return n
    except:
        try:
            n = float(n)
            return n
        except:
            print("Invalid input:", n)


n = input()
result = floor(n)
print(result, type(result))
```


## Question 8

### Question 8a - Distance

```python
def distance(x1, y1, x2, y2):
    return sqrt((x1 - x2) ** 2 + (y1 - y2) ** 2)
```


### Question 8b - Closest

```python
def closest(x1, y1, x2, y2):
    d1 = distance(0, 0, x1, y1)
    d2 = distance(0, 0, x2, y2)

    if d1 < d2:
        print(x1, y1)
    elif d1 == d2:
        print("Equal distance")
    else:
        print(x2, y2)
```

### Question 8c - Valid Triangle

```python
def valid_triangle(x1, y1, x2, y2, x3, y3):
    d1 = distance(x1, y1, x2, y2)
    d2 = distance(x1, y1, x3, y3)
    d3 = distance(x2, y2, x3, y3)

    if d1 == 0 or d2 == 0 or d3 == 0:
        raise ZeroDivisionError

    if d1 >= d2 + d3 or d2 >= d1 + d3 or d3 >= d1 + d2:
        return False
    return True
```

### Question 8d - Perimeter

```python
def perimeter(x1, y1, x2, y2, x3, y3):
    d1 = distance(x1, y1, x2, y2)
    d2 = distance(x1, y1, x3, y3)
    d3 = distance(x2, y2, x3, y3)

    if d1 == 0 or d2 == 0 or d3 == 0:
        raise ZeroDivisionError

    if d1 >= d2 + d3 or d2 >= d1 + d3 or d3 >= d1 + d2:
        raise ValueError

    return d1 + d2 + d3
```


### Question 8e - Area

```python
def area(x1, y1, x2, y2, x3, y3):
    try:
        if valid_triangle(x1, y1, x2, y2, x3, y3):
            return 0.5 * abs((x1 * y2 + x2 * y3 + x3 * y1) - (y1 * x2 + y2 * x3 + y3 * x1))
        return 0
    except ZeroDivisionError:
        return -1
```

### Question 8f - Point in Triangle

```python
def point_inside_triangle(x1, y1, x2, y2, x3, y3, m, n):
    at = area(x1, y1, x2, y2, x3, y3)
    a1 = area(x1, y1, x2, y2, m, n)
    a2 = area(x1, y1, m, n, x3, y3)
    a3 = area(m, n, x2, y2, x3, y3)

    if a1 == -1:
        a1 = 0
    if a2 == -1:
        a2 = 0
    if a3 == -1:
        a3 = 0

    if at == a1 + a2 + a3:
        return True
    return False
```
