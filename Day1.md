Problem 1 : 

73. Set Matrix Zeroes

My approach : Optimal Approach :
1. First we will check wether our first row and our first column need to be set to all 0's.
2. If yes, we will store that in two boolean variables.
3. Now we will use this row and column as our array and we will check for further rows and columns.
4. If we find any 0, we will mark for that particular row and column as 0 int our first row and column.
5. Then we will traverse again for rows and columns starting from 1, and if matrix[i][0] == 0 ( means matrix has a 0 in ith row) or matrix[0][j] == 0 ( means, matrix has a 0 in jth coloumn ) , then we will make that cell as 0.
6. Now we will check for our boolean flags and change the first row and column respectively.

Time Complexity : O(m*n)

My Learnings : Think smartly, try to optimize the solution as much as you can. 
In - place problems are trickier so keep your mind open. 



Problem 2 : 

118. Pascal's Triangle

My Appraoch :

1. Simple intution is that for each index of a particular list ( or row ) either it is first element, or last element for in-between element.
2. For first and last element, we need to store 1.
3. For in-between elements, we need to sum the previous row's current index's value and current index - 1's value.

Time Complexity :  O(n^2)  

My Learning : It is a simple problem, do not take too much time. 



Problem 3 : 

31. Next Permutation

My Approach :

1. It is not very easy problem.
2. Analyse the pattern of the permutations.
3. We first need to find the index of the element where the array is pivoted.
4. Next we find the element just greater than that element.
5. We swap pivot element with the current element.
6. Now we reverse the array from current elment till the last element.
7. We have found the next permutation.

Time Complexity : O(n) ( we performed linear scans of the array ) 













