# Strings

## Question 1 - SpOnGeBoB MeMe

Write a function that takes a string and returns it by converting it into a spongebob meme. Every letter with odd index should be lowercase and every letter with even index should be uppercase.

| Input                                  | Output                                 |
| -------------------------------------- | -------------------------------------- |
| stop making sponge bob memes           | StOp mAkInG SpOnGe bOb mEmEs           |
| CMPE will be fun in the next few years | CmPe wIlL Be fUn iN ThE NeXt fEw yEaRs |


## Question 2 - Convert string to camel case
There are different naming conventions: lowercase lower_case_with_under_scores UPPERCASE CamelCase.

Write a function that converts dash/underscore delimited words into camel casing. Every word should start with a uppercase letter and continue with lowercase letters. (known as Upper Camel Case or Pascal Case. 

| Input                         | Output     |
| ----------------------------- | ---------- |
| to_camel_case | ToCamelCase |
| Hard_exam-pLe | HardExamPle |
| unnecessarily-LONG-Example | UnnecessarilyLongExample |

## Question 3 - Abbreviate

Write a function called abbreviation() that takes a string st.<br>
If st has strictly more than 14 characters: returned string:<br>
* has the same first and last two characters as st.
* the characters in the middle should be replaced by the number of characters being replaced. (if you are replacing 15 characters return value should look like ww15ww)<br>

Else return st as is.

| INPUT  | OUTPUT |
| ------ | ------ |
| afyonkarahisarlarstiramadiklarimizdan |  af33an    |
| helo|  helo     |


## Question 4 - Stop gninnipS My sdroW!
Write a function that takes a string of one or more words, and returns the same string, but with all five or more letter words reversed.

| Input                         | Output     |
| ----------------------------- | ---------- |
| This is another test | This is rehtona test |
| You know you’re in love when you can’t fall asleep because reality is finally better than your dreams. | You know er’uoy in love when you t’nac fall peelsa esuaceb ytilaer is yllanif retteb than your .smaerd|
| Challenges are what make life interesting and overcoming them is what makes life meaningful. | segnellahC are what make life gnitseretni and gnimocrevo them is what sekam life .lufgninaem |

## Question 5 - Requirements

Write a function which takes a password as parameter and return whether the password is valid or not. The password has the following requirements:

* The password must be at least 6 characters and at most 20 characters.

* It must contain at least one lowercase letter, one uppercase letter, and one number.

| Input   | Output |
| ------- | ------ |
| Covid19 | True   |
| 123456  | False  |

## Question 6  - Length

Write a program to find shortest and largest word in a given string.

| Input                              | Output         |
| ---------------------------------- | -------------- |
| the house is a long way from here  | a house        |
| This room is exclusively for women | is exclusively |


## Question 7 - Alphabetical order

Write a program that accepts a comma separated sequence of words as input and prints the words in sorted form (alphanumerically).

| Input                                | Output                       |
| ------------------------------------ | ---------------------------- |
| red, white, black, red, green, black | black, black, green, red, red, white |


## Question 8 - Second Most Common
Write a program that prompts the user for a string. Then find and print out the second most repeated character (lowercase) in the string (not case-sensitive). Do not take whitespaces into consideration.

<em> Hint : You can use replace() method of strings to get rid of whitespaces. Then you can use count() method to check if a character is in the string. </em>
<em> Alternatively, you can use a dictionary to store the occurrences of each character. </em>

| INPUT  | OUTPUT |
| ------ | ------ |
| " Hey there partner! " |  "r"    |
| "CaN you CAn a CAN as a canner CaN CAn a CAN?"|  "n"     |
|  "    LEsSer leather weaTheREd weTTer weathEr BettEr"| "t"   |

## Question 9 - Not poor

Write a function to find the first appearance of the substring **'not'** and **'poor'** from a given string, if **'not'** follows the **'poor'**, replace the whole '**not'...'poor'** substring with **'good'. ** and return the resulting string.

| Input                        | Output              |
| ---------------------------- | ------------------- |
| The lyrics is not that poor! | The lyrics is good! |
| The lyrics is poor!          | The lyrics is poor! |


## Question 10 - Find and replace

Write a function that takes 3 strings ``input``, ``a`` and ``b`` and replaces all the instances of ``a`` in ``input`` with ``b``.

| ``input``                         |``a``|``b``| Output     |
| ----------------------------- |----|---| ---------- |
| This is another test |"is"|"is not"| This not is not another test |
| I mean, it went badly last time but surely it will go much better this time. |"it"|"filling zepplins with hydrogen"|I mean, filling zepplins with hydrogen went badly last time but surely filling zepplins with hydrogen will go much better this time.|
| Test test TeSt te st TEst teSt crest TEA  | "st TE" |" test "|Test test TeSt te testst teSt cretestA |


## Question 11 - Reading Backwards
You are a very skilled artist who can read sentences backwards. Jury will test you by giving you four strings. <code>i</code> value will be given by the jury. 
* Read the first one changing the order of the words in backwards. 
* Read the second one by changing the letters of the words as well. 
* Read the third one backwards but starting from the i<sup>th</sup> word (according to the given order) without changing the words. 
* Read the last one, again starting from the ith word but changing the words as well. 

| INPUT  | OUTPUT |
| ----- | ------ |
| But then I took an arrow in the knee <br> i = 6 | knee the in arrow an took I then But <br>eenk eht ni worra na koot I neht tuB <br>in arrow an took I then But <br>ni worra na koot I neht tuB |
| I want to play a game <br> i = 12 | game a play to want I <br>emag a yalp ot tnaw I <br>play to want I <br>yalp ot tnaw I |
| It can't be for nothing <br> i = 4 | nothing for be can't It <br>gnihton rof eb t'nac tI <br>be can't It <br>eb t'nac tI |

