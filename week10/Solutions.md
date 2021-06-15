# Strings

## Question 1 - SpOnGeBoB MeMe

```python
# https://www.codewars.com/kata/5982619d2671576e90000017
def sponge_bob(sentence):
    return "".join([sentence[i].lower() if i % 2 else sentence[i].upper() for i in range(len(sentence))])

def spongebob(input_str):
    result_str = ""
    for i, s in enumerate(input_str):
        if i % 2 == 0:
            result_str += s.upper()
        else:
            result_str += s.lower()

    return result_str

print(sponge_bob("stop making sponge bob memes"))
```


## Question 2 - Convert string to camel case

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
    return ''.join([word.title() for word in words])

print(to_camel_case("to_camel_case"))
print(to_camel_case("Hard_exam-pLe"))
print(to_camel_case("unnecessarily-LONG-Example"))
```

## Question 3 - Abbreviate

```python
def abbreviation(st):
    if (len(st) <= 14):
        return st
    else:
        return st[0:2] + str(len(st) - 4) + st[-2:]
```

## Question 4 - Stop gninnipS My sdroW

```python
# https://www.codewars.com/kata/5264d2b162488dc400000001/train/python
def spin_words(sentence):
    return " ".join([word[::-1] if len(word) > 4 else word for word in sentence.split()])


print(spin_words("This is another test"))
print(spin_words(
    "You know you’re in love when you can’t fall asleep because reality is finally better than your dreams."))
print(spin_words("Challenges are what make life interesting and overcoming them is what makes life meaningful."))
```

## Question 5 - Requirements

```python
def is_valid(password):
    length = len(password)
    if length < 6 or length > 20:
        return False
    lower, upper, digit = 0, 0, 0
    for c in password:
        lower += c.islower()
        upper += c.isupper()
        digit += c.isdigit()
    return lower >= 1 and upper >= 1 and digit >= 1    
```

## Question 6  - Length

```python
sentence = input()
words = sentence.split()
lengths = [len(w) for w in words]
shortest_index = lengths.index(min(lengths))
longest_index = lengths.index(max(lengths))
print(words[shortest_index], words[longest_index])
```

## Question 7 - Alphabetical order

```python
items = input("Input comma separated sequence of words")
words = [word.strip() for word in items.split(",")]
print(", ".join(sorted(list(words))))
```


## Question 8 - Second Most Common
```python
string = str(input())
modified = string.replace(" ", "").lower()
Max = 0
secondMax = 0
second = ''
first = ''
for i in modified:
    occur = modified.count(i)
    if(occur > Max):
        second = first
        first = i
        secondMax = Max
        Max = occur
    elif(occur < Max and occur > secondMax):
        second = i
        secondMax = occur
print(first, second)
```

## Question 9 - Not poor

```python
def not_poor(str1):
  snot = str1.find('not')
  spoor = str1.find('poor')
  if spoor > snot and snot > 0 and spoor > 0:
  	  str1 = str1.replace(str1[snot:(spoor+4)], 'good')
      return str1
  else:
      return str1
print(not_poor('The lyrics is not that poor!'))
print(not_poor('The lyrics is poor!'))
```

## Question 10 - Find and replace

```python
def find_and_replace(string, a, b):
    output = ""
    i = 0
    while i <= len(string) - len(a):
        if string[i:i + len(a)] == a[0:len(a)]:
            output += b
            i += len(a)
        else:
            output += string[i]
            i += 1
    return output

def find_and_replace2(string, a, b):
    ix = 0
    while string.find(a, ix) != -1:
        ix = string.find(a, ix)
        string = string[:ix] + b + string[ix+len(a):]
        ix = ix + len(b)
    return string

print(find_and_replace("This is another test", "is", "is not"))
print(find_and_replace("I mean, it went badly last time but surely it will go much better this time.", "it", "filling zeppelins with hydrogen"))
print(find_and_replace("Test test TeSt te st TEst teSt crest TEA", "st TE", "test"))
```


## Question 11 - Reading Backwards
```python
string = input()
i = int(input())

words = string.split(" ")

#1
words.reverse()
print(" ".join(words))
#2
changed_words = list(words)
for i in range(0,len(changed_words)):
    changed_words[i] = changed_words[i][::-1]
print(" ".join(changed_words))
#3
i_reverse = len(words)-i +1
print(" ".join(words[i_reverse:]))
#4
print(" ".join(changed_words[i_reverse:]))
```
