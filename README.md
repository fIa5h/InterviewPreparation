# My Interview Preparation Studies

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 1) STRINGS AND ARRAYS

### 1.1 - Is Unique
Implement an algorithm to determine if a string has all unique characters. What if you cannot use additional data structures?

### 1.2 - Check Permutation
Given two strings, write a method to decide if one is a permutation of the other.

### 1.3 - URLify
Write a method to replace all spaces in a string with ‘%20’. You may assume that the string has sufficient space at the end to hold the additional characters, and that you are given the “true” length of the string. (Note: implementing in Java, please use a character array so that you can perform this operation in place.) 

### 1.4 - Palindrome Permutation
Given a string, write a function to thick if it is a permutation of a palindrome. A palindrome is a word of phrase that is the same forwards and backwards. A permutation is a rearrangement of letters. The palindrome does not need to be limited to just dictionary words.

### 1.5 - One Away
There are three types of edits that can be performed on strings: insert a character, remove a character or replace a character. Given to strings, write a function to check if they are one edit or zero edits away.

### 1.6 - String Compression
Implement a method to perform basic string compression using the counts of repeated characters. For example, the string aabbccccaaa would become a2b1c5a3. If the compressed string would not become smaller than the original string, your method should return the original string. You can assume the string has only uppercase and lowercase letters (a-z)

### 1.7 - Rotate Matrix
Given an image represented by an NxN matrix, where each pixel in the image is 4 bytes, write a method to rotate the image by 90 degrees. Can you do this in place?

### 1.8 - Zero Matrix
Write an algorithm such that if an element in an MxN matrix is 0, its entire row and column are set to 0.

### 1.9 - String Rotation
Assume you have a method isSubstring which checks if one word is a substring of another. Given two strings, s1 and s2, write code to check if s2 is a rotation of s1 using only one call to isSubstring. (e.g. “waterbottle” is a rotation of “erbottlewat”)

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 2) LINKED LISTS

### 2.1 - Remove Dups
Write code to remove duplicates from an unsorted linked list.
Follow up - How would you solve this problem if a temporary buffer is not allowed?

### 2.2 - Return Kth to the last
Implement an algorithm to find the Kth to the last element of a singly linked list.

### 2.3 - Delete middle node
Implement and algorithm to delete a node in the middle (i.e., any node but the first and last node, not necessarily the exact middle) of a singly linked list, given only access to the node.

EXAMPLE:
Input: the node c from the linked list a->b->c->d->e->f
Result: nothing is returned but the new linked list looks like a->b->d->e->f

### 2.4 - Partition
Write code to partition a linked list around a value X, such that all nodes less than X come before all nodes greater than or equal to X. If X is contained within the list, the values of X only need to be after the elements less than X (see below). The partition element X can appear anywhere in the “right partition”; it doesn’t need to appear between the left and right partitions.

EXAMPLE:
Input: 3 -> 5 -> 8 -> 5 -> 10 -> 2 -> 1 [partition = 5]
Output: 3 -> 1 -> 2 -> 10 -> 5 -> 5 -> -> 8

### 2.5 - Sum lists
You have two numbers represented by a linked list, where each node contains a single digit. The digits are stored in reverse order, such that the 1’s digit is at the head of the list. Write a function that adds the two numbers and returns the sum as a linked list.

EXAMPLE:
Input: (7 -> 1 -> 6) + (5 -> 9 -> 2). That is, 617 +295.
Output: 2 -> 1 -> 9. That is, 912.

FOLLOW UP
Suppose the digits are stored in a forward order. Repeat the above problem.
Input: (6 -> 1 -> 7) + (2 -> 9 -> 5). That is, 617 +295.
Output: 9 -> 1 -> 2. That is, 912.

### 2.6 - Palindrome
Implement a function to check if a linked list is a palindrome.

### 2.7 - Intersection
Given two singly linked lists, determine if the two lists intersect. Return the intersecting node. Note that the intersection is defined based on reference, not value. That is, if the nth node of the first linked list is the exact same node (by reference) as the nth node of the second linked list, then they are intersecting.

### 2.8 - Loop Detection
Given a circular linked list, implement an algorithm that returns the node at the beginning of the loop. 

DEFINITION
Circular linked list: A (corrupt) linked list in which a node’s next pointer points to an earlier node, so as to make a loop in the linked list

EXAMPLE
Input: a -> b -> c -> d -> e -> c (the same c as earlier)
Output: c

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 3) Stacks and Queues

### 3.1 - Three in One
Describe how you could use a single array to implement three stacks.

### 3.2 - Stack Min
How would you design a stack which, in addition to push and pop, has a function which returns the minimum element? Push, pop and min should all operate in O(1) time.

### 3.3 - Stack of Plates
Imagine a literal stack of plates. If the stack gets too high, it might topple. Therefore, in real life, we would likely start a new stack when the previous stack exceeds som threshold. Implement a data structure SetOfStacks that mimics this. SetOfStacks should be composed of several stacks and should create a new stack once the previous one exceeds capacity. SetOfStacks.push() and SetOfStacks.pop() should behave indentically to a sinfle stack (that is, pop() should return the same calues as it would if there were just a single stack).

FOLLOW UP:
Implement a function popAt(int index) which performs a pop operation on a specific sub-stack.

### 3.4 - Queue via Stacks
Implement a MyQueue class which implements a queue using two stacks.

### 3.5 - Sort Stack
Write a program to sort a stack such that the smallest items are on the top. You can use an additional temporary stack, but you may not copy the elements into any other data structure (such as an array). The stack suports the following operations: push, pop, peek, and isEmpty.

### 3.6 - Animal Shelter
An animal shelter, which holds only dogs and cats, operates on a strictly "first in, first out" basis. People must adopt either the "oldest" (based on arrival time) of all the animals at the shelter, or they can select whether they would prefer a dog or a cat (and will receive the oldest animal of that type). They cannost select which specific animal they would like. Create the data astructures to maintain this system and implement operations such as enqueue, dewueueAny, dequeueDog, and dequeueCat. You may use the built-in LinkedLust data structure. 

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 4) Trees and Graphs

### 4.1 - Route between nodes
Given a directed graph, design an algorithm to find out whether there is a route between two nodes.

### 4.2 - Minimal Tree
Given a sorted (increasing order) array with unique integer elements, write an algorithm to create a binary search tree with minimal height.

### 4.3 - List of Depths
Given a binary tree, design an algorithm which creates a linked list of all the nodes at each depth (e.g., if you have a tree with depth D, you'll have D linked lists)

### 4.4 - Check Balanced
Implement a function to check if a binary tree is balanced. For the purposes of this question, a balanced tree is defined to ba a stree such that the heights of the two subtrees of any node never differ by more than one. 


### 4.5 - Validate BST
Implement a function to check if a binary tree is a binary search tree.


### 4.6 - Successor
Write an algorithm to find the "next" node (i.e., in-order successor) of a given node in a binary search tree. You may assume that each node has a link to its parents. 


### 4.7 - Build order
You are given a list of projects and a list of dependencies (which is a list of pairs of projects, where the second project is dependent on the first project). All of a project's dependeies must be built before the project is. Find a build order that will allow the projects to be built. If there is no valid build order, return an error.

EXAMPLE:

Input:
projects: a, b, c, d, e, f
dependencies: (a,d), (f,b), (b,d), (f,a), (d,c)

Output: 
f, e, a, b, d, c


### 4.8 - First Common Ancestor
Design an algorithm and write code to find the first common ancestor of two nodes in a binary tree. Avoid storing additionall nodes in a data structure. NOTE: This is not necessarily a binary search tree.


### 4.9 - BST sequences
A binary search tree was created bu traversing through an array from left to right and inserting each element. Given a binary search tree with distinct elements, print all possible arrays that coule have led to this tree.

EXAMPLE:
   2
  / \
 1   3
 
Output:
[2,1,3], [2.3.1]

### 4.10 - 


### 4.11 - 


### 4.12 - 


*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 5) Bit Manipulation

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 6) Math and Logic Puzzles

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 7) Object-Oriented Design

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 8) Recursion and Dynamic Programming

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 9) System Design and Scalability

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 10) Sorting and Searching

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 11) Testing

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 12) C and C++

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 13) Java

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 14) Databases

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 15) Threads and Locks

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 16) Moderate

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 17) Hard

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************
