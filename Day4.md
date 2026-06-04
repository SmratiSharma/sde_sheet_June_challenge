Problem 1  : 287. Find the Duplicate Number

Brute force is O(n^2)
Optimal approach is Hare and Tortoise method.

Approach : 
1. Treat the array like a linked list,, index = node, value = next node.
2. Since numbers are from 1 to n , every value points to a valid index. But we have duplicate elements, so two or more elements will point to the same number.
3. This means there will be cycle formed, now if we move our pointers slow and fast, slow by one and fast by two, we will eventually meet slow and fast inside this cycle.
4. Now we will reset the slow pointer to start.
5. Now we move each one by one and they meet at the ccycle start  ( the duplicate element).

Time Complexity : O(n)

Problem 2  : Missing and Repeating

This one is tricky too.
Approach :
1. There should be ideally n intergers in the array. For each element , its index should be ideally element - 1.
2. So as we visite each element in the array ,we will mark its element-1 's value as negative, that way we will keep track of the element which have already occured in the array.
3. Once we find an element which is already negative, we have found the duplicate element.
4. Now for missing element, if for any index, the value is still postive then, the element will be index + 1.

5. Time complexity :  O(n)

Problem 3  : Count Inversion

Approach :
1. We use merge Sort.
2. Divide array into two, count inversion in left half and right half.
3. While merging, if the left element <= right element, merge noramlly
4. otherwise add all the remaining elements in the left half to inversion count.
5. merge normally then.

Time Complexity : O(nlog n )

