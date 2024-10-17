# Sorting_Algorithm
Experiment_20

## Contents
- [Aim](#aim)
- [Software Used](#software-used)
- [Theory](#theory)
  * [Definition](#Definition)
  * [Properties](#Properties-of-Sorting-Algorithms)
  * [Advantages](#Advantages-of-Sorting-Algorithms)
  * [Types](#Types-of-Sorting-Algorithm)
- [Algorithms](#algorithms)
- [Conclusion](#conclusion)

## Aim: 
To Study and Implement Sorting Algorithm.

## Software Used:
VS Code , Dev C++

## Theory:
### Sorting ALgorithms Defination:
A Sorting Algorithm is used to rearrange a given array or list of elements according to a comparison operator on the elements. The comparison operator is used to decide the new order of elements in the respective data structure.
For Example: The below list of characters is sorted in increasing order of their ASCII values. That is, the character with a lesser ASCII value will be placed first than the character with a higher ASCII value.
Sorting refers to rearrangement of a given array or list of elements according to a comparison operator on the elements. The comparison operator is used to decide the new order of elements in the respective data structure. Sorting means reordering of all the elements either in ascending or in descending order.
![image](https://github.com/user-attachments/assets/3efcdfde-8d10-43f1-82bd-509cda71dbc4)

### Properties of the Sorting Algorithm
Sorting algorithms can be characterized by several properties that help evaluate their efficiency and suitability for different tasks. Here are the key properties:
1. **Time Complexity**:
   - **Best Case**: Minimum time taken for a sorted input.
   - **Average Case**: Expected time taken for random inputs.
   - **Worst Case**: Maximum time taken for the least favorable input.
   Common complexities:
   - O(n log n): Merge Sort, Quick Sort (average case)
   - O(n²): Bubble Sort, Insertion Sort, Selection Sort (worst case)
2. **Space Complexity**:
   - The amount of extra memory required beyond the input data.
   - In-place sorting algorithms (like Quick Sort and Heap Sort) use O(1) or O(log n) additional space.
   - Out-of-place algorithms (like Merge Sort) require O(n) additional space.
3. **Stability**:
   - A stable sort maintains the relative order of records with equal keys.
   - Stable algorithms: Merge Sort, Insertion Sort.
   - Unstable algorithms: Quick Sort, Heap Sort.
4. **Adaptability**:
   - An adaptive sorting algorithm takes advantage of existing order in the input.
   - For example, Insertion Sort is adaptive and performs well on partially sorted arrays.
5. **Comparison-Based vs Non-Comparison-Based**:
   - Comparison-based sorts (like Quick Sort and Merge Sort) compare elements to determine order.
   - Non-comparison-based sorts (like Counting Sort and Radix Sort) use specific properties of the input data and can achieve better time complexities under certain conditions.
6. **Iterative vs Recursive**:
   - Some algorithms are naturally implemented recursively (like Merge Sort), while others can be implemented iteratively (like Bubble Sort).
7. **Performance on Different Data Types**:
   - Some algorithms perform better on specific types of data, such as nearly sorted data or data with many duplicates.

### Advantages of Sorting Algorithms:
 Sorting algorithms offer several advantages that can greatly impact the efficiency and usability of data processing. Here are some key benefits:
1. **Improved Search Efficiency**:
   - Sorted data allows for faster search algorithms, such as binary search, which operates in O(log n) time compared to O(n) for linear search.
2. **Simplified Data Management**:
   - Sorting organizes data, making it easier to understand and analyze. It aids in data visualization and reporting.
3. **Enhanced Performance in Other Algorithms**:
   - Many algorithms, like merge algorithms and certain graph algorithms, perform better or are simpler to implement when data is sorted.
4. **Facilitates Duplicate Removal**:
   - Sorting can simplify the process of identifying and removing duplicates in datasets.
5. **Data Integrity**:
   - Sorted data can help in maintaining data integrity by allowing easier identification of outliers or anomalies.
6. **Ease of Merging**:
   - When merging datasets, having them sorted can simplify the merging process, leading to more efficient data handling.
7. **Improved Performance in Databases**:
   - Many database operations, like indexing, benefit from sorted data, leading to faster retrieval and processing times.
8. **Better Memory Utilization**:
   - Some sorting algorithms are in-place, meaning they require minimal additional memory, which is beneficial for memory-constrained environments.
9. **Adaptability**:
   - Certain algorithms (like Insertion Sort) are adaptive, meaning they perform better on partially sorted data, making them useful in dynamic scenarios.
10. **Flexibility**:
    - Various sorting algorithms are available, allowing you to choose one that best fits your specific data characteristics and performance requirements.

## Types of Sorting Algorithm:
## 1. Insertion Sort:
Insertion sort is a simple sorting algorithm that works by iteratively inserting each element of an unsorted list into its correct position in a sorted portion of the list. It is like sorting playing cards in your hands. You split the cards into two groups: the sorted cards and the unsorted cards. Then, you pick a card from the unsorted group and put it in the right place in the sorted group.
- We start with second element of the array as first element in the array is assumed to be sorted.
- Compare second element with the first element and check if the second element is smaller then swap them.
- Move to the third element and compare it with the first two elements and put at its correct position
- Repeat until the entire array is sorted.
- ![image](https://github.com/user-attachments/assets/721b9e81-262b-4c1e-9397-2c19fee93d67)

## 2. Bubble Sort:
Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in the wrong order. This algorithm is not suitable for large data sets as its average and worst-case time complexity are quite high.
- We sort the array using multiple passes. After the first pass, the maximum element goes to end (its correct position). Same way, after second pass, the second largest element goes to second last position and so on.
- In every pass, we process only those elements that have already not moved to correct position. After k passes, the largest k elements must have been moved to the last k positions.
- In a pass, we consider remaining elements and compare all adjacent and swap if larger element is before a smaller element. If we keep doing this, we get the largest (among the remaining elements) at its correct position.
## Step 1:
  ![image](https://github.com/user-attachments/assets/4cc1f189-9f7d-40e6-923c-69fab7c747ca)
## Step 2:
  ![image](https://github.com/user-attachments/assets/94c7576a-3bf8-4a4f-9eeb-b908772b1b8c)
## Step 3:
  ![image](https://github.com/user-attachments/assets/9af10392-849d-4d7b-9575-595c8952766b)

## Selection Sort:
Selection Sort is a comparison-based sorting algorithm. It sorts an array by repeatedly selecting the smallest (or largest) element from the unsorted portion and swapping it with the first unsorted element. This process continues until the entire array is sorted.
- First we find the smallest element and swap it with the first element. This way we get the smallest element at its correct position.
- Then we find the smallest among remaining elements (or second smallest) and move it to its correct position by swapping.
- We keep doing this until we get all elements moved to correct position.
Certainly! Here’s a simple step-by-step explanation of the Selection Sort algorithm:

### Selection Sort Steps
1. **Start with the first element**:
   - Assume the first element of the array is the smallest.
2. **Find the smallest element**:
   - Compare this element with the rest of the elements in the array to find the smallest one.
3. **Swap**:
   - Once you find the smallest element, swap it with the first element of the array.
4. **Move to the next position**:
   - Now, consider the next element as the starting point (the second element) and repeat the process:
     - Assume this new starting element is the smallest.
     - Compare it with the rest of the unsorted elements to find the smallest one.
     - Swap if necessary.
5. **Repeat**:
   - Continue this process for each position in the array:
     - Each time you find the smallest element from the unsorted portion, move it to its correct position in the sorted portion of the array.
6. **Finish when sorted**:
   - Repeat until you have gone through all the elements. By the time you reach the last element, the entire array will be sorted.
  
## Algorithm Insertion Sort:
1. **Start from the second element**:
   - Begin with the second element of the array (index 1). Assume the first element (index 0) is already sorted.
2. **Store the current element**:
   - Store the current element in a variable (e.g., `current`).
3. **Find the correct position**:
   - Compare `current` with the elements in the sorted portion (to its left).
   - Start from the element just before `current` and move backward:
     - If the current element is smaller than the compared element, shift the compared element one position to the right.
4. **Insert the current element**:
   - Once you find the correct position (where the compared element is less than or equal to `current`), insert `current` into this position.
5. **Repeat**:
   - Move to the next element and repeat the process until the entire array is sorted.
6. **Output the sorted array**:
   - After sorting, print the sorted array.

### Example Walkthrough
Given the array: `[45, 23, 86, 12, 9]`
- **1st Pass** (i = 1):
  - `current = 23`
  - Compare with `45`, shift `45` right → `[45, 45, 86, 12, 9]`
  - Insert `23` → `[23, 45, 86, 12, 9]`
- **2nd Pass** (i = 2):
  - `current = 86`
  - No shifts needed → `[23, 45, 86, 12, 9]`
- **3rd Pass** (i = 3):
  - `current = 12`
  - Compare with `86`, shift `86` right.
  - Compare with `45`, shift `45` right.
  - Compare with `23`, shift `23` right → `[23, 23, 45, 86, 9]`
  - Insert `12` → `[12, 23, 45, 86, 9]`
- **4th Pass** (i = 4):
  - `current = 9`
  - Compare with `86`, shift `86`.
  - Compare with `45`, shift `45`.
  - Compare with `23`, shift `23`.
  - Compare with `12`, shift `12` → `[12, 12, 23, 45, 86]`
  - Insert `9` → `[9, 12, 23, 45, 86]`
### Final Sorted Array
The sorted array will be: `[9, 12, 23, 45, 86]`.
The code you provided implements the **Bubble Sort** algorithm. Here’s a simple step-by-step explanation of how it works:

### Bubble Sort Algorithm
1. **Start with the first element**:
   - Begin with the first element of the array.
2. **Compare adjacent elements**:
   - For each pair of adjacent elements (from the beginning of the array), compare them.
3. **Swap if necessary**:
   - If the first element of the pair is greater than the second element, swap them.
4. **Repeat for the entire array**:
   - Continue this process for all pairs in the array. After one full pass, the largest element will "bubble up" to the end of the array.
5. **Reduce the range**:
   - After each complete pass through the array, the next largest element will be in its correct position. Thus, reduce the range of comparison for the next pass (ignore the last sorted elements).
6. **Repeat until sorted**:
   - Continue the process until you make a complete pass without any swaps, which means the array is sorted.
7. **Output the sorted array**:
   - After sorting, print the sorted array.

### Example Walkthrough
Given the array: `[23, 12, 56, 144, 78]`
- **1st Pass**:
  - Compare `23` and `12`: swap → `[12, 23, 56, 144, 78]`
  - Compare `23` and `56`: no swap.
  - Compare `56` and `144`: no swap.
  - Compare `144` and `78`: swap → `[12, 23, 56, 78, 144]`
- **2nd Pass**:
  - Compare `12` and `23`: no swap.
  - Compare `23` and `56`: no swap.
  - Compare `56` and `78`: no swap.
  - Compare `78` and `144`: no swap.
- **3rd Pass**:
  - Compare `12` and `23`: no swap.
  - Compare `23` and `56`: no swap.
  - Compare `56` and `78`: no swap.
- **4th Pass**:
  - Compare `12` and `23`: no swap.
  - Compare `23` and `56`: no swap.
After the last pass with no swaps, the array is confirmed sorted.
### Final Sorted Array
The sorted array will be: `[12, 23, 56, 78, 144]`.
The code you provided implements the **Selection Sort** algorithm. Here’s a simple step-by-step explanation of how it works:

### Selection Sort Algorithm
1. **Start with the first element**:
   - Assume the first element of the array is the minimum.
2. **Find the minimum element**:
   - Loop through the unsorted portion of the array (starting from the current index) to find the smallest element.
3. **Update the minimum index**:
   - If you find an element smaller than the current minimum, update the index of the minimum element (`min_index`).
4. **Swap**:
   - After the inner loop completes, if the smallest element found is not at the current index, swap it with the element at the current index.
5. **Move to the next position**:
   - Repeat the process for the next index, treating it as the new starting point.
6. **Finish when sorted**:
   - Continue until you have gone through all the elements. By the end, the array will be sorted.
7. **Output the sorted array**:
   - After sorting, print the sorted array.

### Example Walkthrough
Given the array: `[23, 12, 56, 144, 78]`
- **1st Pass** (i = 0):
  - Start with `min_index = 0` (23).
  - Compare with `12` (update `min_index` to 1).
  - Compare with `56`, `144`, and `78` (no changes).
  - Swap `23` with `12` → `[12, 23, 56, 144, 78]`.
- **2nd Pass** (i = 1):
  - Start with `min_index = 1` (23).
  - Compare with `56`, `144`, and `78` (no changes).
  - No swap needed.
- **3rd Pass** (i = 2):
  - Start with `min_index = 2` (56).
  - Compare with `144` and `78` (update `min_index` to 4).
  - Swap `56` with `78` → `[12, 23, 78, 144, 56]`.
- **4th Pass** (i = 3):
  - Start with `min_index = 3` (144).
  - Compare with `56` (update `min_index` to 4).
  - Swap `144` with `56` → `[12, 23, 78, 56, 144]`.
- **5th Pass** (i = 4):
  - Only one element left, no action needed.
### Final Sorted Array
The sorted array will be: `[12, 23, 56, 78, 144]`.

## Conclusion:
We learnt to use the concepts of Sorting Algorithm and types of Sorting Algorithm such as Insertion sort, bubble sort, selection sort.


   

