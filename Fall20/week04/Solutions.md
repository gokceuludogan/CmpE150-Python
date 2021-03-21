# Nested Loops

## Question 1 - R\*\*\*tangle

### Question 1a

```python
N = int(input("N: "))
M = int(input("M: "))

for _ in range(N):
    for _ in range(M):
        print("*", end='')
    print()
```

### Question 1b

```python
N = int(input("N: "))
M = int(input("M: "))

for _ in range(M):
    print("*", end='')
print()

for _ in range(N-2):
    print("*", end='')
    for _ in range(M-2):
        print("-", end='')
    print("*")

for _ in range(M):
    print("*", end='')
```


## Question 2 - TriNumber

### Question 2a

```python
N = int(input("N: "))

for i in range(1, N+1):
    for j in range(i):
        print(i, end='')
    print()
```

### Question 2b

```python
N = int(input("N: "))

for i in range(1, N+1):
    for j in range(i):
        print(j+1, end='')
    print()
```

### Question 2c

```python
N = int(input("N: "))
x = int(input("x: "))

for i in range(1, N+1):
    for j in range(1, i+1):
        power = 1
        for k in range(j):
            power *= x
        print(power, end=' ')
    print()
```


## Question 3 - TriHard

```python
N = int(input())

for i in range(1, N+1):
    for j in range(N - i):
        print('-', end='')
    for j in range(i):
        print('*', end='')
    print()
```


### Question 4 - Zzz

```python
    n=int(input())
    
    for i in range(n):
        for j in range(n):
            if i==0:
                print('*', end='')
            elif i+j==n-1:
                print('*',end='')
            elif i==n-1:
                print('*', end='')
            else:
                print(' ', end='')
        print('\n')
```


## Question 5 - Sum Facts

```python
x = int(input())

fact_sum = 0

while x > 0:
    digit = x % 10
    fact = 1
    for i in range(2, digit+1):
        fact *= i
    fact_sum += fact

    x //= 10

print(fact_sum)
```


## Question 6 - Sum of Digits

```python
n = int(input())

while n >= 10:
    sum = 0
    while n:
        sum += n%10
        n //= 10
    n = sum

print(n)
```


## Question 7 - Prime Example

### Question 7a

```python
x = int(input())

isPrime = True

for i in range(2, x):
    if x % i == 0:
        isPrime = False
        break

if isPrime:
    print("Prime")
else:
    print("Prime Not")
```


### Question 7b

```python
N = int(input())

for x in range(2, N+1):
    isPrime = True
    for i in range(2, x):
        if x % i == 0:
            isPrime = False
            break

    if isPrime:
        print(x, end=' ')
```


## Question 8 - Prime factors

### Question 8a

```python
number = int(input())
for i in range(1, number + 1):
    if number % i == 0:
        print(i, end = " ")
```

### Question 8b

```python
number = int(input())
for i in range(2, number + 1):
    while number % i == 0:
        number //= i
        print(i, end=" ")
```

This works because at any point in the loop, number doesn't have any factors smaller than ``i``. Therefore, ``i`` has to be prime if it divides ``number``.

### Question 8c

```python
number = int(input())
firstPrime = True
for i in range(2, number + 1):
    count = 0
    while number % i == 0:
        number //= i
        count += 1
    if count > 0:
        if firstPrime:
            firstPrime = False
        else:
            print(" * ", end="")
        print(i, "^", count, end="")
```



## Question 9 - Pascal's Triangle

```python
    import math
    
    n=int(input())
    
    for i in range(n):
        for j in range(i+1):
            c_ij=int( math.factorial(i) / ( math.factorial(j) * math.factorial(i-j) ))
            print(str(c_ij), end=' ')
        print('\n')
```


## Question 10 - Half-Matrix

### Question 10a

```python
n=int(input())
cur = 0
    
for i in range(n):
    for j in range(i+1):
        print(cur , end = ' ')
        cur+=1
    print()
```

### Question 10b

```python

n = int(input())

for i in range(n):
    cur = i
    j = n-1
    for k in range(i+1):
        print(cur ,end=' ')
        cur+=j
        j=j-1
    print()

```