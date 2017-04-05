### 排序
**按照时间复杂度分类**      
> O(n^2) time: insertion sort, selecting sort, bubble sort     
O(nlogn) time: heapsort, merge sort and quick sort     
O(n) time: counting sort, bucket sort and radix sort   

**不同方法的比较**     
heapsort is in-place (use constant space) but not stable (duplicate numbers' original relative order will be preserved)    
quicksort run O(n^2) time in worst case    
merge sort is stable but not in-place     

insertion sort适用于元素数量少的数列，  
部分排序（前k个最大/小元素）可以用heapsort提高时间复杂度到O(nlogk)    
如果元素的值的范围很小，采用counting sort (用array或者二叉树存储）   

