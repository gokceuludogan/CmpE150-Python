## Question 1 - Voweeels

```python
def vowel(s):
    max_length, length = 0, 0
    for c in s:
        if c in 'oeaiu':
            length += 1
        else:
            length = 0
        max_length = max(length, max_length)
    return max_length

print(vowel("happy beaar"))
print(vowel("how you doin?"))
print(vowel("aiaiai"))
print(vowel("try"))
```

## Question 2 - Palindrome

```python
def is_palindrome(str):
    return str == str[::-1]
```

## Question 3 - Lower/Upper Counts

```python
str = "HeLLo WoRLD"
lower_count, upper_count = 0, 0
for c in str:
    lower_count += c.islower()
    upper_count += c.isupper()

print(upper_count, lower_count)
```

## Question 4 - Requirements

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

## Question 5 - Ing

```python
str = 'abc'
if len(str) >= 3:
    if str.endswith('ing'):
        str = str + 'ly'
    else:
        str = str + 'ing'
print(str)
```

## Question 6 - Trim

#### Question 6a

```python
str = input()
str = input.strip()
print(str)
```

#### Question 6b

```python
sentence = input()
characters = input()
sentence = sentence.lstrip(characters)
print(sentence)
```

```python
sentence = input()
characters = input()
sentence = sentence.rstrip(characters)
print(sentence)
```

## Question 7  - Length

```python
sentence = input()
words = sentence.split()
lengths = [len(w) for w in words]
shortest_index = lengths.index(min(lengths))
longest_index = lengths.index(max(lengths))
print(words[shortest_index], words[longest_index])
```

## Question 8 - Not poor

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

## Question 9 - Word Cases

```python
def modify(str):
    words = str.split()
    new_str = ''
    for ix, word in enumerate(words):
        if ix % 2 == 0:
            new_str += word.upper() + ' '
        else:
            new_str += word.lower() + ' '
    return new_str

def modify2(str):
    return ' '.join([word.upper() if ix % 2 == 0 else word.lower() for ix, word in enumerate(str.split())])

print(modify('stop making sponge bob memes'))
print(modify2('stop making sponge bob memes'))

```

## Question 10 - Capitalize First Letters

```python
def capitalize(sentence):
    return " ".join([word[0].upper() + word[1:].lower() for word in sentence.split()])

# Title method performs this 
print("perFecT NORMAL sentence".title())

print(capitalize("perFecT NORMAL sentence"))
print(capitalize("A true friend overlooks your failures and tolerates your success"))
print(capitalize("a WITTY saying proves nOthing"))

```

## Question 11 - Initials

### Question 11a

```python
def name(s):
    # split the string into a list
    l = s.split()
   	return ' '.join([l[0].upper() for w in l])

s = "mohandas karamchand gandhi"
print(name(s))
```

### Question 11b

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

## Question 12 - Alphabetical order

```python
items = input("Input comma separated sequence of words")
words = [word for word in items.split(",")]
print(",".join(sorted(list(set(words)))))
```