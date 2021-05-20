# Lists

## Question 1 - Large

Write a program that reads an integer N from the user, then reads N more integers from the user and store them in a list. Then prints elements larger than the average of numbers held in the array.

| Input                                                        | Output     |
| ------------------------------------------------------------ | ---------- |
| 10 <br />1 <br />2 <br />3 <br />4 <br />5 <br />6 <br />7 <br />8 <br />9 <br />10 | 6 7 8 9 10 |
| 4 <br />4 <br />1 <br />3 <br />8                            | 8          |



## Question 2 - Let's Count

Write a function that takes a list and find frequency of each element in the list then prints. Assume the numbers in the list will be between 0 and 100 (inclusive).

| INPUT                  | OUTPUT                                                       |
| ---------------------- | ------------------------------------------------------------ |
| 5 10 2 5 50 5 10 1 2 2 | 1 --> 1 <br />2 --> 3 <br />5 --> 3 <br />10 --> 2 <br />50 --> 1 |



## Question 3 - Fifth Powers

List comprehensions might enable you to turn loop-based codes into one line elegant expressions. Write a program that takes 5 integers as input and prints a new list consisting of the fifth power of each number. Try to construct and print the new list in just one line.

| INPUT             | OUTPUT                      |
| ----------------- | --------------------------- |
| [1, 2, 3, 5, 0]   | [1, 32, 243, 3125, 0]       |
| [4, 1, 6, -2, -3] | [1024, 1, 7776, -32, -243]  |
| [-3, -6, 2, 9, 0] | [-243, -7776, 32, 59049, 0] |



## Question 4 - Pairs

Write a function which takes a list and a number X, then find all pairs in the list whose sum is equal to X.

- A number can not be a pair with itself. Pairs should consist of different numbers.
- You can print either (3,4) or (4,3) for one pair.
- You should print all the pairs even if they are same.

| INPUT                              | OUTPUT                                        |
| ---------------------------------- | --------------------------------------------- |
| [2, 4, 3, 5, 7, 8, 9], 7           | (2, 5) <br />(4, 3)                           |
| [2, 4, 3, 5, 6, -2, 4, 7, 8, 9], 7 | (2, 5) <br />(4, 3)<br />(3, 4) <br />(-2, 9) |



## Question 5 - To the left

Write a function which takes a list of numbers and an integer k and shifts the numbers to the left circularly by *k* and
return the shifted list.

| Input             | Output          |
| ----------------- | --------------- |
| [1, 2, 3, 4, 5] 2 | [3, 4, 5, 1, 2] |
| [2, 18, 6, 0] 3   | [0, 2, 18, 6]   |



## Question 6 - Reverse

Write a program which reads a list of integers from the user and store them in a list.

**a**. Then print them to the screen in reverse order.

**b.** Then reverse the order of these integers in the array and print the array.

| Input          | Output         |
| -------------- | -------------- |
| 3 1 -4 5 2     | 2 5 -4 1 3     |
| 15 7 2 89 8 12 | 12 8 89 2 7 15 |



## Question 7 - Remove X

Write a function that accepts a list and variable X and removes all occurrence of X from the list.

| INPUT                           | OUTPUT          |
| ------------------------------- | --------------- |
| [5, 20, 15, 20, 25, 50, 20], 20 | [5, 15, 25, 50] |



## Question 8 - Remove Consecutive Duplicates

Write a function that takes a list of integers then returns without consecutive duplicates.

| Input                                   | Output             |
| --------------------------------------- | ------------------ |
| [1, 1, 1, 1, 1, 2, 2, 2, 3, 2, 2, 4, 5] | [1, 2, 3, 2, 4, 5] |
| [0,0,0,0,0,0,0]                         | [0]                |



## Question 9 - Remove Duplicates

Write a function that takes a list of integers then returns without all duplicates.

| Input                                   | Output          |
| --------------------------------------- | :-------------- |
| [1, 1, 1, 1, 1, 2, 2, 2, 3, 2, 2, 4, 5] | [1, 2, 3, 4, 5] |
| [0,0,0,0,0,0,0]                         | [0]             |



## Question 10 - Odd Occurrences

Write a function that takes a list and prints the elements that occur 2n+1 times. If there is no element with odd number
of occurrences then it should not print anything.

| Input                                           | Output    |
| ----------------------------------------------- | --------- |
| [1, 1, 2, 3, 4, 2, 'apple', 'banana', 'banana'] | 3 4 apple |
| [2, 2, 3, 3, 2]                                 | 2         |
| [ 'a' , 'b' , 'c' , 'c' , 'b' , 'a' ]           |           |



## Question 11 - Slice List Sum

Write a function which takes a list of integers and an integer n. This function will 'slice' the initial list into smaller lists such that individual sums of elements in each smaller list exceed n the first time while reading the elements of the list from left to right.

| Input                                    | Output                                              |
| ---------------------------------------- | --------------------------------------------------- |
| [5, 3, 2, 1 ,4 ,51, 2, 1, 3, 5, 3, 5], 4 | [[5], [3, 2], [1, 4], [51], [2, 1, 3], [5], [3, 5]] |



## Question 12 - Inception

Write a program which reads two integers: N and M from the user. Then the program should read N more integers, then M
more integers from the user. Assume N < M < 50.

If the first combination of N integers appears at least once in the second combination of M integers, the program should
write the starting index of the first appearance in the second combination. Otherwise it should not print anything.

| Input                                              | Output |
| -------------------------------------------------- | ------ |
| 4 12 <br />4 5 6 5 <br />1 2 1 2 99 99 4 5 6 5 9 9 | 6      |
| 3 5 <br />2 2 2 <br />1 2 2 2 2 5                  | 1      |
| 3 5 <br />2 3 2 <br />1 2 2 2 5                    |        |



## Question 13 - Shuffle Double

Write a function which takes a list and shuffles in a specific way and then return it. The shuffle is as follows: odd number indexed elements are moved to the end of the list with their respective order. If you are confused, here is an example.

| Input                                      | Output                      |
| ------------------------------------------ | --------------------------- |
| [1, 2, 3, 4, 5, 6, 7, 8, 9] | [1, 3, 5, 7, 9, 2, 4, 6, 8] |



## Question 14 - Bubble Sort

Write a function that sorts elements of the list in ascending order.

| INPUT           | OUTPUT          |
| --------------- | --------------- |
| 4 2 8 6 7 3 1 5 | 1 2 3 4 5 6 7 8 |

Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in
wrong order.

**Example:**

**First Pass:**

- ( **5** **1** 4 8 2 ) –> ( **1** **5** 4 8 2 ), Here, algorithm compares the first two elements, and swaps since 5 >
  1.
- ( 1 **5** **4** 8 2 ) –> ( 1 **4** **5** 8 2 ), Swap since 5 > 4
- ( 1 4 **5** **8** 2 ) –> ( 1 4 **5** **8** 2 ), since these elements are already in order (8 > 5), no swap.
- ( 1 4 5 **8** **2** ) –> ( 1 4 5 **2** **8** ), Swap since 8 > 2.

The largest element is at the end.

**Second Pass:**

- ( **1** **4** 5 2 8 ) –> ( **1** **4** 5 2 8 )
- ( 1 **4** **5** 2 8 ) –> ( 1 **4** **5** 2 8 )
- ( 1 4 **5** **2** 8 ) –> ( 1 4 **2** **5** 8 ), Swap since 5 > 2
- ( 1 4 2 **5** **8** ) –> ( 1 4 2 **5** **8** )

**Third Pass:**

- ( **1** **4** 2 5 8 ) –> ( **1** **4** 2 5 8 )
- ( 1 **4** **2** 5 8 ) –> ( 1 **2** **4** 5 8 ), Swap since 4 > 2
- ( 1 2 **4** **5** 8 ) –> ( 1 2 **4** **5** 8 )
- ( 1 2 4 **5** **8** ) –> ( 1 2 4 **5** **8** )

Now, the array is already sorted, but our algorithm does not know if it is completed. The algorithm needs one whole pass
without any swap to know it is sorted.

**Fourth Pass:**

- ( **1** **2** 4 5 8 ) –> ( **1** **2** 4 5 8 )
- ( 1 **2** **4** 5 8 ) –> ( 1 **2** **4** 5 8 )
- ( 1 2 **4** **5** 8 ) –> ( 1 2 **4** **5** 8 )
- ( 1 2 4 **5** **8** ) –> ( 1 2 4 **5** **8** )



## Question 15 - Consecutive Combo

Write a function that returns *True* if two lists, when combined, form a consecutive sequence. <br>
A consecutive sequence is a sequence without any gaps in the integers, e.g. 1, 2, 3, 4, 5 is a consecutive sequence, but 1, 2, 4, 5 is not.<br>

**Notes:**<br>
The input lists will have unique values.<br>
The input lists can be in any order.<br>

| INPUT             | OUTPUT                      |
| ----------------- | --------------------------- |
| [7, 4, 5, 1], [2, 3, 6]   | True       |
| [1, 4, 6, 5], [2, 7, 8, 9] | False  |
| [1, 4, 5, 6], [2, 3, 7, 8, 10] | False |
| [44, 46], [45] | True |