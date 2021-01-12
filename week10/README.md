# Dictionaries

## Question 1 - Split the Bill

Write a program that splits the bill.

For example, 3 friends go out together: A spends £20, B spends £15, and C spends £10. The function should return a dictionary showing that A should receive £5, B should receive £0, and C should pay £5.

| Input                         | Output     |
| ----------------------------- | ---------- |
| {'A':20, 'B':15, 'C':10}      | {'A':5, 'B':0, 'C':-5}  | 

## Question 2 - Different Types

Write a script that takes list of different types, and creates a dictionary which has each different type as keys and the list of elements of that type as as value. Then display all elements of each type like in the example.

| INPUT                           | OUTPUT                                                       |
| ------------------------------- | ------------------------------------------------------------ |
| [10, 4.20, False, 'Word', 'CMPE150', 30, 3.5, 9.99, 'oblivion', True, 68, 88, "88"] | <class 'int'>  ->  [10, 30, 68, 88]<br><class 'float'>  ->  [4.2, 3.5, 9.99]<br><class 'bool'>  ->  [False, True]<br><class 'str'>  ->  ['Word', 'CMPE150', 'oblivion', '88']|


## Question 3 - Sorting Dictionary

Write a function that returns a sorted list of (key, value) tuples. The list must be sorted by the value and be sorted largest to smallest.

| Input                         | Output     |
| ----------------------------- | ---------- |
| {3:1, 2:2, 1:3}   | [(1,3), (2,2), (3,1)] |
| {'a' :5, 'b' :10, 'c' :2, 'd' :3, 'e' :8} | [('b',10), ('e',8), ('a',5), ('d',3), ('c',2)] | 


## Question 4 - Letter Count 

Write a script that takes a string, then create a dictionary which has letters as keys and the counts of that letters as values. Then sort that dictionary by descending values and print out the letters and the frequency of that letters to console.

| INPUT                           | OUTPUT                                                       |
| ------------------------------- | ------------------------------------------------------------ |
| What we think, we become. | e -> 0.21<br>w -> 0.16<br>h -> 0.11<br>t -> 0.11<br>a -> 0.05<br>b -> 0.05<br>c -> 0.05<br>i -> 0.05<br>k -> 0.05<br>m -> 0.05<br>n -> 0.05<br>o -> 0.05|


## Question 5 - Dictionary Merge

Write a function that takes one or more dictionaries and combines them in one result dictionary. The keys in the given dictionaries can overlap. In that case you should combine all values in a list. Duplicate values should be preserved.

| Input                         | Output     |
| ----------------------------- | ---------- |
| {"A": 1, "B": 2} <br> {"A": 3}     | {"A": [1, 3]}, "B": [2]} |
| {"A": 1, "B": 2, "C": 3}      | {"A": [1], "B": [2], "C": [3]} |
| {"A": 1, "B": 2, "C": 3} <br> {"A": 4, "D": 5} <br> {"A": 4} | {"A": [1, 4, 4], "B": [2], "C": [3], "D": [5]} |



## Question 6 - Zip Two Lists 

Write a function that takes 2 lists, then returns a dictionary which has keys from the first one, values from the second one.

| INPUT                           | OUTPUT                                                       |
| ------------------------------- | ------------------------------------------------------------ |
| list1 = ["melih", "burak", "ahmet", "recep", "melis"] <br>list2 = [1,2,3,4,5] |{'melih': 1, 'burak': 2, 'ahmet': 3, 'recep': 4, 'melis': 5}
|



# Sets

## Question 1 - List to Distinct

Write a function that takes a list as an argument and returns distinct elements of the list. The order of elements
doesn't matter.

| Input                | Output         |
| -------------------- | -------------- |
| 3 5 4 4 7 11 2 8     | 2 3 4 5 7 8 11 |
| 1 8 1 1 27 32 17  32 | 32 1 8 17 27   |

## Question 2 - Set Operations

Write a function that takes two sets then prints union, intersection and difference operations between them.

| Input             | Output |
| ----------------- | ------ |
| A = {1, 2, 3, 4, 5, 6} <br>B = {1, 1, 2, 7, 11}    | A ∪ B = {1, 2, 3, 4, 5, 6, 7, 11} <br>A ∩ B = {1, 2}<br>A / B = {3, 4, 5, 6}<br>B / A = {11, 7}   |


## Question 3 - Diff

Write a program that find the missing and additional values of the first list from the second list.

| Input                              | Output                                                       |
| ---------------------------------- | ------------------------------------------------------------ |
| [1, 2, 3, 4, 5, 6] [4, 5, 6, 7, 8] | Missing values in list1 = [8, 7]<br />Additional values in list1 = [1, 2, 3] |
| [1, 3, 5, 7] [2, 4, 6, 8]          | Missing values in list1 = [2, 4, 6, 8]<br />Additional values in list1 = [1, 3, 5, 7]|

## Question 4 - Distinct String

**A distinct string** is a string whose all characters occurs only once.

Write a function that takes a string as an argument and checks whether given string is distinct or not.

| Input     | Output |
| --------- | ------ |
| dwarf     | True   |
| violate   | True   |
| violation | False  |

## Question 5 - Numgram

**A numgram** is a string containing all digits (0, 1, 2, 3, 4, 5, 6, 7, 8, 9).

Write a program which takes a string as input and prints whether this string is numgram or not.

| Input                 | Output        |
| --------------------- | ------------- |
| SAS102BAD347 HELP5689 | Numgram       |
| Wh4t 4 811ll7 q0386n  | Not a numgram |



