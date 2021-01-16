# Strings

## Question 1 - Remove Odds

```python
def even_string(my_str):
    res_str = ""
    for i in range(len(my_str)):
        if i % 2 == 0:
            res_str += my_str[i]
    return res_str

def even_string2(my_str):
    res_str = ""
    for i, c in enumerate(my_str):
        if i % 2 == 0:
            res_str += c
    return res_str

print(even_string("abcdef"))
print(even_string2("abcdef"))

```

## Question 2 - Initials

### Question 2a

```python
def name(s):
    # split the string into a list
    l = s.split()
    return ' '.join([w[0].upper() for w in l])

s = "mohandas karamchand gandhi"
print(name(s))
```

### Question 2b

```python
def name(s):
    # split the string into a list
    l = s.split()
    new = ""

    # traverse in the list
    for i in range(len(l) - 1):
        s = l[i]
        # adds the capital first character
        new += (s[0].upper() + '.')
        # l[-1] gives last item of list l. We
    # use title to print first character in
    # capital.
    new += l[-1].title()
    return new

s = "mohandas karamchand gandhi"
print(name(s))
```

## Question 3 - Stop gninnipS My sdroW!

```python
def spin_words(my_str):
    words = my_str.split()
    res_str = ""
    for word in words:
        if len(word) > 4:
            res_str += word[::-1] + " "
        else:
            res_str += word + " "
    res_str = res_str.strip()
    return res_str

def spin_words2(my_str):
    words = my_str.split()
    return " ".join([word[::-1] if len(word) > 4 else word for word in words])

print(spin_words("This is another test"))
print(spin_words2("This is another test"))

```

## Question 4 - Convert string to camel case

```python
# https://www.codewars.com/kata/517abf86da9663f1d2000003/train/python
def to_camel_case(text):
    result = ""
    flag = True
    for i in text:
        if i in ["-", "_"]:
            flag = True
        else:
            result += i.upper() if flag else i.lower()
            flag = False

    return result

def to_camel_case_s(text):
    text = text.replace('-', '_')
    words = text.split('_')
    return ''.join([word.capitalize() for word in words]) # word.capitalize() -> word[0].upper() + word[1:].lower()


print(to_camel_case("to_camel_case"))
print(to_camel_case("Hard_exam-pLe"))
print(to_camel_case("unnecessarily-LONG-Example"))

```

## Question 5 - Find and replace

```python
def find_replace(input, a, b):
    res_str = ""
    i = 0
    while i <= len(input) - len(a):
        if input[i:i + len(a)] == a:
            res_str += b
            i += len(a)
        else:
            res_str += input[i]
            i += 1
    if i < len(input):
        res_str += input[i:]
    return res_str

def find_replace2(input, a, b):
    ix = 0
    while input.find(a, ix) != -1:
        ix = input.find(a, ix)
        input = input[:ix] + b + input[ix+len(a):]
        ix = ix + len(b)
    return input

print(find_replace("This is another test", "is", "is not"))
print(find_replace2("This is another test", "is", "is not"))
print("This is another test".replace("is", "is not"))

```

# Files

## Question 1 - Save input

```python

string = input()

f = open("inputs.txt", "w")
f.write(string)
f.close()

# Alternative: closes file implicitly
"""with open("inputs.txt", "a+") as f:
    f.write(string)"""

```

## Question 2 - To lines

```python

with open("data/q2.txt", "r") as f:
    file_str = f.read()
    sentences = file_str.split(".")
    sentences = [s.strip() for s in sentences]
    sentences = sentences[:-1]

with open("data/q2_splitted.txt", "w") as f:
    for sentence in sentences:
        f.write(sentence + ".\n")

```

## Question 3 - Reverse 

```python

with open("data/q2_splitted.txt", "r") as f:
    lines = f.readlines()

lines = [l.strip() for l in lines]
lines = [l[::-1] for l in lines]

with open("data/reverse.txt", "w") as f:
    f.write("\n".join(lines))

```

## Question 4 - Count occurrences

```python

import string

with open("data/q2.txt", "r") as f:
    txt = f.read()

words = txt.split()
words = [w.strip(string.punctuation).lower() for w in words]

words_set = list(set(words))
counts = [0] * len(words_set)

for word in words:
    counts[words_set.index(word)] += 1

for word, count in zip(words_set, counts):
    print(word, count)

```

Alternative: (using dictionary)

```python

import string

with open("data/q2.txt", "r") as f:
    txt = f.read()

words = txt.split()
words = [w.strip(string.punctuation).lower() for w in words]

dict = {}

for word in words:
    if word not in dict:
        dict[word] = 1
    else:
        dict[word] += 1
        
print(dict)

```

## Question 5 - Pluralize

```python
#This is from another university's intro to computing class. I hope it's ok to ask. It was due to October 26.

with open('input.txt','r') as f:
    words = [line.strip() for line in f.readlines()]
    alphas = [word for word in words if word.isalpha()]

with open('output.txt','w') as f:
    f.write("\n".join([word+'s' if word[-1] != 'y' else word[:-1]+'ies' for word in alphas]))
```

## Question 6 - Grades

### Question 6a

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

### Question 6b

```python
with open("corrected.txt", 'r') as f:  
    mt1 = [float(grade) for grade in f.readline().split()]
    mt2 = [float(grade) for grade in f.readline().split()]
    final = [float(grade) for grade in f.readline().split()]
n= len(mt1)
avg = 0.3*sum(mt1)/n + 0.3*sum(mt1)/n + 0.4*sum(final)/n
print(round(avg,2))
```