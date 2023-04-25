# Insertion-Sorting

The simple sorting algorithm known as insertion sort functions similarly to how you would arrange playing cards in your hands. In a sense, the array is divided into sorted and unsorted parts. Values are chosen and assigned to the appropriate positions in the sorted part of the data from the unsorted part.

![234086383-73ff3103-d2c8-475b-a495-d2974589f146](https://user-images.githubusercontent.com/125882453/234398657-c08854f3-0dfd-432e-bb13-2c85a52f457a.png)


Characteristics of Insertion Sort:

One of the simplest algorithms, with straightforward implementation, is this one. For modest data values, insertion sort is generally effective. Insertion sort is adaptive in nature, hence it is suitable for data sets that have already undergone some degree of sorting.


  procedure insertionSort(A: list of sortable items)
  
     n = length(A)
     for i = 1 to n - 1 do
         j = i
         while j > 0 and A[j-1] > A[j] do
             swap(A[j], A[j-1])
             j = j - 1
         end while
     end for
  end procedure
  
  This algorithm sorts an array of items by repeatedly taking an element from the unsorted portion of the array and inserting it into its correct position in the sorted portion of the array.

The procedure takes a single argument, ‘A’, which is a list of sortable items. The variable ‘n’ is assigned the length of the array A. The outer for loop starts at index ‘1’ and runs for ‘n-1’ iterations, where ‘n’ is the length of the array. The inner while loop starts at the current index i of the outer for loop and compares each element to its left neighbor. If an element is smaller than its left neighbor, the elements are swapped. The inner while loop continues to move an element to the left as long as it is smaller than the element to its left. Once the inner while loop is finished, the element at the current index is in its correct position in the sorted portion of the array. The outer for loop continues iterating through the array until all elements are in their correct positions and the array is fully sorted.
