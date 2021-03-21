# Strings

## Question 1 - Remove Odds

Write a program to remove the characters which have odd index values of a given string.

| Input  | Output |
| ------ | ------ |
| abcdef | ace    |
| python | pto    |

## Question 2 - Initials

#### Q2a

Write a function which takes a name and returns the initials of the name.

| Input            | Output |
| ---------------- | ------ |
| Evan Rachel Wood | E R W  |
| Jude Law         | J L    |
| Jane Doe         | J D    |

#### Q2b

Write a function which takes a name and returns the initials of a name (uppercase) with last name(with first alphabet in uppercase) written in full separated by dots.

| Input                      | Output     |
| -------------------------- | ---------- |
| geeks for geeks            | G.F.Geeks  |
| mohandas karamchand gandhi | M.K.Gandhi |

## Question 3 - Stop gninnipS My sdroW!

Write a function that takes a string of one or more words, and returns the same string, but with all five or more letter words reversed.

| Input                                                        | Output                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| This is another test                                         | This is rehtona test                                         |
| You know you’re in love when you can’t fall asleep because reality is finally better than your dreams. | You know er’uoy in love when you t’nac fall peelsa esuaceb ytilaer is yllanif retteb than your .smaerd |
| Challenges are what make life interesting and overcoming them is what makes life meaningful. | segnellahC are what make life gnitseretni and gnimocrevo them is what sekam life .lufgninaem |

## Question 4 - Convert string to camel case

There are different naming conventions: lowercase lower_case_with_under_scores UPPERCASE CamelCase.

Write a function that converts dash/underscore delimited words into camel casing. Every word should start with a uppercase letter and continue with lowercase letters. (known as Upper Camel Case or Pascal Case.

| Input                      | Output                   |
| -------------------------- | ------------------------ |
| to_camel_case              | ToCamelCase              |
| Hard_exam-pLe              | HardExamPle              |
| unnecessarily-LONG-Example | UnnecessarilyLongExample |

## Question 5 - Find and replace

Write a function that takes 3 strings `input`, `a` and `b` and replaces all the instances of `a` in `input` with `b`.

| `input`                                                      | `a`     | `b`                              | Output                                                       |
| ------------------------------------------------------------ | ------- | -------------------------------- | ------------------------------------------------------------ |
| This is another test                                         | "is"    | "is not"                         | This not is not another test                                 |
| I mean, it went badly last time but surely it will go much better this time. | "it"    | "filling zepplins with hydrogen" | I mean, filling zepplins with hydrogen went badly last time but surely filling zepplins with hydrogen will go much better this time. |
| Test test TeSt te st TEst teSt crest TEA                     | "st TE" | " test "                         | Test test TeSt te testst teSt cretestA                       |

# Files

## Question 1 - Save input

**a)** Write a program that will open a file named **inputs.txt** and reads user input and write this input into this file.

**b)** Update your program to save the file to a different directory using `os` module.

## Question 2 - To lines

Write a program which reads the file named `q2.txt` under data directory and manipulates it. The file contains a paragraph with multiple sentences. The program must split this paragraph into sentences and write these sentence to a new file named `q2_splitted.txt` that will contain one sentence on each line.

| q2.txt                                                       | q2_splitted.txt                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s. It has survived not only five centuries but also the leap into electronic typesetting, remaining essentially unchanged. | Lorem Ipsum is simply dummy text of the printing and typesetting industry.<br />Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.<br />It has survived not only five centuries but also the leap into electronic typesetting, remaining essentially unchanged. |

## Question 3 - Reverse 

Write a program that prompts for a file name and reverses each line of the file and writes the resulting list of lines to a new file.

## Question 4 - Count occurrences

Write a program which takes a file name and reads the file and splits into words, then counts the occurrence of each word and prints the result to console.

## Question 5 - Pluralize

Write a program which takes a file name and reads file that has one word each line. It should pluralize only the **words that is made up only letters** and will print out the pluralized form of these words in to an output file called `pluralWords.txt`. If the last letter of a word is 'y', drop 'y' and add 'ies' (cherry to cherries). In other cases add 's' to that word (orange to oranges).

| input.txt                                                    | pluralWords.txt                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| lady <br> CMPE150 <br> phone <br> Mr.Nobody <br> area51 <br> 8ship <br> student <br> secretary <br> Dr.ErolBey <br> python_variable <br> Hello! <br> system | ladies <br> phones  <br> students <br> secretaries <br> systems |

## Question 6 - Grades

### Question 6a

Write a program which reads the file named `grades.txt` which has Midterm 1 grades on the first line, Midterm 2 grades on the second line and Final grades on the third line. Assume that each line has the same number of grades. Correct the grades such that nonnegative grades will be replaced by 0. Write the resulting grades to `corrected.txt`.

| grades.txt                                                   | corrected.txt                                               |
| ------------------------------------------------------------ | ----------------------------------------------------------- |
| 70 85 0 -5 20 100 <br>100 50 45 30 -10 90 <br>-3 50 30 25 60 85 | 70 85 0 0 20 100 <br>100 50 45 30 0 90 <br>0 50 30 25 60 85 |

### Question 6b

Write a program which reads the file `corrected.txt` and calculates the average grade of class. The weights of Midterm 1, Midterm2, and Final are %30, %30, and %40 respectively. Print the calculated average grade to console with rounding to two decimal.

| corrected.txt                                               | output |
| ----------------------------------------------------------- | ------ |
| 70 85 0 0 20 100 <br>100 50 45 30 0 90 <br>0 50 30 25 60 85 | 44.17  |