# Lists and Tuples

## Question 1 - All the Same

```python
def check(sampleTuple):
    return all(i == sampleTuple[0] for i in sampleTuple)


tuple1 = (45, 45, 45, 45)
print(check(tuple1))
```

## Question 2 - Filter Even Numbers

```python
# https://www.codewars.com/kata/53dbd5315a3c69eed20002dd

def even_filter(list1):
    return [i for i in list1 if i % 2]


example = [2, 4, 6, 8]
print(even_filter(example))

```

## Question 3 - List Comprehension

### Question 3a

```python
def sum_of_evens(list):
    return sum([num for num in list if num % 2 == 0])

print(sum_of_evens([1, 2, 3, 4, 5]))
```

### Question 3b

```python
def sum_of_odds(list):
    return sum([num for num in list if num % 2])

print(sum_of_odds([1, 2, 3, 4, 5]))
```

## Question 4 - Remove Duplicates

```python
def remove_duplicates(list1):
    result = []
    for i in list1:
        if i not in result:
            result.append(i)
    return result
    # return list(dict.fromkeys(list1))


example = [1, 1, 1, 1, 1, 2, 2, 2, 3, 2, 2, 4, 5]
print(remove_duplicates(example))

```

## Question 5 - Remove Consecutive Duplicates

```python
def remove_consecutive_duplicates(list1):
    i = 1
    while i < len(list1):
        if list1[i - 1] == list1[i]:
            list1.pop(i)
        else:
            i += 1
    return list1


example = [1, 1, 1, 1, 1, 2, 2, 2, 3, 2, 2, 4, 5]
print(remove_consecutive_duplicates(example))
```

### Question 6 - Odd Occurrences

```python
def oddones(*l):
    mylist = []

    for i in range(len(l)):
        if not l[i] in mylist:
            mylist.append(l[i])
        else:
            mylist.remove(l[i])

    for i in range(len(mylist)):
        print(mylist[i], end=' ')


oddones(1, 1, 2, 3, 3, 3)
```

## Question 7 - Neighbors

```python
def sum_neighbors(numbers):
    new_list = [numbers[0] + numbers[1]]
    x = 1
    while x < len(numbers) - 1:
        new_list.append(numbers[x - 1] + numbers[x] + numbers[x + 1])
        x += 1
    new_list.append(numbers[x - 1] + numbers[x])
    return new_list

new_list = sum_neighbors([10, 20, 30, 40])
print(new_list)
```

## Question 8 - Circulation

### Question 8a - To the left

```python
def rotate(l, n):
    return l[n:] + l[:n]

print(rotate([1, 2, 3, 4, 5], 2))
```

### Question 8b - Left or right?

```python
def rotate(l, n, is_left):
    if is_left:
        return l[n:] + l[:n]
    else:
        return l[-n:] + l[:-n]
    
print(rotate([1, 2, 3, 4, 5], 2, False))
```

## Question 9 - Points

### Question 9a - Distance

```python
def distance(point1, point2):
    return ((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2) ** (1/2)

print(distance((3, 0), (0, 4)))
```

### Question 9b - Closest

```python
def distance(point1, point2):
    return ((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2) ** (1/2)

def closest(point1, point2):
    dist1 = distance(point1, (0, 0))
    dist2 = distance(point2, (0, 0))
    return point2 if dist1 > dist2 else point1

print(closest((3, 0), (0, 4)))
```

### Question 9c - Farthest

```python
def distance(point1, point2):
    return ((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2) ** (1/2)

N = int(input())
points = []
for i in range(N):
    x, y = input().split()
    points.append((int(x), int(y)))

max_dist = None
for ix, p in enumerate(points):
    for p2 in points[ix+1:]:
        dist = distance(p, p2)
        if max_dist is None or dist > max_dist:
            max_dist = dist
            farthest = (p, p2)

print(farthest)
```

## Question 10 - Fractions

### Question 10a - Addition

```python
def simplify(nom, denom):
    factor = min(nom, denom)
    while True:
        if nom % factor == 0 and denom % factor == 0:
            nom //= factor
            denom //= factor
        factor -= 1
        if factor == 1:
            break
    return nom, denom


def addition(frac1, frac2):
    common_denominator = frac1[1] * frac2[1]
    nominator_sum = frac1[0] * frac2[1] + frac2[0] * frac1[1]
    return simplify(nominator_sum, common_denominator)

print(addition((3,5), (4, 8)))
```

### Question 10b - Multiplication

```python
def simplify(nom, denom):
    factor = min(nom, denom)
    while True:
        if nom % factor == 0 and denom % factor == 0:
            nom //= factor
            denom //= factor
        factor -= 1
        if factor == 1:
            break
    return nom, denom


def multiply(frac1, frac2):
    return simplify(frac1[0] * frac2[0], frac1[1] * frac2[1])

print(multiply((3,5), (1, 3)))
```

## Question 11 - Tuples/Lists

### Question 11a - Lists inside Tuple

```python
def replace_last_value(items, value):
    for item in items:
        item[-1] = value
    return items

modified_list = replace_last_value(([10, 20, 40], [40, 50, 60], [70, 80, 90]), 100)
print(modified_list)
```

### Question 11b - Tuples inside List

```python
def replace_last_value(items, value):
    for item in items:
        item = item[:-1] + (value, )
    return items

# Alternatively:
def replace_last_value(items, value):    
    return [tup[:-1] + (value,) for tup in items]

modified_list = replace_last_value([(10, 20, 40), (40, 50, 60), (70, 80, 90)], 100)
print(modified_list)
```


## Question 12 - Tuple Sort Tuple

```python
def sort_tuple2(sampleTuple):
    return tuple(sorted(list(sampleTuple), key=lambda x: x[1]))


tuple1 = (('a', 23), ('b', 37), ('c', 11), ('d', 29))
tuple1 = sort_tuple2(tuple1)
print(tuple1)
```
