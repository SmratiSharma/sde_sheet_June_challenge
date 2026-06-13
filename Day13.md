Problem 1 : Rotate a linked lIst by k 

Approach :
1.  First we make a cycle of linked list.
2.  To do so, we will connect the end of ll with it's head. We will simultaneoulsy calculate the length of the LL.
3.  Now we will find the actual k, that will be k % length.
4.  No we will reach the node, just before the new head.
5.  We will create a new node and assign it curr.next
6.  Now curr.next will be null ( breaking the cycle ).

Time Complexity : O(n)

Problem 2 : 138. Copy List with Random Pointer  
Approach:
1. Very tricky. Simple and easy to understand approach is to add new nodes just after the original nodes and keep copying random of original into the random of copied nodes.
2. Step 1 : Add a new copy of current node just after it.
3. Step 2 : Assign random of copied node to the random of original node's next.
4. Step 3 : seperate both linkedl lists.

Time complexity : ;O(n)

Problem 3 : 3Sum

Approach :
1. Okay, so we have to find triplet pair of elements which have sum = 0.
2. First we will sort this array.
3. So second we will keep iterating from 0 to n-1.
4. For each element, we will find two other eleemnts in the list using two pointers.
5. If the sum of these elements equal to zero, we add them to the list, or else we increase left and right accordingly.
6. We will also skip the duplicate elements.

Time compelxity : O(n^2)
