# Conditional-Execution

## Q1
```python
num1 = int(input("Please enter first number: "))
num2 = int(input("Please enter second number: "))

if(num1 % num2 == 0):
    print("First number can be divided by second number.")
else:
    print("First number can be divided by second number. Remainder is: " + str(num1 % num2))
```


## Q2

```python
num1 = int(input("Please enter first number: "))
num2 = int(input("Please enter second number: "))
num3 = int(input("Please enter third number: "))

if num1 > num2 and num2 > num3:
    minnum = num3
    maxnum = num1
elif num1 > num3 and num3 > num2:
    minnum = num3
    maxnum = num1
elif num2 > num3 and num3 > num1:
    minnum = num1
    maxnum = num2
elif num2 > num1 and num1 > num3:
    minnum = num3
    maxnum = num2
elif num3 > num1 and num1 > num2:
    minnum = num2
    maxnum = num3
else:
    minnum = num1
    maxnum = num3
    
print("Minimum is: " + str(minnum))
print("Maximum is: " + str(maxnum))

# We can also calculate min and max with builtin functions
# print("Minimum is: " + str((min(num1,num2,num3))))
# print("Maximum is: " + str((max(num1,num2,num3))))

# Another solution
minimum = c
maximum = c

if a >= b and a >= c:
    maximum = a
elif b >= a and b >= c:
    maximum = b

if a <= b and a <= c:
    minimum = a
elif b <= a and b <= c:
    minimum = b

print(minimum, maximum)
```


## Q3
```python
w = int(input("Plese enter your weight: "))
h = float(input("Plese enter your height (meters): ")) / 100

bmi = w / h**2
print("Your BMI score is: " + str(bmi))

if bmi < 15:
    print("You are very severely underweight.")
elif bmi < 16:
    print("You are severely underweight.")
elif bmi < 18.5:
    print("You are underweight.")
elif bmi < 25:
    print("You are normal.")
elif bmi < 30:
    print("You are overweight.")
elif bmi < 35:
    print("You are Obese Class I.")
elif bmi < 40:
    print("You are Obese Class II.")
else:
    print("You are Obese Class III.")
```


## Q4
```python
num1 = int(input("Plese enter first number: "))
num2 = int(input("Plese enter second number: "))

if num1 % num2 == 0 or num2 % num1 == 0:
    print("Multiple")
else:
    print("Not multiple")

```


## Q5

```python
amount = int(input("Please enter the amount of money requested by the customer: "))
n = int(input("Please enter the amount of banknotes inside the machine: "))

if (n < amount//5): #we will have more than or equal to 5 coins
    print(n, amount - 5*n)
else:
    print(amount//5, amount%5)

# Another solution
if n * 5 > amount:
    print(amount // 5, amount % 5)
else:
    print(n, amount - (n * 5))

```


## Q6

### Q6a

```python
num1 = int(input("Please enter first number: "))
num2 = int(input("Please enter second number: "))

if (num1 > num2):
    tmp = num1
    num1 = num2
    num2 = tmp

print(num1, num2)
```

### Q6b

```python
num1 = int(input("Please enter first number: "))
num2 = int(input("Please enter second number: "))
num3 = int(input("Please enter third number: "))

#1 and 2
if (num1 > num2):
    tmp = num1
    num1 = num2
    num2 = tmp

#1 and 3
if (num1 > num3):
    tmp = num1
    num1 = num3
    num3 = tmp

#2 and 3
if (num2 > num3):
    tmp = num2
    num2 = num3
    num3 = tmp

print(num1, num2, num3)

# Another solution
if a >= b and a >= c:
    maximum = a
elif b >= a and b >= c:
    maximum = b
else:
    maximum = c

if a <= b and a <= c:
    minimum = a
elif b <= a and b <= c:
    minimum = b
else:
    minimum = c

middle = a + b + c - minimum - maximum

print(minimum, middle, maximum)

""" We can find middle in another way
if a != minimum and a != maximum:
    middle = a
if b != minimum and b != maximum:
    middle = b
if c != minimum and c != maximum:
    middle = c
"""
```


## Q7

```python
Bob = input("Decision of Bob (silence/betrayal): ")
Sam = input("Decision of Sam (silence/betrayal): ")

#Solution 1    Does not print anything at incorrect input
if (Bob=='silence'):
    if (Sam=='silence'):
        print("1 1")
    elif (Sam=='betrayal'):
        print("3 0")

elif (Bob=='betrayal'):
    if (Sam=='silence'):
        print("0 3")
    elif (Sam=='betrayal'):
        print("2 2")

#Solution 2    Prints at incorrect input
if (Bob != "silence" and Bob != "betrayal") or (Sam != "silence" and Sam != "betrayal"):
    print("Wrong input!")
else:
    if Bob == "silence":
        if Sam == "silence":
            print(1, 1)
        else: # Sam=='betrayal'
            print(3, 0)
    else: # Bob == "betrayal"
        if Sam == "silence":
            print(0, 3)
        else: # Sam=='betrayal'
            print(2, 2)

```


## Q8

```python
x = int(input())
y = int(input())
z = int(input())

# Solution 1
print(not(x <= 0 or y <= 0 or z <= 0)and((x * x + y * y == z * z)or(x * x + z * z == y * y)or(y * y + z * z == x * x)))

# Solution 2
if x <= 0 or y <= 0 or z <= 0:
    print("False")
elif x*x + y*y == z*z or x*x + z*z == y*y or y*y + z*z == x*x:
    print("True")
else:
    print("False")
```


## Q9

```python
input = int(input("Please enter an integer from 0 to 9999:"))
if (input<0 or input>9999):
    print("Input is not in the interval 0-9999")
else:
    print(input//1000 + (input//100)%10 + (input//10)%10 + input%10)

# More clearly
if a < 0 or a > 9999:
    print("Input is not in the interval")
else: # a = 1234
    summation = a % 10 # = 4
    a = a // 10 # a = 123
    summation = summation + (a % 10) # = 3
    a = a // 10 #12
    summation = summation + (a % 10) # = 2
    a = a // 10 #1
    summation = summation + a # = 1
    print(summation)
```


## Q10
```python
warm = int(input("Please enter the degress of water:"))
if warm < 0:
    print("It is in the solid state.")
elif warm == 0:
    print("It can be solid or liquid.")
elif warm < 100:
    print("It is in the liquid state.")
elif warm == 100:
    print("It can be liquid or gas.")
else:
    print("It is in the gas state.")
```
