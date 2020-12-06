# Q1

```python
def is_leap_year(year):
    if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
        return True
    else:
        return False
leap = is_leap_year(1904)    
if leap:
    print('leap year')
else:
    print('not a leap year')
```

# Q2

```python
def calculate_cost(cost, is_student):
    if is_student:
        cost /= 2
    return cost
print(calculate_cost(10, True))
```

# Q3

## a

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

## b 

```python
def print_powers(number):
    for i in range(6):
        print(power(number, i+1)) 
print_powers(3)   
```

# Q4

```python
def is_prime(number):
    for i in range(2, number):
        if number % i == 0:
            return False
    return True
print(is_prime(7))
print(is_prime(12))
```

# Q5

```python
def is_super(number):
    for i in range(2, number):
        if number % i == 0 and not is_prime(i): 
            return False
    return True

res = is_super(15)
if res:
    print('Suuuper')
else:
    print(':(')
```

# Q6

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

# Q7

```python
def is_relatively_prime(a, b):
    isrltprime = True
        
    for i in range(2,a+1):
        if a % i == 0 and b % i == 0:
            isrltprime = False
                
    if isrltprime:
        print("Relatively Prime")
    else:
        print("Not Relatively Prime")

is_relatively_prime(2, 5)
is_relatively_prime(12, 8)
```

# Q8

## a

```python
def modulus(a, b):
    while a > b:
        a -= b
    return a

print(modulus(17, 3))
print(modulus(27, 5))
```

## b & c

```python
def gcd(a, b):
    if a < b:
  		a, b = b, a
    while b != 0:
        mod = a % b
        a, b = b, mod
    return a

def lcm(a, b):
    return a * b // gcd(a, b)

print(gcd(2, 5))  # 1
print(gcd(12, 8))  # 4

print(lcm(2, 5))  # 10
print(lcm(12, 8))  # 24
```

# Q9

```python
def is_square(n):
    if n >= 0:
        root = n ** (1 / 2)
        if root == int(root):
            return True
        else:
            return False
    return False   
```

# Q10

```python
def multiply(*args):
    result = 1
    for i in args:
        result *= i
    return result

print(multiply(42,96))   
```

