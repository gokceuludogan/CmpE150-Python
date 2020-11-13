## Question 1

```python
number = float(input())
if number >= 0:
    print(number)
else:
    print(-number)
```

## Question 2

```python
num1 = int(input())
num2 = int(input())
if num1 % num2 == 0:
    print(num1//num2)
else:
    print(num1%num2)
```

## Question 3

```python
a = int(input())
b = int(input())
c = int(input())
if a > b and b > c:
    print(c, a)
elif a > c and c > b:
    print(b, a)
elif b > c and c > a:
    print(a, b)
elif b > a and a > c:
    print(c, b)
elif c > a and a > b:
    print(b, c)
else:
    print(a, c)  
```



```python
a = int(input())
b = int(input())
c = int(input())
max_num, min_num = None, None
if (a >= b) and (a >= c): 
    max_num = a 
elif (b >= a) and (b >= c): 
    max_num = b 
else: 
    max_num = c 

if (a <= b) and (a <= c): 
    min_num = a 
elif (b <= a) and (b <= c): 
    min_num = b 
else: 
    min_num = c     
    
print(min_num, max_num)    
```



```python
a = int(input())
b = int(input())
c = int(input())

max_num = a if a > b else b
max_num = c if c > max_num else max_num

min_num = a if a < b else b
min_num = c if c < min_num else min_num

print(min_num, max_num)
```



## Question 4

```python
num_input = int(input())
if num_input % 2 == 0:
    print('Divisible by 2')
if num_input % 3 == 0:
    print('Divisible by 3')
if num_input % 5 == 0:
    print('Divisible by 5')    
        
```

## Question 5

```python
age = int(input())
if age >= 0 and age <= 17:
    print('Child')
elif age >= 18 and age <= 64:
    print('Can Work')
elif age >= 65:
    print('Retired')
```

## Question 6

```python
year = int(input())

if year % 400 == 0:
    print('Leap year')
elif year % 100 == 0:
    print('Not a leap year')
elif year % 4 == 0:
    print('Leap year')
else: 
    print('Not a leap year')
   
```

```python
year = int(input())

if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print('Leap year')
else:
    print('Not a leap year')
```

## Question 7

```python
mt = int(input())
lab = int(input())
ass = int(input())
proj = int(input())
final = int(input())
overall_grade = mt * 0.2 + lab * 0.1 + ass * 0.15 + proj * 0.25 + final * 0.3
if overall_grade >= 75:
    print('A')
elif overall_grade >= 55:
    print('B')
elif overall_grade >= 35:
    print('C')
else:
    print('F')    
```

## Question 8

```python
mass = int(input())
height = float(input())
bmi = mass / height ** 2
print('%.1f' % bmi)
if bmi <= 15:
    print('Very severely underweight')
elif bmi <= 16:
    print('Severely underweight')
elif bmi <= 18.5:
    print('Underweight')
elif bmi <= 25:
    print('Normal (healthy weight)')
elif bmi <= 30:
    print('Overweight')
elif bmi <= 35:
    print('Obese Class I (Moderately obese)')
elif bmi <= 40:
    print('Obese Class II (Severely obese)')
else:
    print('Obese Class III (Very severely obese)')
```

## Question 9

```python
a = int(input())
b = int(input())

if a % b == 0 or b % a == 0:
    print('Multiple')
else:
    print('Not Multiple')
```

## Question 10

```python
import math
a = float(input())
b = float(input())
c = float(input())
disc = b ** 2 - 4 * a * c 
if disc > 0:
    print((-b + math.sqrt(disc)) / 2 * a, (-b - math.sqrt(disc)) / 2 * a)
elif disc == 0:
    print((-b + math.sqrt(disc)) / 2 * a)
```

