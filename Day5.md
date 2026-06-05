Problem 1 : Seach a 2D matrix

Approach :
1. To make search simple, we will assume the 2D matrix into 1D,
2. To do so, we need to assume that total size of the 1D array is m*n.
3. Now say a random index i, in 1D array will be equal to i/n th row and i%n the column.
4. So no we will apply our binary seach, since the elements are already in sorted order, we will find mid and we keep on updating mid until we find target or reach the end.

Time Complexity : O( (m+n) log (m + n))


Problem 2 : Pow(x,n)

Approach:
1. In traditional (brute force ) method, we have to multiply x by x , n times, which is slow.
2. So we use the fact that : 2*2*2*2 = (2^2)^2 , and if odd power, then x* (x^2)^(n-1)/2.
3. So we first check if the n is negative and change x accoringly, then we keep on updating answer untill power becomes 0.

Time complexity : O(log n)

Problem 3 : Majority element

Approach :
1. Simple af.
2. We sort the array,
3. So the mojoirty element is more than n/2 times, so it has to appear at the index n/2, so we return it

Time complexity : O(nlogn) : sorting
