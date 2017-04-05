### Array
Array is a data structure for storage at continuous locations, each element is indexed by continuous int number.
It supports location, insertion, deletion, iteration and search operation.

### Properties
* no holes (no gap after removing an element)
* fixed size (after initialization)
* O(1) time to retrieve or update any element A[i]
* O(1) time to add or remove at the end
* O(n) time to add and remove at any arbitrary location (begin, middle).
    We shift all elements over one spot to create/remove a hole at the indicated index,
    if the index is out of boundary, throw new IndexOutOfBoundsException() (Java)
* O(n) time to search in unsorted array and O(logn) time to search in sorted array
* O(n) time to iterate an array

### Resizing: handle the insertion an item to a full array
- allocate a new array with additional memory and copy over the entries from the original array
- worst case runtime: O(n) time  
- amortised constant time: due to the infrequenct operation
