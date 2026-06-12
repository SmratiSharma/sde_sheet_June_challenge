Problem 1 : List is palindrome or not.

Approach :
1. We smartly solve this problem.
2. Since in palindrome, we check if one half is equal to other half or not, but here we cannot traverse backward.
3. So, we reverse half of the linkedlist.
4. First we find the middle of the list using hare and tortoise method.
5. Now we reverse the list from middle.
6. Now we check the valus of each node from start and from last.
7. If each node matches then, the list is palindrom otherwise not.

Time complexity : O(n)


Problem 2 : 142. Linked List Cycle II

Approach :
1. First we detect if there is a cycle or not. For this we take two pointer slow and fast, and if they meet evntually, there is a cycle or else not.
2. Now when they meet, we take another node and start from head;
3. We move by one step , and the node at which both nodes meet, is the start of the cycle.

Time Complexity: O(n)

Problem 3: 

Appraoch : 
1. Check the base case: If the list is empty or there is only one next list, return it.
2. Recursively flatten the right side (root.next).
3. Now you have two sorted lists: The current list (root using bottom pointers). , The flattened right list (root.next).
4. Merge these two sorted lists just like merging two sorted linked lists: Compare the current nodes of both lists. ,Attach the smaller node to the answer.
5. Move that pointer forward. Repeat until one list is exhausted.
6. Attach the remaining nodes.
7. Return the head of the merged list.
8. As recursion unwinds, every column gets merged, producing one completely flattened sorted list.

Time complexity : O(n*m)
