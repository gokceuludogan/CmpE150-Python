## Files

### Q1

```python
with open('data/paragraph.txt', 'r') as f_read:
    content = f_read.read()
    lines = content.split('.')
with open('paragraph_splitted.txt', 'w') as f_write:
    for line in lines:
        f_write.write(line + '\n')
```

```python
f_read = open('data/paragraph.txt', 'r')
content = f_read.read()
f_read.close()
lines = content.split('.')
f_write = open('paragraph_splitted.txt', 'w') 
for line in lines:
    f_write.write(line + '\n')
f_write.close()
```

### Q2

```python
filename = input()
input_f = open(filename, 'r')
output_f = open('output.txt', 'w')
for line in input_f:
    output_f.write(line[::-1])
input_f.close()
output_f.close()
```

### Q3

```python
filename = input()
f = open(filename, 'r')
content = f.read()
words = content.split(' ')
print(' '.join(sorted(words)))
f.close()
```

### Q4

```python
with open('input.txt','r') as f:
    words = [line.strip() for line in f.readlines()]
    alphas = [word for word in words if word.isalpha()]

with open('output.txt','w') as f:
    f.write("\n".join([word +'s' if word[-1] != 'y' else word[:-1]+'ies' for word in alphas]))
```

### Q5

```python
with open("grades.txt", 'r') as f:
    mt1 = [str(max(0, int(grade))) for grade in f.readline().split()]
    mt2 = [str(max(0, int(grade))) for grade in f.readline().split()]
    final = [str(max(0, int(grade))) for grade in f.readline().split()]
    
with open("corrected.txt", 'w') as f:
    f.write(' '.join(mt1))
    f.write('\n')
    f.write(' '.join(mt2))
    f.write('\n')
    f.write(' '.join(final))
```

### Q6

```python
with open("corrected.txt", 'r') as f:  
    mt1 = [float(grade) for grade in f.readline().split()]
    mt2 = [float(grade) for grade in f.readline().split()]
    final = [float(grade) for grade in f.readline().split()]
n = len(mt1)
avg = 0.3 * sum(mt1) / n + 0.3 * sum(mt2) / n + 0.4 * sum(final) / n
# avg = sum([0.3*mt1[i] + 0.3 * mt2[i] + 0.4 * final[i] for i in range(n)])/n
print('{:.2f}'.format(avg))
```

## Dictionaries

### Q1

```python
elements = [10, 4.20, False, 'Word', 'CMPE150', 30, 3.5, 9.99, 'oblivion', True, 68, 88, "88"]
element_dict = {}
for el in elements:
    if el not in element_dict:
        element_dict[type(el)] = [el]
    else:
        element_dict[type(el)].append(el)
for el_type, el_list in element_dict.items():
    print(el_type, '->', el_list)
```

### Q2

```python
sentence = input()
my_dict = dict()
total_letter =0
for letter in sentence:
    if letter.isalpha():
        letter = letter.lower()
        total_letter += 1
        if letter not in my_dict:
            my_dict[letter] = 1
        else:
            my_dict[letter] += 1

sorted_dict = sorted(my_dict.items(), key=lambda x: (-x[1], x[0]))
for k,v in sorted_dict:
    print(k,"->","{:.2f}".format(v/total_letter))
```

### Q3

```python
list1 = ["melih", "burak", "ahmet", "recep", "melis"]
list2 = [1,2,3,4,5]
def dict_2_lists(list1, list2):
    return dict(zip(list1, list2))

print(dict_2_lists(list1,list2))
```

### Q4

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

#### Q5

```python
lines = []
line = str(input())
while line != "exit":
    lines.append(line)
    line = str(input())

mydict = {}
for line in lines:
    line = line.split() # transform into a list
    info = {'genre' : line[1], 'release_date': line[2], 'producer':line[3]}
    mydict[line[0]] = info
print(mydict)
```

### Q6

```python
def sort_dict(d):
	return sorted(d.items(), key=lambda x: x[1], reverse=True)
 
print(sort_dict({3:1, 2:2, 1:3}))
```

### Q7

```python
mylist = str(input()).split()
mydict = {}

for i in mylist:
    mydict[i] = 1 if mydict.get(i) is None else mydict[i] + 1
for i in sorted(mydict, key=mydict.get, reverse=True):
    print(i, end = " ")
```

### Q8

```python
word_list = ["percussion", "supersonic", "car", "tree", "boy", "girl", "arc"]

def freq(word):
    freq_dict = {}
    for char in word:
        freq_dict[char] = freq_dict.get(char, 0) + 1
    return freq_dict

anagram_list = []
for word_1 in word_list:
    for word_2 in word_list:
        if word_1 != word_2 and (freq(word_1) == freq(word_2)):
            anagram_list.append(word_1)
print(anagram_list)
```

