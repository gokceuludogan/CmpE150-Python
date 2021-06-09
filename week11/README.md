# Files

## Question 1 - Split Paragraph

Write a program which reads the file named `paragraph.txt` under data directory and manipulates it. The file contains a paragraph with multiple sentences. The program must split this paragraph into sentences and write these sentence to a new file named `paragraph_splitted.txt` that will contain one sentence on each line.

| Input File                                                   | Output File                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| He had three simple rules by which he lived. The first was to never eat blue food. There was nothing in nature that was edible that was blue. People often asked about blueberries, but everyone knows those are actually purple. He understood it was one of the stranger rules to live by, but it had served him well thus far in the 50+ years of his life. | He had three simple rules by which he lived<br />There was nothing in nature that was edible that was blue<br />People often asked about blueberries, but everyone knows those are actually purple<br />He understood it was one of the stranger rules to live by, but it had served him well thus far in the 50+ years of his life |
| Eating raw fish didn't sound like a good idea. "It's a delicacy in Japan," didn't seem to make it any more appetizing. Raw fish is raw fish, delicacy or not. | Eating raw fish didn't sound like a good idea<br />"It's a delicacy in Japan," didn't seem to make it any more appetizing<br />Raw fish is raw fish, delicacy or not |

## Question 2 - Reverse Lines

Write a program that prompts for a file name and reverses each line of the file and writes the resulting list of lines to a new file.

| Input File                                                   | Output File                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Eating raw fish didn't sound like a good idea<br />"It's a delicacy in Japan," didn't seem to make it any more appetizing<br />Raw fish is raw fish, delicacy or not | aedi doog a ekil dnuos t'ndid hsif war gnitaE<br/>gniziteppa erom yna ti ekam ot mees t'ndid ",napaJ ni ycaciled a s'tI"<br/>ton ro ycaciled ,hsif war si hsif waR |

## Question 3 - Sort Words

Write a function which takes a file name as input, reads the file, splits into words, sorts these words alphabetically, and then prints the results to the console. 

| Input File                                                   | Output File                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| There was nothing in nature that was edible that was blue. People often asked about blueberries, but everyone knows those are actually purple. | People There about actually are asked blue. blueberries, but edible everyone in knows nature nothing often purple. that that those was was was |
| As she woke, she realized she was once again at a crossroads. Would it be another excuse or would she finally find the courage to pursue her dream? | As Would a again another at be courage crossroads. dream? excuse finally find her it once or pursue realized she she she she the to was woke, would |

## Question 4 - Pluralize

Write a program which takes a file name and reads file that has one word each line. It should pluralize only the words that is made up only letters and will print out the pluralized form of these words in to an output file called pluralWords.txt. If the last letter of a word is 'y', drop 'y' and add 'ies' (cherry to cherries). In other cases add 's' to that word (orange to oranges).
| input.txt                                                    | output.txt                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| lady <br> CMPE150 <br> phone <br> Mr.Nobody <br> area51 <br> 8ship <br> student <br> secretary <br> Dr.ErolBey <br> python_variable <br> Hello! <br> system | ladies <br> phones  <br> students <br> secretaries <br> systems |

## Question 5 - Correct Grades

Write a program which reads the file named `grades.txt` which has Midterm 1 grades on the first line, Midterm 2 grades on the second line and Final grades on the third line. Assume that each line has the same number of grades. Correct the grades such that nonnegative grades will be replaced by 0. Write the resulting grades to `corrected.txt`.

| grades.txt                                                   | corrected.txt                                                |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 70 85 0 -5 20 100 <br> 100 50 45 30 -10 90 <br>-3 50 30 25 60 85 | 70 85 0 0 20 100 <br> 100 50 45 30 0 90 <br> 0 50 30 25 60 85 |

## Question 6 - Calculate Grades

Write a program which reads the file corrected.txt and calculates the average grade of class. The weights of Midterm 1, Midterm2, and Final are %30, %30, and %40 respectively. Print the calculated average grade to console with rounding to two decimal.

| corrected.txt                                                | output |
| ------------------------------------------------------------ | ------ |
| 70 85 0 0 20 100 <br> 100 50 45 30 0 90 <br> 0 50 30 25 60 85 | 46.17  |

# Dictionary

## Question 1 - Different Types

Write a program that takes list of different types, and creates a dictionary which has each different type as keys and the list of elements of that type as as value. Then display all elements of each type like in the example.

| INPUT                                                        | OUTPUT                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [10, 4.20, False, 'Word', 'CMPE150', 30, 3.5, 9.99, 'oblivion', True, 68, 88, "88"] | <class 'int'> -> [10, 30, 68, 88]<br /> <class 'float'> -> [4.2, 3.5, 9.99] <br /><class 'bool'> -> [False, True]<br /> <class 'str'> -> ['Word', 'CMPE150', 'oblivion', '88'] |

## Question 2 - Letter Count

Write a program that takes a string, then create a dictionary which has letters as keys and the counts of that letters as values. Then sort that dictionary by descending values and print out the letters and the frequency of that letters to console.

| INPUT                     | OUTPUT                                                       |
| ------------------------- | ------------------------------------------------------------ |
| What we think, we become. | e -> 0.21 <br />w -> 0.16 <br />h -> 0.11 <br />t -> 0.11 <br />a -> 0.05 <br />b -> 0.05 <br />c -> 0.05<br /> i -> 0.05 <br />k -> 0.05 <br />m -> 0.05 <br />n -> 0.05 <br /o -> 0.05 |

## Question 3 - Zip Two Lists

Write a function that takes 2 lists, then returns a dictionary which has keys from the first one, values from the second one.

| INPUT                                                        | OUTPUT                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| list1 = ["melih", "burak", "ahmet", "recep", "melis"] list2 = [1,2,3,4,5] | {'melih': 1, 'burak': 2, 'ahmet': 3, 'recep': 4, 'melis': 5} |

## Question 4 - Dictionary Merge

Write a function that takes one or more dictionaries and combines them in one result dictionary. The keys in the given dictionaries can overlap. In that case you should combine all values in a list. Duplicate values should be preserved.

| Input                                              | Output                                         |
| -------------------------------------------------- | ---------------------------------------------- |
| {"A": 1, "B": 2} {"A": 3}                          | {"A": [1, 3]}, "B": [2]}                       |
| {"A": 1, "B": 2, "C": 3}                           | {"A": [1], "B": [2], "C": [3]}                 |
| {"A": 1, "B": 2, "C": 3} {"A": 4, "D": 5} {"A": 4} | {"A": [1, 4, 4], "B": [2], "C": [3], "D": [5]} |

## Question 5 - Data Collection

Write a program that reads lines from the input. Each line will be composed of 4 words, name of the game, genre of the game, year of release and the producer respectively. If a line is equal to "exit", stop reading. Store the games in a dictionary. Their values should also correspond to dictionaries composed of their genre, release_data and producer.

| Input                                                        | Output                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| RDR2 Action 2018 Rockstar<br />Fifa14 Sports 2013 EA<br />Borderlands Shooter 2009 Gearbox<br />Skyrim RPG 2011 Bethesda<br />Wall-E Platform 2008 THQ<br />exit | {'RDR2': {'genre': 'Action', 'release_date': '2018', 'producer': 'Rockstar'},<br/>'Fifa14': {'genre': 'Sports', 'release_date': '2013', 'producer': 'EA'},<br/>'Borderlands': {'genre': 'Shooter', 'release_date': '2009', 'producer': 'Gearbox'},<br/>'Skyrim': {'genre': 'RPG', 'release_date': '2011', 'producer': 'Bethesda'},<br/>'Wall-E': {'genre': 'Platform', 'release_date': '2008', 'producer': 'THQ'}} |

## Question 6 - Sorting Dictionary

Write a function that returns a sorted list of (key, value) tuples. The list must be sorted by the value and be sorted largest to smallest.

| Input                                     | Output                                         |
| ----------------------------------------- | ---------------------------------------------- |
| {3:1, 2:2, 1:3}                           | [(1,3), (2,2), (3,1)]                          |
| {'a' :5, 'b' :10, 'c' :2, 'd' :3, 'e' :8} | [('b',10), ('e',8), ('a',5), ('d',3), ('c',2)] |

## Question 7 - Word Frequency

Write a program that prompts the user for a sentence. Split the sentence into words and store the frequency of each word (number of occurrences). Then print the words in a sorted manner from most common to the least common. If there is a tie, print the word that comes first in the original sentence.

*Hint: You can use sorted(dict_, key=dict_.get) function to sort a dictionary according to the values. In order to get the reversed version of this, add reverse = True parameter.*

| INPUT                                                        | OUTPUT                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------- |
| "one two two three three four four four four"                | "four three two one"                                    |
| "fair is foul and foul is fair"                              | "fair is foul and"                                      |
| "How much wood would a woodchuck chuck if a woodchuck could chuck wood?" | "a woodchuck chuck How much wood would if could wood? " |

## Question 8 - Anagrams

Anagram is a word formed by rearranging the letters of a different word (heart, earth). Write a program that takes a word list and prints out all the anagrams in the word list.

| Input                                                        | Output                                     |
| ------------------------------------------------------------ | ------------------------------------------ |
| ["percussion", "supersonic", "car", "tree", "boy", "girl", "arc"] | ['percussion', 'supersonic', 'car', 'arc'] |

