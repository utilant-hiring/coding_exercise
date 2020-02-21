# Lucky 13s

## Numbers with "13-snippets"

Suppose a number can be said to have a "13-snippet" if there is a consecutive sequence of digits whose sum is 13. For example, the number 43917 has a single 13-snippet:

4<b><ins>391</ins></b>7

Some numbers can be shown to have more than one 13-snippet, such as 3472041:

3<b><ins>472</ins></b>041  
3<b><ins>4720</ins></b>41  
34<b><ins>7204</ins></b>1

## Numbers that are "13-snippet Complete"

Now, suppose a number is considered "13-snippet _complete_" if every digit in the number is part of a 13-snippet. For example, the number 28311 is 13-snippet complete:

<b><ins>283</ins></b>11  
2<b><ins>8311</ins></b>

## Exercise:

In a separate file, write a function that takes in an iterable of integers, and returns the count of 13-snippet complete numbers found in the iterable.

Usage of the function might look like:
```python
>>> my_list = [ 43917, 3472041, 28311 ]
>>> count_13_snippet_complete(my_list)
1
```
