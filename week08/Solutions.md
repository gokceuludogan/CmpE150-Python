# Lists

## Question 1 - Large

```python
N = int(input())

list1 = list()
for i in range(N):
    list1.append(int(input()))

average = 0
for l in list1:
    average += l
average /= N

# average = sum(list1)/len(list1)

for l in list1:
    if l > average:
        print(l, end=' ')
```



## Question 2 - Let's Count

```python
def find_freq(list1):
    freq = [0] * 101
    for l in list1:
        freq[l] += 1
    for i, f in enumerate(freq):
        if f > 0:
            print(str(i) + ' --> ' + str(f))


find_freq([5, 10, 2, 5, 50, 5, 10, 1, 2, 2])
```



## Question 3 - Fifth Powers

```python
list1 = list(map(int, input().split()))
print([x**5 for x in list1])
```



## Question 4 - Pairs

```python
def find_pairs(list1, X):
    for i, l1 in enumerate(list1):
        for l2 in list1[i + 1:]:
            if l1 + l2 == X:
                print("(%d, %d)" % (l1, l2))
                
    # [(l1,l2) for i, l1 in enumerate(list1) for l2 in list1[i+1:] if l1+l2==7]


find_pairs([2, 4, 3, 5, 7, 8, 9], 7)
```



## Question 5 - To the left

```python
def rotate(l, n):
    return l[n:] + l[:n]


print(rotate([1, 2, 3, 4, 5], 2))
```



## Question 6 - Reverse

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



## Question 7 - Remove X

```python
list1 = [5, 20, 15, 20, 25, 50, 20]


def removeValue(sampleList, val):
    return [value for value in sampleList if value != val]


resList = removeValue(list1, 20)
print(resList)
```



## Question 8 - Remove Consecutive Duplicates

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



## Question 9 - Remove Duplicates

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



## Question 10 - Odd Occurrences

```python
def oddones(l):
    mylist = []

    for i in range(len(l)):
        if not l[i] in mylist:
            mylist.append(l[i])
        else:
            mylist.remove(l[i])

    for i in range(len(mylist)):
        print(mylist[i], end=' ')


oddones([1, 1, 2, 3, 3, 3])
```



## Question 11 - Slice List Sum

```python
def slice_list(list1, n):
    result = []
    sind = 0
    for i in range(1, len(list1)+1):
        if sum(list1[sind:i]) > n:
            result.append(list1[sind:i])
            sind = i
    return result

print(slice_list([5, 3, 2, 1 ,4 ,51, 2, 1, 3, 5, 3, 5], 4))s
```



## Question 12 - Inception

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



## Question 13 - Shuffle Double

```python

def shuffle_double(list1):
    result = [list1[x] for x in range(0, len(list1), 2)]
    result.extend([list1[x] for x in range(1, len(list1), 2)])
    return result

print(shuffle_double([1, 2, 3, 4, 5, 6, 7, 8, 9]))
```



## Question 14 - Bubble Sort

```python
def bubble_sort(arr):
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


print(bubble_sort([4, 2, 8, 6, 7, 3, 1, 5]))

#print(sorted([4, 2, 8, 6, 7, 3, 1, 5]))
```



## Question 15 - Consecutive Combo

```python
def consecutive_combo(a, b):
    c = sorted(a+b)
    return len(c)-1 == c[-1] - c[0]

print(consecutive_combo([7, 4, 5, 1], [2, 3, 6]))
```
