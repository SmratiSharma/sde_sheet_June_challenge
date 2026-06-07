Problem 1 : 2Sum : Literally 1st problem of Leetcode

Approach :
1. Brute force approach will take O(n^2).
2. So we keep a map, and store elements in it, with their index, but before that, we check if the compliment element is already present in the map, if yes, then we add it into our ans.

Time complexity : O(n)


Problem 2 : 4Sum

Approach :
1. Now normal approach might take O(n^4).
2. WE will try to reduce it to O(n^3).
3. We will first sort the array.
4. We will start from 1st element, then reach 2nd element using iterator.
5. Now for 3rd and 4th element we will use 2 pointers approach.
6. To remove duplicate, we will keep on checking the previous element, and skip it.
7. now the key point is, the sum of 1st two elements should equal to target - ( sum of last two elements )
8. If that's true, we have found one array of elements summed to target.
9. We keep on updating the left and right based on the sum value.

Time Complexity : O(n^3)


Problem 3 : Longest Consecutive Subsequence

Approach :
1. We insert all the elements into HashSet.
2. WE start traversing the array.
3. We assume each element is the start of the subsequence, if the element - 1 is not present in the set.
4. WE keep checking num+1, num+2... and count the length;
5. WE update the maximum length.

Time Complexity : O(n)
