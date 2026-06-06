Problem 1 : Majority Element II

Approach :
1. Okay, the simplest approach will be store each element's occurance in a map, then find out whoes occurance is more than n /3.
2. But a even more optimal approach will be to use Boyer-Moore Voting Algorithm.
3. Now understand that, only atmostt 2 elements can be majority element.
4. So, we keep 2 candidates (candidate1 and candidate2) and 2 counters (count1 and count2).
5. If the current number is equal to candidate1, increase count1.
    Else if it is equal to candidate2, increase count2.
    Else if count1 is 0, make the current number candidate1.
    Else if count2 is 0, make the current number candidate2.
    Otherwise, decrease both count1 and count2.
7. After the first traversal, we get two possible majority elements.
8. Traverse the array again and count how many times these two candidates actually appear.
9. If any candidate appears more than n/3 times, add it to the answer and return the list.

Time Complexity: O(n)


Problem 2  :Unique path

Approach :
1. This is a classic DP problem.
2. we can use memoization, then we can use tabulation, then we can optimize even tabulation solution.
3. Keep in mind that, we can only move to left or bottom, and each block will add up to 1 step.
4. We fill our dp array ( 1D ) with 1, since each step will cost us 1 step.
5. Now , if we observe, we only need one block to find out how many step we need to reach the current block, that it the previous block in current row.
6. So we find result using dp [ col ] += dp [ col-1 ]

Time complexity : O(m+n) 
