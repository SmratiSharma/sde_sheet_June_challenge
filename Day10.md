Problem 1 : Delete nth node from the end of a linked list

Approach :
1. We declare two pointer fast and slow. 
2. First we find the nth node from the start of the list using fast pointer.
3. Now we check if the fast pointer has reached the end of the list ( which means that the n is the number of nodes, so we have to remove the first node, so we return the head.next )
4. Now we move both fast and slow pointer one by one until fast reaches the end.
5. Now our slow pointer points to the node just before the node we want to delete
6. Now we update the slow pointer using slow.next = slow.next.next
7. And we return the head.

Time Complexity : O (n)

Problem 2 : Add two numbers as a linked list

Approach : 
1. We declare a head node and a tail node which will point to head.
2. We store carry in a variable initialized as 0.
3. Now we iterate both the lists until they are empty or the carry is empty.
4. Now we keep on adding values of list1 and list 2 in a sum variable.
5. Now we update the tail .next value which will be sum % 10
6. and the carry is updated as sum / 10

Time complexity : O (Max(n,m))

Problem 3 : Delete node in a linked list.

Algorithm :
1. Create a temp node and point it to the given node.
2. Iterate until the we reach the second lasts node
3. With each iteration keep copying the value of next node in the current node.
4. When the loop end, copy the next value in the current node and set the temp.next = null

Time complexity : O(n)

