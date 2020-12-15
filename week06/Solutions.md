## Question 1 - Reverse

```python
N = int(input())

list1 = list()
for i in range(N):
    list1.append(int(input()))

# a
print(list1[::-1])

# b
list1 = list1[::-1]
# list1.reverse()
print(list1)
```

## Question 2 - Let's Count

```python
def find_freq(list1):
    freq = [0] * 100
    for l in list1:
        freq[l] += 1
    for i, f in enumerate(freq):
        if f > 0:
            print(str(i) + ' --> ' + str(f))


find_freq([5, 10, 2, 5, 50, 5, 10, 1, 2, 2])
```

## Question 3 - Inception

```python
N = int(input())
M = int(input())

list1 = list()
for i in range(N):
    list1.append(int(input()))

list2 = list()
for i in range(M):
    list2.append(int(input()))

for j in range(len(list2) - len(list1)):
    isFound = True
    for i in range(len(list1)):
        if list1[i] != list2[j + i]:
            isFound = False
            break

    if isFound:
        print(j)
        break
```

## Question 4 - Pairs

```python
def find_pairs(list1, X):
    for i, l1 in enumerate(list1):
        for l2 in list1[i + 1:]:
            if l1 + l2 == X:
                print("(%d, %d)" % (l1, l2))


find_pairs([2, 4, 3, 5, 7, 8, 9], 7)
```

## Question 5 - fix34

```python
N = int(input())
list1 = list()
for i in range(N):
    list1.append(int(input()))

for i in range(len(list1)):
    if list1[i] == 3:
        for j in range(len(list1)):
            if list1[j] == 4 and list1[j - 1] != 3:
                list1[i + 1], list1[j] = list1[j], list1[i + 1]

print(list1)
```

## Question 6 - Bubble Sort

```python
def bubbleSort(arr):
    n = len(arr)

    # Traverse through all array elements
    for i in range(n - 1):
        # range(n) also work but outer loop will repeat one time more than needed.

        # Last i elements are already in place
        for j in range(0, n - i - 1):

            # traverse the array from 0 to n-i-1
            # Swap if the element found is greater
            # than the next element
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]

                # temp = arr[j]
                # arr[j] = arr[j+1]
                # arr[j+1] = temp

    return arr


print(bubbleSort([4, 2, 8, 6, 7, 3, 1, 5]))
```

## Question 7 - Concatwise

```python
def concatwise(list1, list2):
    return [i + j for i, j in zip(list1, list2)]


list1 = ["M", "na", "i", "Pat"]
list2 = ["y", "me", "s", "rick"]
print(concatwise(list1, list2))
```

## Question 8 - Combine Reverse

```python
def combine_reverse(list1, list2):
    for x, y in zip(list1, list2[::-1]):
        print(x, y)


list1 = [10, 20, 30, 40]
list2 = [100, 200, 300, 400]
combine_reverse(list1, list2)
```

## Question 9 - Remove X

```python
list1 = [5, 20, 15, 20, 25, 50, 20]


def removeValue(sampleList, val):
    return [value for value in sampleList if value != val]


resList = removeValue(list1, 20)
print(resList)
```