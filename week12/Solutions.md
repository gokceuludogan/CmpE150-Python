# Dictionaries

## Question 1 

```python
def name_to_age_ratio(a):
    result = []
    for name, age in a.items():
        total_characters = sum([len(word) for word in name.split()])
        result.append(totalCharacters / age)
    return result
```

### Alternative

```python
def name_to_age_ratio(info):
    results = []
    for name in info:
        results.append(sum([for ch in name if not ch.isspace()]) / info[name])
    return results    
```

## Question 2

```python
mylist = str(input()).split()
mydict = {}

for i in mylist:
    mydict[i] = 1 if mydict.get(i) is None else mydict[i] + 1
for i in sorted(mydict, key = mydict.get, reverse = True):
    print(i, end = " ")
```

### Alternative

```python
words = str(input()).split()
counts = {}
for word in words:
    # counts[word] = counts.get(word, 0) + 1
    if word not in counts:
        counts[word] = 1
    else:
        counts[word] += 1
counts_sorted = sorted(counts, key=counts.get, reverse=True) # returns words
print(' '.join(counts_sorted))
```

## Question 3

```python
def tickets(people):
    change = {25: 0, 50: 0, 100: 0}
    for money in people:
        if money == 25: 
            change[25] += 1
        elif money == 50: 
            change[25] -= 1
            change[50] += 1
        elif money == 100 and change[50] > 0:
            change[25] -= 1
            change[50] -= 1
        elif money==100 and change[50] == 0:
            change[25] -= 3

        if change[25] < 0 or change[50] < 0:
            return 'NO'
    return 'YES'

print(tickets([25, 25, 50])) # => YES
print(tickets([25, 100])) # => NO. Vasya will not have enough money to give change to 100 dollars
print(tickets([25, 25, 50, 50, 100])) # => NO. Vasya will not have the right bills to give 75 dollars of change (you can't make two bills of 25 from one of 50)
```

# Sets

## Question 1

```python
A = {1, 2, 3, 4, 5, 6}
B = {1, 1, 2, 7, 11}

def set_operations(set1, set2):
    print("A ∪ B = {}".format(set1.union(set2)))
    print("A ∩ B = {}".format(set1.intersection(set2)))
    print("A / B = {}".format(set1.difference(set2)))
    print("B / A = {}".format(set2.difference(set1)))

set_operations(A, B)
```

## Question 2

```python
required = {"CmpE150","CmpE160","CmpE220","CmpE250","CmpE260"}
def is_eligible(current):
    if len(required.intersection(current)) == len(required):
        return "Eligible"
    else:
        return "Not Eligible"
print(is_eligible({"Cmpe150"}))
```

## Question 3

```python
def overall_traits(traits1, traits2):
    intersection = traits1.intersection(traits2)
    return sum(intersections)
```

## Question 4

```python
def is_distinct(string):
    return len(set(string)) == len(string)

print(is_distinct('violate'))
```

