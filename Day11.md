Problem 1: Intersection of two linked list

Approach :
1. Okay, so what we do is, we make both node traverse each other.
2. So node1 will travel list1 completely, and when it reaches the end, it starts to travel list2.
3. Similarly, node2 will travel list2 completely and when it reaches the end, it starts to travel list1.
4. NOw, both of the nodes have travelled each other and they will meet at the intersection point.

Time Complexity : O(m+n)



Problem 2 : Detect a cycle in a Linked List.

Approach :
1. The problem is actually very simple.
2. We will use simple hare and tortoise method to solve it.
3. Slow pointer moves by one node and fast pointer moves by two nodes.
4. If there is a cycle in the list, then these pointers will eventually meet.

Time Complexity : O(N)

Problem 3 : 25. Reverse Nodes in k-Group

Approach :
1. First we count total number of nodes in the list.
2. Now we find the total groups that can be formed.
3. We keep track of current node and previous node.
4. Initially curr = head, prev = null
5. For each group, we keep the first node ( the node before the first group ), last node ( first node of the current group, which will eventually become the last node after reversing)
6. After reversing If it's the first group, update head to the new head (prev).
7. Otherwise, connect the previous group's tail (first) to the new head (prev).
8. Connect the tail of the reversed group (last) to the remaining list (curr).
9. Move prev to last so it can connect with the next reversed group.
10. Repeat until all complete groups are processed.
11. Return head.

Time Complexity : O(n)
