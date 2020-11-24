# Loops

## Question 1 - Staaaars

### Question 1a

```python
print('*')
```

### Question 1b

```python
print('**********')
```

### Question 1c

```python
N = int(input())

for i in range(N):
    print('*')
```

### Question 1d

```python
N = int(input())

for i in range(N):
    print('*', end='')
```


## Question 2 - Numbeeeers

```python
N = int(input())

for i in range(N):
    print(i+1, end=' ')

# OR

for i in range(1, N+1):
    print(i, end=' ')
```


## Question 3 - Hooping Numbers

### Question 3a

```python
A = int(input("A: "))
B = int(input("B: "))
t = int(input("t: "))

for i in range(A, B+1, t):
    print(i, end=' ')
```


### Question 3b

```python
A = int(input("A: "))
B = int(input("B: "))
t = int(input("t: "))

for i in range(B, A-1, -t):
    print(i, end=' ')
```


## Question 4 - Even Numbeeeers

```python
A = int(input("A: "))
B = int(input("B: "))

result = 0

for i in range(A+1, B):
    if i % 2 == 0:
        result += i

print(result)
```


## Question 5 - Average Team

```python
N = int(input("N: "))

result = 0

for _ in range(N):
    x = int(input())
    result += x

print(result/N)
```


## Question 6 - Boom Boom POW

```python
a = int(input("a: "))
b = int(input("b: "))

result = 1

for _ in range(b):
    result *= a

print(result)

```

## Question 7 Factorial

```python
n = int(input())

resultFor = 1
resultWhile = 1
for i in range(n):
    resultFor *= i+1

while n:
    resultWhile *= n
    n -= 1

print(resultFor)
print(resultWhile)

```

## Question 8 - Fibonacci

```python
N = int(input("N: "))

prev = 0
curr = 1

for _ in range(3, N+1):
    next = prev + curr
    prev = curr
    curr = next

if N <= 0:
    print("Invalid!")
elif N == 1:
    print(prev)
else:
    print(curr)
```

### Question 9 - Second Largest

```python
x = int(input())
largest = 0
second = 0
    
while x != 0:
    if x > largest:
        second = largest
        largest = x
    elif x > second:
        second = x
    x = int(input())
            
print(largest-second)
```

## Question 10 - Digiiiits

```python
x = int(input())

count = 0
even_sum = 0

while x > 0:
    digit = x % 10
    if digit % 2 == 0:
        even_sum += digit
    count += 1

    x //= 10

print(count, even_sum)
```

## Question 11 - Positive Mental Attitude

```python
odd_sum = 0

x = int(input())
while x >= 0:
    if x % 2 == 1:
        odd_sum += x
    x = int(input())

print(odd_sum)
```

## Question 12 - NoBig

```python
total_sum = 0
count = 1

x = int(input())
y = int(input())
total_sum += x
while y <= x:
    total_sum += y
    count += 1

    x = y
    y = int(input())

print(total_sum/count)
```


## Question 13 - Guess

```python
import random

number = random.randint(1,100)
count = 0

while True:
    guess = input("Make your guess: ")
    guess = int(guess)
    count += 1
    
    if guess < number:
        print("Too low!")
    elif guess > number:
        print("Too high!")
    else:
        print("You got it!")
        print("And it only took you",count,"tries!")
        break
```

## Question 14 - Basic Calculator

```python
help = """q for quit
h for help
+ for addition
- for subtraction
* for multiplication
/ for integer division"""
print(help)
number = int(input("Please enter number: "))
operation = input("Please enter operation: ").lower()

while operation != "q":
    if operation == "+":
        second_number = int(input("Enter another number: "))
        number += second_number
    elif operation == "-":
        second_number = int(input("Enter another number: "))
        number -= second_number
    elif operation == "*":
        second_number = int(input("Enter another number: "))
        number *=  second_number
    elif operation == "/":
        second_number = int(input("Enter another number: "))
        if second_number == 0:
            print("Can't divide by 0")
        else:
            number //= second_number
    elif operation == "h":
        print(help)
    else:
        print("Operation is invalid!")
    print("Number is {} now".format(number))
    operation = input("Enter another operation (h for help): ").lower()

```
