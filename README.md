# Problem-1-Hunny-Hunt - Data Structures and Algorithms
Data Structures and Algorithms

#Question
Write a function linear_search() to help Winnie the Pooh locate his lost items. The function accepts a list items and a target value as parameters. The function should return the first index of target in items, and -1 if target is not in items. Do not use any built-in functions.

Walk through of the question:
The question is asking that a list containing items will be check to see if our target value can be found. If our target is seen, then we return it otherwise we return a negative answer.

This is a typical array question.

Edge cases to consider
1. Empty list
2. Target not in list
3. One target in the list
4. Duplicates of the target in the list
5. Target at the end of the list

Approach chosen:
Linear Search
Trade Off: Simplicity Over Performance


Algorithm/Brute Force:
Step 1: Start at the first element of the list.
Step 2: Compare it with the target.
Step 3: If it matches, return the index.
Step 4: If not, move to the next element.
Step 5: Repeat until you find the target or reach the end.

Code in Python:
def linear_search(items, target):
    if not items:
        return -1  #targeting edge case

    for i in range(len(items)):
          if items[i] == target:
              return i

    return -1

Time complexity in the worse case scenario is O(n) because we will check through each element once. So we start at first, if it does not correspond with target we move to the next until we get to the end of the list.


Time complexity in the best case scenario is O(1) where we find the target at the beginning of the list so we don’t have to search through the entire list


Tradeoff of Linear search to other possible options like binary search is simplicity over performance. 

NB: Ideally  Linear Search is best for shorter list, were the list get longer options like binary search can be considered. 

Space Complexity:
The space complexity is O(1) because no extra memory and data structure is needed.


