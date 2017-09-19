# Integers and Arrays Interview Practice
In this assignment, you'll design and implement some of integer number and array manipulation functions that are commonly asked during interviews.
If you think of multiple approaches to solve the problem, implement the solution which minimizes space complexity. Explain the other approaches, and your decision in comments above the code.

## Exercises
Design and implement a method for each of the following. Do not use Ruby library provided functionality. You may use `.length`. Share and explain the time and space complexity for each method.
1. Design and implement a method that accepts two non-negative integers as parameters and that returns the number of digits that match in the two integers. Two digits match if they are equal and have the same position relative to the end of the number (i.e. starting with the ones digit). In other words, the method should compare the last digits of each number, the second-to-last digits of each number, the third-to-last digits of each number, and so forth, counting how many pairs match.
For example, for  input values of (1072503891, 62530841), the method would compare as follows:
```
1 0 7 2 5 0 3 8 9 1
    | | | | | | | |
    6 2 5 3 0 8 4 1
```
The method should return 4 in this case because 4 of these pairs match (2-2, 5-5, 8-8, and 1-1).
2. Design and implement a method that checks if the digits in the input positive integer forms a palindrome. The method returns true if the digits in the input form a palindrome. The method returns false otherwise.
For example, 12521 and 4554 are palindromes. 326725 is not a palindrome.
3. Design and implement a method that computes factorial of the input non-negative integer and returns it. Factorial of a number, 'n' is represented as 'n!' and is defined as follows:
   - '0!' = '1'
   - 'n!' = 'n * (n-1)!' if 'n' > 0
   -    = 'n * (n-1) * (n-2) * ... * 1'
For example, 3! = 3 * 2 * 1 = 6. 6! = 720.
4. Design and implement a method to compute the nth fibonacci number in the series starting with 0.
   - Fibonacci series starting with 0 looks like this: 0 1 1 2 3 5 8 13 21 34 55 89 144 ...
   - The next number in the series is the sum of the previous two numbers in the series.
   - For example:
     - The 0th fibonacci number is 0
     - The 1st fibonacci number is 1
     - The 6th fibonacci number is 8
5. Design and implement a method that takes two integer arrays and returns their intersection. The two input arrays have non repeating elements.
   - For example, intersection of [2, 3, 4] and [4, 5, 6] is [4]
   - intersection of [50, 43, 25, 72] and [25, 36, 43, 50, 80] is [50, 25, 43]
   - intersection of [9, 30, 42] and [56, 34, 90, 32] is []
6. Design and implement a method that updates the input matrix. The input matrix i.e. two-dimensional array contains only '0's and '1's. If any number in the array is found to be '0', the method updates all the numbers in the corresponding row as well as the corresponding column to be '0'.
   - For example if the input is:
```
1 1 1
1 0 1
1 1 1
1 1 0
```
should get updated to:
```
1 0 0
0 0 0
1 0 0
0 0 0
```
7. Design and implement a method that checks that for the given matrix, where number of rows are equal to number of columns whether the sum of each row matches the sum of the corresponding column i.e. sum
of numbers in row 'i' is the same as the sum of numbers in column 'i' for 'i' ranging from '0' to 'row.length-1'. If this is the case, the method return true. Otherwise, it return false.
   - For example for the following input, the method should return true. (Sum of 0th row and 0th column is 10, sum of 1st row as well as the 1st column is 18 and so on.)
```
1 2 3 4
9 5 3 1
0 3 5 6
0 8 3 6
```

Update the integers_and_arrays.rb file to implement the above methods.
