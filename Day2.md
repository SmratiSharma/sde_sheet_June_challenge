Problem 1 : 53. Maximum Subarray

Kadane's Algorithm.

My approach :
1. We need to find the maximum sum of any subarray. We do not need the subarray only track the sum of subarray
2. We will keep on checking value of sum on every element.
3. If the current sum is greater than the maxSum value ( which we will initialize as minimum value possible ), then we will update the maxSum value, otherwise not.
4. If at any point, the value of local sum becomes negative, we will reset it to zero, becuase negative value will never give maximum result.

Time complexity : O(n) , because we are traversing the array only once.

Problem 2 : 

75. Sort Colors

My Approach : 
1. Keep three pointers, One will be left, which will point to the last zero, 2nd will be middle, which will point the last 1, 3rd will be right which will point to the last 2 in the beginning.
2. We will check the element at middle, if the elment at middle is 0, then we will swap these element and increase the value of low and middle by one.
3. If the element is 1, we will simply increase the value of middle counter by one.
4. Else the element in the middle is 2, then we will swap the elements at middle and right and decrease the value of right by one.
5. In the end we will get an array with all the zeros in the beginning , all the ones in middle and all the 2's in end.

This is also called dutch national flag problem.

Time complexity : O(n) , because we are traversing array only once.


Problem 3 : 

121. Best Time to Buy and Sell Stock

My Approach : 
1. It is a simple problem of checking maximum profit at each step.
2. First we will assume the minimum stock values as prices[0].
3. Now we will traverse, and keep on updating min value if prices[i] < min.
4. At each step we will check for maxProfit.
5. In the end we return maxProfit.

Time Complexity: O(n) 
