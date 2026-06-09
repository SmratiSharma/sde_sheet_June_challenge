Problem 1 : Reverse a LInked List.
Oldest problem in the book
Oldest solution in the book.

Approach:
1. Make a current pointer and point it to the head.
2. This current pointer will always point the current node as we move forward untill linked list ends.
3. Now we need a previous pointer which will always point to the the previous node of the current node ( because we want to reverse the linkedlist, we need the pointer to the previous node.
4. Now we will iterate through the linked list until the list is empty.
5. Inside the loop, we keep a temperory node which will be used to update current and previous pointer.

Time complexity : O(n)


Problem 2 : Find middle of the linked list

Approach 
1.  We use simple horse and tortoise method here.
2.  We initialize two pointers, fast and slow to the head.
3.  We move fast by two nodes, and slow by one node.
4.  We keep on moving until the fast becomes null or fast.next becomes null
5.  We return the slow pointer.

Time Complexity : O(n)


Problem 3 : Merge two sorted Lists

Approach :
1. First we create a dummy node, which will point to the merged node.
2. Now the merged node will get updated depending on the value of list1 and list2.
3. We keep track of dummy node and update it accordingly.
4. In the end, we merge the list which has not ended yet.

Time complexity : O(n+m)
