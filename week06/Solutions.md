# Nested Loops

## Question 1 - R\*\*\*tangle

### Question 1a

```python
N, M = map(int, input().split())

for _ in range(N):
    for _ in range(M):
        print("*", end="")
    print()
```

### Question 1b

```python
N, M = map(int, input().split())

for i in range(N):
    for j in range(M):
        if i == 0 or j == 0 or i == N - 1 or j == M - 1:
            print("*", end="")
        else:
            print("-", end="")
    print()
```

## Question 2 - TriNumber

### Question 2a

```python
N = int(input())

for i in range(1, N + 1):
    for j in range(i):
        print(i, end="")
    print()
```

### Question 2b

```python
N = int(input())

for i in range(1, N + 1):
    for j in range(i):
        print(j + 1, end="")
    print()
```

### Question 2c

```python
N, x = map(int, input().split())

for i in range(1, N+1):
    for j in range(i):
        print(x ** (j + 1), end=" ")
    print()
```

## Question 3 - TriHard

```python
N = int(input())

for i in range(N):
    for j in range(N - 1):
        if i + j < N:
            print("-", end="")
        else:
            print("*", end="")
    print()
```

## Question 4 - Sum Facts

```python
number = int(input())

sum = 0

while number > 0:
    digit = number % 10
    number = number // 10
    factorial = 1
    for i in range(1, digit + 1):
        factorial *= i
    sum += factorial

print(sum)
```

## Question 5 - Prime Example

### Question 5a

```python
n = int(input())

isPrime = True
for i in range(2, n):
    if n % i == 0:
        isPrime = False
        break

if isPrime:
    print("Prime")
else:
    print("Prime Not")
```

### Question 5b

```python
n = int(input())

for j in range(2,n+1):
    isPrime = True
    for i in range(2, j):
        if j % i == 0:
            isPrime = False
            break
    if isPrime:
        print(j, end=" ")
```

## Question 6 - Prime factors

### Question 6a

```python
N = int(input())

for i in range(1, N + 1):
    if N % i == 0:
        print(i, end=" ")
```

### Question 6b

```python
number = int(input())
for i in range(2, number + 1):
    while number % i == 0:
        number //= i
        if number != 1:
            print(i, end=" * ")
        else:
            print(i)
```

### Question 6c

```python
number = int(input())
for i in range(2, number + 1):
    count = 0
    while number % i == 0:
        number //= i
        count += 1
    if count > 0:
        if number != 1:
            print(i, "^", count, end=" * ")
        else:
            print(i, "^", count)
```

## Question 7 - Zzz

```python
n = int(input("Enter number greater than 2: "))

for i in range(n):
    for j in range(n):
        if i == 0:
            print("*", end="")
        elif i == n - 1:
            print("*", end="")
        elif i + j == n - 1:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

## Question 8 - Half-Matrix

### Question 8a

```python
N = int(input())

counter = 0

for i in range(1, N+1):
    for j in range(i):
        print(counter, end=" ")
        counter += 1
    print()
```

### Question 8b

```python
N = int(input())

for i in range(N):
    cur = i
    k = N - 1
    for j in range(i + 1):
        print(cur, end=" ")
        cur += k
        k -= 1
    print()
```

## Question 9 - Sore Loser Bob

```python
from random import randint

max_score = int(input("Winning score: "))
iteration = 0
bob_won = False
while not bob_won:
    bob_score = 0
    iteration += 1
    while abs(bob_score)<max_score:
        bob_number = randint(0,10)
        sam_number = randint(0,10)

        if (bob_number>sam_number):
            bob_score+=1
        elif (bob_number<sam_number):
            bob_score-=1

    if bob_score == max_score:
        bob_won = True

print("Bob was able to win after %d iterations!" % iteration)
```

## Question 10 - Palindromic Primes

```python
start, end = map(int, input().split())

for i in range(start, end + 1):
    num = i
    reverse = 0
    while num > 0:
        digit = num % 10
        num = num // 10
        reverse = reverse * 10 + digit
    if reverse == i:
        isPrime = True
        for j in range(2, i):
            if i % j == 0:
                isPrime = False
                break
        if isPrime:
            print(i, end=" ")
```

## Question 11 - Draw a figure

```python
size= int(input("Please enter the size: "))

backslash_pointer = 0
slash_pointer = 2 * size
middle_pointer = size

for i in range(2 * size):
    if i == size:
        backslash_pointer += 1
        slash_pointer -= 1
    for j in range(2 * size + 1):
        if j == backslash_pointer:
            print("\\", end="")
        elif j == middle_pointer:
            print("|", end="")
        elif j == slash_pointer:
            print("/", end="")
        else:
            print(" ", end="")
    backslash_pointer += 1
    slash_pointer -= 1
    print()
```


