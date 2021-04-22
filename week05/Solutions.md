## Question 1 - Numbeeeers

```python
N = int(input())
K = int(input())

while N <= K:
    print(N, end=" ")
    N = N + 1

# OR

for i in range(N, K+1):
    print(i, end=' ')
```


## Question 2 - Hooping Numbers

```python
A = int(input("A: "))
B = int(input("B: "))
T = int(input("T: "))

while A <= B:
    print(A, end=" ")
    A = A + T

# OR

for i in range(A, B+1, T):
    print(i, end=' ')
```


## Question 3 - Even Numbeeeers

```python
A = int(input("A: "))
B = int(input("B: "))

result = 0

for i in range(A, B + 1):
    if i % 2 == 0:
        result += i
        
print(result)

# OR

summation = 0

while A <= B:
    if A % 2 == 0:
        summation = summation + A
    A = A + 1

print(summation)
```

## Question 4 - Average Team

```python
N = int(input("N: "))

result = 0

for _ in range(N):
    x = int(input())
    result += x

print(result/N)

# OR

index = 0
summation = 0

while index < N:
    a = int(input())
    summation = summation + a
    index = index + 1

print(summation / N)
```


## Question 5 - Boom Boom POW

```python
a = int(input("a: "))
b = int(input("b: "))

result = 1

for _ in range(b):
    result *= a

print(result)

# OR

power = 1
index = 0

while index < b:
    power = power * a
    index = index + 1

print(power)
```


## Question 6 - Fibonacci

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
    
# OR

"""
     F_x_2 + F_x_1 = F_x
F_0: 0
F_1: 1
F_2: 0 + 1 = 1
F_3: 1 + 1 = 2
F_4: 1 + 2 = 3
F_5: 2 + 3 = 5
F_6: 3 + 5 = 8
F_7: 5 + 8 = 13

0 1 1 2 3 5 8 13
"""

n = int(input()) - 1

if n == 0:
    print(0)
elif n == 1:
    print(1)
else:
    F_x_2 = 0
    F_x_1 = 1
    index = 2
    while index < n:
        F_sum = F_x_2 + F_x_1
        F_x_2 = F_x_1
        F_x_1 = F_sum
        index = index + 1

    print(F_x_2 + F_x_1) 
```


## Question 7 - Second Largest

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

# OR

large_1 = int(input())
large_2 = 0

while True:
    x = int(input())
    if x == 0:
        break

    if x > large_1:
        large_2 = large_1
        large_1 = x
    elif x > large_2:
        large_2 = x

print(large_1 - large_2)
```


## Question 8 - Digiiiits

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


## Question 9 - Positive Mental Attitude

```python
odd_sum = 0

x = int(input())
while x >= 0:
    if x % 2 == 1:
        odd_sum += x
    x = int(input())

print(odd_sum)
```


## Question 10 - Guess

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
        
# Limited number of tries

import random

number = random.randint(1, 10)

count = 0
trys = 3
not_found = True

while not_found and trys > 0:
    x = int(input())
    count = count + 1
    trys = trys - 1
    if x > number:
        print("Too high!")
    elif x < number:
        print("Too low!")
    else: # x == number
        print("You got it!")
        not_found = False

if not not_found:
    print("And it only took you", count, "tries!")
else:
    print("You could not find!")
```


## Question 11 - NoBig

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


## Question 12 - FizzBuzz

```python
userNumber= int(input("Please enter a number: "))
for i in range(1,userNumber+1):
    output = ""
    if(i%2==0):
        output+= "Fizz"
    if(i%3==0):
        output+= "Buzz"
    if(output==""):
        output = i
    print(output)
```


## Question 13

```python
a = int(input())
b = int(input())

if a == 0 or b == 0:
    print(0)
else:
    index = 1
    small = a
    if b < a:
        small = b

    result = 1

    while index <= small:
        if a % index == 0 and b % index == 0:
            result = index
        index = index + 1

    print(result)
```


## Question 14

```python
n = int(input())

copy = n
count = 0

while copy > 0:
    count = count + 1
    copy = copy // 10

copy = n

summation = 0

while copy > 0:
    digit = copy % 10
    summation = summation + digit ** count
    count = count - 1
    copy = copy // 10

print(n == summation)
```
