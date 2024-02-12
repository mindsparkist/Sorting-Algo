# Sorting-Algo

The Soring algo today we will discuss is 
https://visualgo.net/en

## Bubble sort 
 - We have an array of integers and we want to sort them in ascending order.
 - Scan the array from left to right if the left item is bigger than the right we swap them
 - after every sort, the next largest value comes to the right
 - Time and space complexity 
 
|                |Best                          |Worst                         |
|----------------|-------------------------------|-----------------------------|
|Passes          |`O(1)`                         |`O(1)`            |
|comparison      |`o(n)`                         |`O(n)`            |
|Total           |`o(n)`                         |`o(n^2)`          |


## Selection sort
- Find the smallest value and move it to the smallest index 

|                |Best                          |Worst                         |
|----------------|-------------------------------|-----------------------------|
|Passes          |`O(n)`                         |`O(1)`            |
|comparison      |`o(n)`                         |`O(n)`            |
|Total           |`o(n^2)`                         |`o(n^2)`          |


## insertion sort 
- First Sort then insert
- Check the items that we have seen so far if they are greater than the items that we are checking then "SHIFT" it to right.

|                |Best                          |Worst                         |
|----------------|-------------------------------|-----------------------------|
|Passes          |`O(n)`                         |`O(1)`            |
|Shift           |`o(1)`                         |`O(n)`            |
|Total           |`o(n)`                         |`o(n^2)`          |

## Merge sort 
- Break an unsorted array into smaller arrays and merge them back to build shorted arrays.
- Example of divide and conquer algo 
- But this requires extra memory

|                |Best                          |Worst                         |
|----------------|-------------------------------|-----------------------------|
|Dividing        |`O(log n)`                     |`O(log n)`            |
|Merge           |`o(n)`                         |`O(n)`            |
|Total           |`o(n log n)`                   |`o(n log n)`          |

### In-place merge sort
Sure! Let's break down the concept of in-place merge sort in a simple way for a beginner in computer science.

### Merge Sort Overview:
Merge sort is a popular sorting algorithm that follows the divide-and-conquer strategy. It divides the input array into smaller sub-arrays, sorts them recursively, and then merges them back together to produce a sorted array.

### In-Place Merge Sort:
In traditional merge sort, we create new arrays to hold the sorted sub-arrays during the merge step. However, in in-place merge sort, we aim to perform the merging operation without using any additional arrays. Instead, we manipulate the elements within the original array itself.

### Basic Steps:
1. **Divide:** Similar to regular merge sort, we start by dividing the array into smaller halves until we have sub-arrays with only one element each. This process is done recursively.

2. **Merge:** After the division, we start merging the smaller sub-arrays back together. However, in in-place merge sort, we need to be careful about how we perform this merging operation to ensure that it's done in the original array itself.

3. **Merging in Place:** To merge two sorted sub-arrays within the original array, we use a technique that involves shifting elements within the array to make room for the merged elements. This shifting process allows us to maintain the sorted order while using only the original array.

### Example:
Let's say we have an array `[3, 8, 12, 15, 6, 9, 10]` and we want to sort it using in-place merge sort.

1. **Divide:** We divide the array into smaller sub-arrays: `[3, 8, 12, 15]` and `[6, 9, 10]`.

2. **Merge:** Now, we start merging the sub-arrays back together in place. For this, we compare elements from both sub-arrays and place them back into the original array in sorted order.

3. **Merging in Place:** During the merging process, we may need to shift elements within the array to make room for the merged elements while maintaining the sorted order.

4. **Final Result:** After merging, the array becomes `[3, 6, 8, 9, 10, 12, 15]`, which is sorted.

### Key Points:
- In-place merge sort doesn't require extra space for creating new arrays during the merge step.
- It achieves the same result as traditional merge sort but with a different approach to merging.

Understanding in-place merge sort can be a bit challenging initially, but with practice and implementation, you'll get a better grasp of how it works.

 ## Quick Sort
-	It is an example of  divide-and-conquer algorithm 
-	check here https://algorithm-visualizer.vercel.app/sorting#
-	we can say an item is sorted if the items before the mentioned item are smaller and the items after it are larger.
-	check video here https://www.youtube.com/watch?v=7h1s2SojIRw&pp=ygUScXVpY2sgc2VhcmNoIGFiZHVs

|                |Best                          |Worst                         |
|----------------|-------------------------------|-----------------------------|
|positioning     |`O(n)`                               |`O(n)`            |
|# number Of times      |`o(log n)`                    |`O(n)`      |
|Total           |`o(n logn)`                         |`o(n^2)`          |
|Space           |`o(n logn)`                         |`o(n)`          |



