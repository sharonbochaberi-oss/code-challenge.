code challenge.

Counting positives and summing negatives in an array
Merging two sorted linked lists

 1. Count Positives and Sum Negatives
Problem Statement

Given an array of integers:

Count how many numbers are positive (> 0)
Calculate the sum of negative numbers (< 0)
Ignore zeros
If the array is empty or null, return an empty array

Example
Input:
[1, 2, 3, -1, -2, 0]
Output:
[3, -3]

Approach

If the input is empty → return []
Initialize:
positive_count = 0
negative_sum = 0
Loop through each number:
If number > 0 → increment count
If number < 0 → add to sum
If number == 0 → ignore
Return [positive_count, negative_sum]


 2. Merge Two Sorted Linked Lists
 Problem Statement

You are given two sorted linked lists.

Merge them into one sorted linked list by reusing existing nodes.

 Example
Input:
list1 = [1, 2, 4]
list2 = [1, 3, 4]

Output:
[1, 1, 2, 3, 4, 4]

 Approach:

We repeatedly compare the heads of both lists:

Steps:
If one list is empty → return the other list

Compare current nodes:
Pick the smaller value node

Set its next pointer to the result of merging the remaining lists

Repeat until both lists are fully merged