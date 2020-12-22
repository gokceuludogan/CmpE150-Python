## Question 1 - Voweeels
Write a function which takes a string that all characters are lowercase and returns the length of longest sequence of consecutive vowels. It should return 0 for the empty string. Vowels are a,e,i,o,u. 

| Input                         | Output     |
| ----------------------------- | ---------- |
| "happy beaar" | 3 |
| "how you doin?" | 2 |
| "aiaiai" | 6 |
| "try" | 0 |

## Question 2 - Palindrome

Write a function to check whether given string is palindrome or not. A palindrome is a word, number, phrase, or other sequence of characters which reads the same backward as forward.

| Input | Output |
| ----- | ------ |
| madam | True   |
| radix | False  |

## Question 3 - Lower/Upper Counts

Write a program to calculate the number of uppercase and lowercase letters in a string.

| Input            | Output |
| ---------------- | ------ |
| CMPE will be fun | 9 4    |
| HeLLo WoRLD      | 7 3    |

## Question 4 - Requirements

Write a function which takes a password as parameter and return whether the password is valid or not. The password has the following requirements:

* The password must be at least 6 characters and at most 20 characters.

* It must contain at least one lowercase letter, one uppercase letter, and one number.

| Input   | Output |
| ------- | ------ |
| Covid19 | True   |
| 123456  | False  |

## Question 5 - Ing

Write a program to add **'ing'** at the end of a given string (length should be at least 3). If the given string already ends with **'ing'** then add **'ly'** instead. If the string length of the given string is less than 3, leave it unchanged.

| Input  | Output   |
| ------ | -------- |
| abc    | abcing   |
| string | stringly |

## Question 6 - Trim

#### Q6a 

Write a program to trim both leading and trailing white space characters in a string

| Input                   | Output   |
| ----------------------- | -------- |
| "    Hi all           " | "Hi all" |

#### Q6b

Write a program which takes two strings sentence and a sequence of characters and

* remove these characters only from the beginning of the sentence. 

  | Input                                                | Output                                |
  | ---------------------------------------------------- | ------------------------------------- |
  | 12.23this is string example....wow!!!23.11<br />123. | this is string example....wow!!!23.11 |

* remove these characters only from the end of the sentence. 

  | Input                                                | Output                                |
  | ---------------------------------------------------- | ------------------------------------- |
  | 12.23this is string example....wow!!!23.11<br />123. | 12.23this is string example....wow!!! |

## Question 7  - Length

Write a program to find shortest and largest word in a given string.

| Input                              | Output         |
| ---------------------------------- | -------------- |
| the house is a long way from here  | a house        |
| This room is exclusively for women | is exclusively |

## Question 8 - Not poor

Write a function to find the first appearance of the substring **'not'** and **'poor'** from a given string, if **'not'** follows the **'poor'**, replace the whole '**not'...'poor'** substring with **'good'. ** and return the resulting string.

| Input                        | Output              |
| ---------------------------- | ------------------- |
| The lyrics is not that poor! | The lyrics is good! |
| The lyrics is poor!          | The lyrics is poor! |

## Question 9 - Word Cases

Write a function that takes a string and returns it by modifying it such that every word with odd index should be lowercase and every word with even index should be uppercase.

| Input                                  | Output                                 |
| -------------------------------------- | -------------------------------------- |
| stop making sponge bob memes           | STOP making SPONGE bob MEMES           |
| CMPE will be fun in the next few years | CMPE will BE fun IN the NEXT few YEARS |

## Question 10 - Capitalize First Letters

Write a function that takes a string and for each word convert first letter to uppercase and other letters to lowercase. (You don't have to worry about punctuations, you can use split function however you can try it as a challenge. For example: "A bad written ,horrible sentence.And it continues" -> "A Bad Written ,Horrible Sentence.And It Continues")

| Input                         | Output     |
| ----------------------------- | ---------- |
| perFecT NORMAL sentence | Perfect Normal Sentence |
| A true friend overlooks your failures and tolerates your success | A True Friend Overlooks Your Failures And Tolerates Your Success|
| a WITTY saying proves nOthing| A Witty Saying Proves Nothing|

## Question 11 - Initials

#### Q11a

Write a function which takes a name and returns the initials of the name.

| Input            | Output |
| ---------------- | ------ |
| Evan Rachel Wood | E R W  |
| Jude Law         | J L    |
| Jane Doe         | J D    |

#### Q11b

Write a function which takes a name and returns the initials of a name (uppercase) with last name(with first alphabet in uppercase) written in full separated by dots.

| Input                      | Output     |
| -------------------------- | ---------- |
| geeks for geeks            | G.F.Geeks  |
| mohandas karamchand gandhi | M.K.Gandhi |

## Question 12 - Alphabetical order

Write a program that accepts a comma separated sequence of words as input and prints the unique words in sorted form (alphanumerically).

| Input                                | Output                       |
| ------------------------------------ | ---------------------------- |
| red, white, black, red, green, black | black, green, red, white,red |

