Problem 1 : Largest Subarray with K sum

Approach : 
1. Now, the brute force approach will give O(n^2) time complexity, we don't want that chat.
2. WE will use Prefix sum + hashmap to solve this problem.
3. We start loop, and keep track of sum of elements till i,
4. If this sum is K, we have found one subarray with sum k, we will update maxLen to the i + 1 ( since We are moving from 0 to n )
5. Now, we check if our map already contains sum - k, this means if sum - k has already existed in the map, then k would also exist.
6. So we checkout the length of that subarray and find out if that is maxlen or not.
7. In the end we put our new sum in the map with the ith position.

Time complexity : O(n)


Problem 2 : Count subarrays with given xor K

Appraoch :
1. Similar to previous solution,
2. Here instead of sum, we keep track of xor till current element, and the count the subarrays with xor k.
3. We update the map

Time Complexity : O(n)

Problem 3 : Longest Substring Without Repeating Characters

1. We use two pointers approach for this problem.
2. WE keep a set to store unique elements of the string.
3. We iterate through the string, and check if the current already exist in the set,
4. We move left pointer untill the set contains unique element
5. WE update the longest substring.
6. Now we add character at right into the set.

Time complexity : O(n)
