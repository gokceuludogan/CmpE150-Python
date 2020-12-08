# Lists and Tuples

## Question 1 - Reverse

Write a program which reads an integer N from the user, then reads N integers from the user and store them in a list.

**a**. Then print them to the screen in reverse order.

**b.** Then reverse the order of these integers in the array and print the array.

| Input                  | Output         |
| ---------------------- | -------------- |
| 5 <br />3 1 -4 5 2     | 2 5 -4 1 3     |
| 6 <br />15 7 2 89 8 12 | 12 8 89 2 7 15 |



## Question 2 - Let's Count

Write a function that takes a list and find frequency of each element in the list then prints. Assume the numbers in the list will be between 0 and 100 (inclusive).

| INPUT                           | OUTPUT                                                       |
| ------------------------------- | ------------------------------------------------------------ |
| 5 10 2 5 50 5 10 1 2 2 | 1 --> 1 <br />2 --> 3 <br />5 --> 3 <br />10 --> 2 <br />50 --> 1 |



## Question 3 - Inception 

Write a program which reads two integers: N and M from the user. Then the program should read N more integers, then M more integers from the user. Assume N < M < 50.

If the first combination of N integers appears at least once in the second combination of M integers, the program should write the starting index of the first appearance in the second combination. Otherwise it should not print anything.

| Input                                              | Output |
| -------------------------------------------------- | ------ |
| 4 12 <br />4 5 6 5 <br />1 2 1 2 99 99 4 5 6 5 9 9 | 6      |
| 3 5 <br />2 2 2 <br />1 2 2 2 2 5                  | 1      |
| 3 5 <br />2 3 2 <br />1 2 2 2 5                    |        |



## Question 4 - Pairs

Write a function which takes a list and a number X, then find all pairs in the list whose sum is equal to X.

- A number can not be a pair with itself. Pairs should consist of different numbers.
- You can print either (3,4) or (4,3) for one pair.
- You should print all the pairs even if they are same.

| INPUT                     | OUTPUT                                        |
| ------------------------- | --------------------------------------------- |
| [2, 4, 3, 5, 7, 8, 9], 7         | (2, 5) <br />(4, 3)                           |
| [2, 4, 3, 5, 6, -2, 4, 7, 8, 9], 7 | (2, 5) <br />(4, 3)<br />(3, 4) <br />(-2, 9) |



## Question 5 - fix34

Write a program which reads an integer N from the user, then reads N integers from the user to a list. Then rearrange the list so that every 3 is immediately followed by a 4. Do not move the 3's, but every other number may move. The list contains the same number of 3's and 4's, every 3 has number after it that is not a 3, and a 3 appears in the list before any 4.

| INPUT                 | OUTPUT        |
| --------------------- | ------------- |
| 4 <br />1 3 1 4       | 1 3 4 1       |
| 7 <br />1 3 1 4 4 3 1 | 1 3 4 1 1 3 4 |
| 4 <br />3 2 2 4       | 3 4 2 2       |



## Question 6 - Bubble Sort

Write a function that sorts elements of the list in ascending order.

| INPUT             | OUTPUT          |
| ----------------- | --------------- |
| 4 2 8 6 7 3 1 5 | 1 2 3 4 5 6 7 8 |

Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in wrong order.

Example:

First Pass:

- ( **5** **1** 4 2 8 ) –> ( **1** **5** 4 2 8 ), Here, algorithm compares the first two elements, and swaps since 5 > 1.
- ( 1 **5** **4** 2 8 ) –> ( 1 **4** **5** 2 8 ), Swap since 5 > 4
- ( 1 4 **5** **2** 8 ) –> ( 1 4 **2** **5** 8 ), Swap since 5 > 2
- ( 1 4 2 **5** **8** ) –> ( 1 4 2 **5** **8** ), Now, since these elements are already in order (8 > 5), algorithm does not swap them.

Second Pass:

- ( **1** **4** 2 5 8 ) –> ( **1** **4** 2 5 8 )
- ( 1 **4** **2** 5 8 ) –> ( 1 **2** **4** 5 8 ), Swap since 4 > 2
- ( 1 2 **4** **5** 8 ) –> ( 1 2 **4** **5** 8 )
- ( 1 2 4 **5** **8** ) –> ( 1 2 4 **5** **8** )

Now, the array is already sorted, but our algorithm does not know if it is completed. The algorithm needs one whole pass without any swap to know it is sorted.

Third Pass:

- ( **1** **2** 4 5 8 ) –> ( **1** **2** 4 5 8 )
- ( 1 **2** **4** 5 8 ) –> ( 1 **2** **4** 5 8 )
- ( 1 2 **4** **5** 8 ) –> ( 1 2 **4** **5** 8 )
- ( 1 2 4 **5** **8** ) –> ( 1 2 4 **5** **8** )


## Question 7 - Concatwise

Write a function that concatenates two lists index-wise.

| INPUT                 | OUTPUT        |
| --------------------- | ------------- |
| list1 = ["M", "na", "i", "Pat"]<br>list2 = ["y", "me", "s", "rick"] | ['My', 'name', 'is', 'Patrick']   |


## Question 8 - Combine Reverse

Write a function that iterates two lists simultaneously such that list1 should display item in original order and list2 in reverse order.

| INPUT                 | OUTPUT        |
| --------------------- | ------------- |
| list1 = [10, 20, 30, 40]<br>list2 = [100, 200, 300, 400] | 10 400<br>20 300<br>30 200<br>40 100   |


## Question 9 - Remove X

Write a function that accepts a list and variable X and removes all occurrence of X from the list.

| INPUT                 | OUTPUT        |
| --------------------- | ------------- |
| [5, 20, 15, 20, 25, 50, 20], 20   | [5, 15, 25, 50]   |