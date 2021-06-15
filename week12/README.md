



# Dictionaries

## Question 1 - Name Length to Age Ratio

Write a function that takes a dictionary consisting of string:int values.
The key values are names of and int are their ages.
You need to return a list that contains their name length to age ratio in order.
Note: Don't count spaces

**Example-1 code snippet:**

```
a = {"Frederick Vought": 103, "Homelander": 52, "William Butcher": 56}

print(name_to_age_ratio(a))
```

**Example-1 Expected Output:**

```
[0.14563106796116504, 0.19230769230769232, 0.25]
```

**Example-2 code snippet:**

```
b = {"Sirus": 6012, "Maven": 9901, "Kalandra": 5123}

print(name_to_age_ratio(b))
```

**Example-2 Expected Output:**

```
[0.00083166999334664, 0.000504999495000505, 0.0015615850087839158]
```

## Question 2 - Word Frequency

Write a program that prompts the user for a sentence. Split the sentence into words and store the frequency of each word (number of occurrences). Then print the words in a sorted manner from most common to the least common. If there is a tie, print the word that comes first in the original sentence.

*Hint: You can use sorted(dict_, key=dict_.get) function to sort a dictionary according to the values. In order to get the reversed version of this, add reverse = True parameter.*

| INPUT                                                        | OUTPUT                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------- |
| "one two two three three four four four four"                | "four three two one"                                    |
| "fair is foul and foul is fair"                              | "fair is foul and"                                      |
| "How much wood would a woodchuck chuck if a woodchuck could chuck wood?" | "a woodchuck chuck How much wood would if could wood? " |

## Question 3 - Vasya - Clerk

The new "Avengers" movie has just been released! There are a lot of people at the cinema box office standing in a huge line. Each of them has a single 100, 50 or 25 dollar bill. An "Avengers" ticket costs 25 dollars.

Vasya is currently working as a clerk. He wants to sell a ticket to every single person in this line.

Can Vasya sell a ticket to every person and give change if he initially has no money and sells the tickets strictly in the order people queue?

Return YES, if Vasya can sell a ticket to every person and give change with the bills he has at hand at that moment. Otherwise return NO.

| Input                 | Output | Explanation                                                  |
| --------------------- | ------ | ------------------------------------------------------------ |
| [25, 25, 50]          | YES    |                                                              |
| [25, 100]             | NO     | Vasya will not have enough money to give change to 100 dollars |
| [25, 25, 50, 50, 100] | NO     | Vasya will not have the right bills to give 75 dollars of change (you can't make two bills of 25 from one of 50) |

# Sets

## Question 1 - Set Operations

Write a function that takes two sets then prints union, intersection and difference operations between them.

| Input                                       | Output                                                       |
| ------------------------------------------- | ------------------------------------------------------------ |
| A = {1, 2, 3, 4, 5, 6} B = {1, 1, 2, 7, 11} | A ∪ B = {1, 2, 3, 4, 5, 6, 7, 11} A ∩ B = {1, 2} A / B = {3, 4, 5, 6} B / A = {11, 7} |

## Question 2 - Eligible to graduate?

You are given 2 sets one of which is the set of all courses that has to be taken to graduate from CmpE department. Other one is the courses that has been taken by a student so far. Write a function indicating whether student can graduate or not.

| Input                                                        | Output       |
| ------------------------------------------------------------ | ------------ |
| {"CmpE150","CmpE160","CmpE220","CmpE250","CmpE260"} {"Cmpe150"} | Not Eligible |

## Question 3 - How good friends can they be?

People need to have common things to be friends. Let's say we have a set for every person consisting of the ID's of their personality traits. Two people can make as better friendship as the sum of their common personality trait IDs. Write a function that calculates the sum of common personality trait IDs.

| Input                 | Output |
| --------------------- | ------ |
| {1,2,3,4,5} {4,5,6,7} | 9      |

## Question 4 - Anagram

Write a function that takes two strings as arguments and returns whether these strings consist of same letters. Ignore case.

| Input             | Output |
| ----------------- | ------ |
| Listen silent     | True   |
| triANGLE integral | True   |
| caution action    | False  |

