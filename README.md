# Selection Sort C

Selection sort is a sorting algorithm that selects the smallest element from an unsorted list in each iteration and places that element at the beginning of the unsorted list.

In selection sort, the smallest value among the unsorted elements of the array is selected in every pass and inserted to its appropriate position into the array. It is also the simplest algorithm. It is an in-place comparison sorting algorithm. In this algorithm, the array is divided into two parts, first is sorted part, and another one is the unsorted part. Initially, the sorted part of the array is empty, and unsorted part is the given array. Sorted part is placed at the left, while the unsorted part is placed at the right.

In selection sort, the first smallest element is selected from the unsorted array and placed at the first position. After that second smallest element is selected and placed in the second position. The process continues until the array is entirely sorted.

## Algorithm
    SELECTION SORT(arr, n)  
  
    Step 1: Repeat Steps 2 and 3 for i = 0 to n-1  
    Step 2: CALL SMALLEST(arr, i, n, pos)  
    Step 3: SWAP arr[i] with arr[pos]  
    [END OF LOOP]  
    Step 4: EXIT  
  
    SMALLEST (arr, i, n, pos)  
    Step 1: [INITIALIZE] SET SMALL = arr[i]  
    Step 2: [INITIALIZE] SET pos = i  
    Step 3: Repeat for j = i+1 to n  
    if (SMALL > arr[j])  
     SET SMALL = arr[j]  
    SET pos = j  
    [END OF if]  
    [END OF LOOP]  
    Step 4: RETURN pos  
    
## Selection Sort Complexity
Now, let's see the time complexity of selection sort in best case, average case, and in worst case. We will also see the space complexity of the selection sort.

1. Time Complexity
**Case	Time Complexity**


*   Best Case - O(n<sup>2</sup>)
*   Average Case - O(n<sup>2</sup>)
*   Worst Case - O(n<sup>2</sup>)

1. Best Case Complexity - It occurs when there is no sorting required, i.e. the array is already sorted. The best-case time complexity of selection sort is O(n<sup>2</sup>). 
2. Average Case Complexity - It occurs when the array elements are in jumbled order that is not properly ascending and not properly descending. The average case time complexity of selection sort is O(n<sup>2</sup>).
3. Worst Case Complexity - It occurs when the array elements are required to be sorted in reverse order. That means suppose you have to sort the array elements in ascending order, but its elements are in descending order. The worst-case time complexity of selection sort is O(n<sup>2</sup>).


2. Space Complexity
Space Complexity - O(1)
Stable - YES

**Please Note** - The space complexity of selection sort is O(1). It is because, in selection sort, an extra variable is required for swapping.

**OUTPUT:**

![image](https://user-images.githubusercontent.com/73773202/151299605-3e3ab4ff-e51a-43e6-b945-4d1dfc5a1dbd.png)


---
