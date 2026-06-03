Problem 1 : Rotate Matrix by 90 degree 
My fav problem.
Appraoch : 
1. Rotating a matrix by 90 degree gives the same result as finding transpose of the matrix and reversing all the rows of it.
2. To find the transpose of a matrix, we swap the elements of matrix[i][j] with the element at matrix[j][i] expect for the diagonal matrix. ( it will be the same anyways ).
3. Basically it.

Time complexity  : O(n^2)  - because we are doing transpose once with O(n^2 ) and then reversing each row again O(n^2).


Problem 2 : Merge Interval

My Approach :
1. Visualise this, you have certain intervals, like each point on a catesian plane, Each interval forms a line, Now you have to merge overlapping lines.
2. Now the given interval array is not sorted, so we will first sort it according to the first element of the interval.
3. Now we have two conditions : (actually 3 )
   a). Intervals do not overlap
   b). Intervals do overlap and new interval is completely inside the older one ( imagine the line is completely inside the previous line )
   c). Intervals do overlap, but only till the halfway, this means the new boundary of the previous interval will be update with the boundary of new interval.

Time complexity : O(n) - Cause we are only traversing each interval once.


Problem 3 : Merge sorted arrays 

My Approach :
1. We use 3 pointers.
2. we start from the last element of each sorted array.
3. We keep on decreasing our pointers accordingly.
4. Untill only one of the array is exahsusted.
5. If the nums2 array is exhausted, we do nothing because all our elements of nums1 are exactly where they should be.
6. If nums1 array is exhausted, we ned to fill the elements of nums2 at the remaining spaces in nums1.

Time complexity : O(N+m) 
