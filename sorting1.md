### 排序
**按照时间复杂度分类**      
> O(n^2) time: insertion sort, selecting sort, bubble sort     
O(nlogn) time: heapsort, merge sort and quick sort     
O(n) time: counting sort, bucket sort and radix sort   

**不同方法的比较**     
heapsort is in-place (use constant space) but not stable (duplicate numbers' original relative order will be preserved)    
quicksort run O(n^2) time in worst case    
merge sort is stable but not in-place     

insertion sort适用于元素数量少的数列，以及基本排好序的数组       
部分排序（前k个最大/小元素）可以用heapsort提高时间复杂度到O(nlogk)    
如果元素的值的范围很小，采用counting sort (用array或者二叉树存储）    

Java Libraries   **
> **Arrays.sort(array)** is used to sort the array      
costs O(nlogn) time and O(n) time to sort a randomly ordered input array     
operates on arrays of objects that implement the Comparable interface    
**Collections.sort(list)** is used to sort the list     
internally proceeds by forming an array A and calling Arrays.sort     
costs O(nlogn) time and O(n) time to sort an array   
**Arrays.sort(array, comp)** and **Collections.sort(array, comp)**       
sort accoding to an explicit Comparator object with method compare(Object a, Object b) overwritten   
in Java 8, the anonymous Inner Comparator class replaced with Lambda expression     


