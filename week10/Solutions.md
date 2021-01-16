# Dictionaries

## Question 1 - Split the Bill
```python
# https://www.codewars.com/kata/5641275f07335295f10000d0/python
group = {
    'A': 20,
    'B': 15,
    'C': 10
}

def split_the_bill(x):
    diff = sum(x.values())/float(len(x))
    return {k: x[k]-diff for k in x}

print(split_the_bill(group)) 
```

## Question 2 - Different Types
This was from another school's intro to computing question. It was due to 10.11.
```python
def separate(my_list):
    my_dict = dict()
    for i in my_list:
        if type(i) in my_dict:
            my_dict[type(i)].append(i)
        else:
            my_dict[type(i)] = [i]
    return my_dict

original_list = [10, 4.20, False, 'Word', 'CMPE150', 30, 3.5, 9.99, 'oblivion', True, 68, 88, "88"]
seperated_list = separate(original_list)

for k,v in seperated_list.items():
    print(k," -> ",v)
```

## Question 3 - Sorting Dictionary

```python
def sort_dict(d):
  return sorted(d.items(), key=lambda x: x[1], reverse=True)
 
print(sort_dict({3:1, 2:2, 1:3}))
```

## Question 4 - Letter Count 

```python
sentence = input()
my_dict = dict()
total_letter =0
for letter in sentence:
    if letter.isalpha():
        letter = letter.lower()
        total_letter+=1
        if letter not in my_dict:
            my_dict[letter] = 1
        else:
            my_dict[letter] += 1

sorted_dict = sorted(my_dict.items(), key=lambda x: (-x[1],x[0]))
for k,v in sorted_dict:
    print(k,"->","{:.2f}".format(v/total_letter))
    
```

## Question 5 - Dictionary Merge
```python
def merge(*dicts):
    mydict = dict()
    for d in dicts:
        for k, v in d.items():
            if k in mydict:
                mydict[k].append(d[k])
            else:
                mydict[k] = [v]
    return mydict
    
print(merge({"A": 1, "B": 2} , {"A": 3}))
```


## Question 6 - Zip Two Lists 

```python
list1 = ["melih", "burak", "ahmet", "recep", "melis"]
list2 = [1,2,3,4,5]
def dict_2_lists(list1, list2):
    return dict(zip(list1, list2))

print(dict_2_lists(list1,list2))

    
```


# Sets

## Question 1 - List to Distinct

```python 
def distinct_elements(lst):
    return list(set(lst))
distinct_list = distinct_elements([3,5,4,4,7,11,2,8])
print(distinct_list)
```

## Question 2 - Set Operations

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

## Question 3 - Diff

```python
def list_values(list1, list2):
    print('Missing values in list1', set(list2).difference(set(list1)))
    print('Additional values in list1', set(list1).difference(set(list2)))


lst1 = [1, 2, 3, 4, 5, 6]
lst2 = [4, 5, 6, 7, 8]
list_values(lst1, lst2)
```

## Question 4 - Distinct String

```python
def is_distinct(string):
    return len(set(string)) == len(string)


print(is_distinct('violate'))
```

## Question 5 - Numgram

```python
def is_numgram(string):
    numbers = ''.join([str(i) for i in list(range(10))])
    common_digits = set(string).intersection(set(numbers))
    return len(common_digits) == len(numbers)


numgram_result = is_numgram('SAS102BAD347 HELP5689')
if numgram_result:
    print('Numgram')
else:
    print('Not a numgram')
```
