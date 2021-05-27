## Q1

```python
def check(sampleTuple):
    return all(i == sampleTuple[0] for i in sampleTuple)


tuple1 = (45, 45, 45, 45)
print(check(tuple1))
```

#### Alternative

```python
def check(sample):
	for item in sample:
		if item != sample[0]:
			return False
	return True		

tuple1 = (45, 45, 45, 45)
print(check(tuple1))
```

## Q2

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


print(addition((3, 5), (4, 8)))
```

## Q3

### Q3a

```python
def replace_last_value(items, value):
    for item in items:
        item[-1] = value
    return items


modified_list = replace_last_value(([10, 20, 40], [40, 50, 60], [70, 80, 90]), 100)
print(modified_list)
```

### Q3b

```python
def replace_last_value(items, value):
    for ix in range(len(items)):
        items[ix] = items[ix][:-1] + (value,)
    return items


modified_list = replace_last_value([(10, 20, 40), (40, 50, 60), (70, 80, 90)], 100)
print(modified_list)
```

#### Alternative

```python
def replace_last_value(items, value):
    return [tup[:-1] + (value,) for tup in items]

modified_list = replace_last_value([(10, 20, 40), (40, 50, 60), (70, 80, 90)], 100)
print(modified_list)
```

## Q4

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

#### Alternative

```python
def sum_neighbors(numbers):
    new_list = [numbers[0] + numbers[1]]
    new_list.extend([numbers[i-1] + numbers[i] + numbers[i+1] for i in range(1, len(numbers) -1)])
    return new_list + [numbers[-2] + numbers[-1]]


new_list = sum_neighbors([10, 20, 30, 40])
print(new_list)
```

## Q5

### Question 5a

```python
def distance(point1, point2):
    return ((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2) ** (1 / 2)


print(distance((3, 0), (0, 4)))
```

### Question 5b

```python
def distance(point1, point2):
    return ((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2) ** (1 / 2)


def closest(point1, point2):
    dist1 = distance(point1, (0, 0))
    dist2 = distance(point2, (0, 0))
    return point2 if dist1 > dist2 else point1


print(closest((3, 0), (0, 4)))
```

### Question 5c

```python
def distance(point1, point2):
    return ((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2) ** (1 / 2)


N = int(input())
points = []
for i in range(N):
    x, y = input().split()
    points.append((int(x), int(y)))

max_dist = None
for ix, p in enumerate(points):
    for p2 in points[ix + 1:]:
        dist = distance(p, p2)
        if max_dist is None or dist > max_dist:
            max_dist = dist
            farthest = (p, p2)

print(farthest)
```

## Q6

```python
new_list = []
for i in range(5):
    value = int(input())
    if i == 0:
        new_list.append(value)
    else:
        if value >= new_list[-1]:
            new_list.append(value)
print(*new_list)

```

#### Alternative

```python
new_list = []
for i in range(5):
    value = int(input())
    if i == 0 or value >= new_list[-1]:
    	new_list.append(value)
print(*new_list)
```

## Q7

```python
def majority_vote(votes):
    for item in votes:
        if votes.count(item) > len(votes) // 2:
            return item
    return None    
```

## Q8

```python
def slice_list(list_of_numbers, n):
    new_list = []
    temp_list = []
    for item in list_of_numbers:
        temp_list.append(item)
        if sum(temp_list) >= n:
            new_list.append(temp_list)
            temp_list = []
    return new_list

print(slice_list([5, 3, 2, 1 ,4 ,51, 2, 1, 3, 5, 3, 5], 4))
```

## Q9

```python
def reverse_pair(list1):
    halfway = int(len(list1)/2)
    return [(x, y) for x, y in zip(list1[:halfway], list1[halfway:][::-1])]

print(reverse_pair(['Krillson', 'Fisherman', 'Chris', 'Wilson', 'Jack', 'The Handsome']))
```

#### Alternative 1

```python
def reverse_pair(list1):
    return [(list1[i], list1[-(i+1)]) for i in range(len(list1)//2)]

print(reverse_pair(['Krillson', 'Fisherman', 'Chris', 'Wilson', 'Jack', 'The Handsome']))
```

#### Alternative 2

```python
def reverse_pair(list1):
    pair_list = []
    for i in range(len(list1) // 2):
        pair_list.append((list1[i], list1[-(i+1)]))
    return pair_list

print(reverse_pair(['Krillson', 'Fisherman', 'Chris', 'Wilson', 'Jack', 'The Handsome']))
```

## Q10

```python
def shuffle_double(list1):
    result = [list1[x] for x in range(0, len(list1), 2)]
    result.extend([list1[x] for x in range(1, len(list1), 2)])
    return result

print(shuffle_double([1, 2, 3, 4, 5, 6, 7, 8, 9]))
```

#### Alternative

```python
def shuffle_double(list1):
    return list1[::2] + list1[1::2]

print(shuffle_double([1, 2, 3, 4, 5, 6, 7, 8, 9]))
```

## Q11

```python
list_of_tuple = [("1", 2), (3, 4), (5, "6"), (7, 5, 8), ("9", 10)]
output_list = []
for tup in list_of_tuple:
    is_added = True
    for item in tup:
        if type(item) != int:
            is_added = False
    if is_added:
        output_list.append(tup)
```

#### Alternative

```python
list_of_tuple = [("1", 2), (3, 4), (5, "6"), (7, 5, 8), ("9", 10)]
output_list = []
for tup in list_of_tuple:
    if all(type(item) == int for item in tup):
        output_list.append(tup)
```

## Q12

This solution includes the tuples containing the same elements in the output list

```python
my_input = [(10, 9), (240, 240, 240), (55, -43), (34, 71), (283, 16)] 
my_output = [i for i in my_input if i[::-1] == sorted(i)]
print(my_output)
```

The correct solution: The added condition removes the tuples containing same elements. 

```python
my_input = [(10, 9), (240, 240, 240), (55, -43), (34, 71), (283, 16)] 
my_output = [i for i in my_input if i[::-1] == sorted(i) and (not all(i.count(i[0]) == len(i)))]
print(my_output)
```

#### Alternative

```python
def decreasing(my_list):
    for i in range(len(my_list) - 1):
        if my_list[i] <= my_list[i + 1]:
            return False
    return True

my_input = [(10, 9), (240, 240, 240), (55, -43), (34, 71), (283, 16)] 
my_output = [i for i in my_input if decreasing(i)]
print(my_output)
```

## Q13

```python
my_input = [(2121777, 86), (2120654, 90), (1990650, 83), (2298755, 86) ]
my_input.sort(key = lambda x: x[1])
print(my_input)
```

#### Alternative

```python
# sorted(iterable, key=None, reverse=False)
my_input = [(2121777, 86), (2120654, 90), (1990650, 83), (2298755, 86) ]
print(sorted(my_input, lambda x: x[1]))
```

## Q14

```python
def odd_parity_checker(signal, target):
    (odd_parity, *information) = signal
    return odd_parity == (information.count(target) % 2 == 1)
```

#### Alternative 1

```python
def odd_parity_checker(signal, target):
    odd_parity = signal[0]
    information = signal[1:]
    return odd_parity == (information.count(target) % 2 == 1)
```

#### Alternative 2

```python
def odd_parity_checker(signal, target):
    parity = signal[0]
    information = signal[1:]
    count = information.count(target)
    remainder = count % 2
    is_odd = remainder == 1
    return parity == is_odd
```

