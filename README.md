# My Interview Preparation Studies
* Please note that the majority of the questions contained in this document are directly from Cracking the Coding Interview by Gayle Laakmann McDowell. This document is intended for my personal use and study of Gayle's book. The book is amazing - I highly suggest you [purchase a copy](http://www.crackingthecodinginterview.com/).

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
FOLLOW UP - How would you solve this problem if a temporary buffer is not allowed?

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
 &nbsp; 2    
  &nbsp;/ &nbsp; \    
1   &nbsp;&nbsp; 3    
 
Output:
[2,1,3], [2,3,1]

### 4.10 - Check Subtree
T1 and T2 are two very large binary trees, with T1 much bigger than T2. Create an algorithm to determine if T2 is a subtree of T1. A tree T2 is a subtree of T1 if there exists a node n in T1 such that the subtree of n is identical to T2. That is, if you cut off the tree at node n, the two trees wuold be identical.


### 4.11 - Random Node
You are implementing a binary tree class from scratch which, in addition to insert, find and delete, has a method getRandomeNode() which returns a randome node from the tree. All nodes should be equally likely to be chosen. Design and implement an algorithm to getRandomNode, and explain how you would implement the rest of the methods.


### 4.12 - Paths with Sum
You are given a binary tree in which each node contains an integer value (which might be positive or negative). Design an algorithm to count the number of paths that sum to a given value. The path does not need to start or end at the root or a leaf, but it must go downwards (traveling only from parent nodes to child nodes).


*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 5) Bit Manipulation

Bitwise operators treat their operands as a sequence of 32 bits (zeroes and ones), rather than as decimal, hexadecimal, or octal numbers. For example, the decimal number nine has a binary representation of 1001. Bitwise operators perform their operations on such binary representations, but they return standard JavaScript numerical values.    

The following table summarizes JavaScript's bitwise operators:    

| Operator | Usage | Description |
|------------------------------|---------|----------------------------------------------------------------------------------------------------------------------------------|
| Bitwise AND | a & b | Returns a one in each bit position for which the corresponding bits of both operands are ones. |
| Bitwise OR | a &#124; b | Returns a one in each bit position for which the corresponding bits of either or both operands are ones. |
| Bitwise XOR | a ^ b | Returns a one in each bit position for which the corresponding bits of either but not both operands are ones. |
| Bitwise NOT | ~ a | Inverts the bits of its operand. |
| Left Shift | a << b | Shifts a in binary representation b (< 32) bits to the left, shifting in zeroes from the right. |
| Sign-propogating right shift | a >> b | Shifts a in binary representation b (< 32) bits to the right, discarding bits shifted off. |
| Zero-fill right shift | a >>> b | Shifts a in binary representation b (< 32) bits to the right, discarding bits shifted off, and shifting in zeroes from the left. |

### 5.1 - Insertion
You are given two 32-bit numbers, N and M, and two bit positions, i and j. Write a method to insert M into N such that M starts at bit j and ends at bit i. You can assume that the bits j through i have enough space to fit all of M. That is, if M=10011, you can assume that there are atleast 5 bits between j and i. You would not, for example, have j=3 and i=2, because M could not fully fit between bit 3 and bit 2.

### 5.2 - Binary to string
Given a real number between 0 and 1 (e.g., 0.72) that is passed in as a double, print the binary representation. If the number cannot be represented accurately in binary with at most 32 characters, print "ERROR"

### 5.3 - Flip Bit to Win
You have an integer and you can flip exactly one bit from a 0 to a 1. Write code to find the length of the longest sequence of 1s you could create.

EXAMPLE:    

Input: 1175 (or: 11011101111)    
Output: 8    

### 5.4 - Next Number
Given a positive integer, print the next smallest and the next largest number that have the same number of 1 bits in their binary representation.

### 5.5 - Debugger
Explain what the following code does: ((n & (n-1)) == 0)

### 5.6 - Conversion
Write a function to determine the number of bits you would need to flip to convert integer A to integer B.

EXAMPLE:    
Input: 29 (or: 11101), 15 (or: 01111)    
Output: 2    

### 5.7 - Pairwise Swap
Write a program to swap odd and even bits in an integer with as few instructions as possible (e.g., bit 0 and bit 1 are swapped, bit 2 and bit 3 are swapped, and so on).

### 5.8 - Draw Line
A monochrome screen is stored as a single array of bytes, allowing eight consecutive pixels to be stored in one byte. The screen has width w, where w is divisible by 8 (that is, no byte will be split accress rows). The height of the screen, of course, can be rerived from the length of the array and the width. Implement a function that draws a horizontal line from (x1, y) to (x2, y). The method signature should look something like this:    
drawLine(byte[] screen, int width, int x1, int x2, int y)

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 6) Math and Logic Puzzles


### 6.1 - The Heavy Pill
You have 20 bottles of pills, 19 bottles have 1.0 gram pills, but one has pills of weight 1.1 grams. Given a scale that provides an exact measurement, how would you find the heavy bottle? You can only use the scale once.

### 6.2 - Basketball
You have a basketball hoop and someone says that you can play one of two games.       
Game 1: You get one shot to make the hoop.    
Game 2: You get three shots and you have to make two of three shots.    
If p is the probability of making a particular shot, for which values of p should you pick one game or the other?

### 6.3 - Dominos
There is an 8x8 chessboard in which two diagonally opposite corners have been cut off. You are given 31 dominos, and a single domino can cover exactly two squares. Can you use the 31 dominos to cover the entire board? Prove your answer (by providing an example or showing why it's impossible)

### 6.4 - Ants on a Triangle
There are three ants on different vertices of a triangle. What is the probability of collision (between any two or all of them) if they start walking on the sides of the triangle? Assume that each ant randomly picks a direction, with either direction being equally likely to be chosen, and that they walk at the same speed.    
Similarly, find the probability of collision with n ants on an n-vertex polygon.

### 6.5 - Jugs of Water
You have a five-quart jug, a three-quart jug, and an unlimited supply of water (but no measuring cups). How would you come up with exactly four quarts of water? Note that the jugs are oddly shaped, such that filling up exactly "half" of the jug would be impossible.

### 6.6 - Blue-Eyed Island
A bunch of people are living on an island, when a visitor comes with a strange order: all blue-eyed people must leave the island as soon as possible. There will be a flight out at 8:00pm every evening. Each person can see everyone else's eye color, but they don't know their own (nor is anyone allowed to tell them). Additionally, they do not know how many people have blue eyes, although they do know that at least one person does. How many days will it take the blue-eyed people to leave?

### 6.7 - The Apocalypse
In the new post-apocalyptic world, the world queen is desperately concerned about the birth rate. Therefore, she decrees that all families should ensure that they have one girl or else they face massive fines. If all families abide by this policy - that is they have continue to have children until they have one girl, at which point they immediately stop - what will the gender ratio of the new generation be? (Assume that the odds of someone having a boy or a girl on any given pregnancy is equal.) Solve this out logically and then write a computer simulation of it.

### 6.8 - The Egg Drop Problem
There is a building of 100 floors. If an egg drops from the Nth floor or above, it will break. If it's dropped from any floor below, it will not break. You're given two eggs, Find N, while minimizing the number of drops for the worst case.

### 6.9 - 100 Lockers
There are 100 closed lockers in a hallway. A man begins by opening all 100 lockers. Next, he closes every second locker. Then, on his third pass, he toggles every third locker (closes it if it is open or opens if it is closed). This process continues for 100 passes, such that on each pass i, the man toggles every ith locker. After his 100th pass in the hallway, in which he toggles only locker #100, how many lockers are open?

### 6.10 - Poison
You have 100 bottles of soda, and exactly one is poisoned. You have 10 test strips which can be used to detect poison. A single drop of poison will turn the test trip positive permanently. You can put any number of drops on a test strip at once and you can resuse a test strip as many times as you'd like (as long as the results are negative). However, you can only run tests once per day and it takes seven days to return a result. How would you figure out the posoned bottle in as few days as possible?    
FOLLOW UP:    
Write code to simulate your approach.

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 7) Object-Oriented Design

### 7.1 - Deck of Cards
Design the data structures for a generic deck of cards. Explain how you would subclass the data structures to implement black jack.

### 7.2 - Call Center
Imagine you have a call center with three levels of employees: respondent, manager and director. An incoming telephone call must be first allocated to a respondent who is free. If the respondent can't hand;e the call, he or she must excalate the call to a manager. If the manager is not free or not able to handle it, then the call should be escalated to a director. Design the classes and data structure for this problem. Implement a method dispatchCall() which assigns a call to the first available employee.

### 7.3 - Jukebox
Design a musical jukebox using object-oriented principles.

### 7.4 - Parking Lot
Design a parking lot using object-oriented principles.

### 7.5 - Online Book Reader
Design the data structures for an online book reader system.

### 7.6 - Jigsaw
Implement an NxN jigsaw puzzle. Design the data structures and explain an algorithm to solve the puzzle. You can assume that you have a fitsWith method which, when passed two puzzle edges, returns true if the two edges belong together.

### 7.7 - Chat Server
Explain how you would design a chat server. In particular, provide details about the various backend components, casses and methods. What would be the hardest problems to solve?

### 7.8 - Othello
Othello is played as follows: Each Othello piece is white on one side and black on the other. When a piece is surrounded by its opponents on both the left and right sides, or both the top and bottom, it is said to be captured and its color is flipped. On your turn, you must capture at least one of your opponent's pieces. The game ends when either user has no more valid moves. The win is assigned to the person with the most pieces. Implement the object-oriented design for Othello.

### 7.9 - Circular Array
Impleent a CircularArray class that supports an array-like data structure which can be efficiently rotated. If possible, the class should use a generic type (also called a template), and should support iteration via the standard for(Obj o : circularArray) notation.

### 7.10 - Minesweeper
Design and implement a text-based Minesweeper game. Minesweeper is the classic single-player gcomputer game where an NxN grid has B mines (or bombs) hidden across the grid. The remaining cells are either blank or have a number behind them. The numbers reflect the number of bombs in the surrounding eight cells. The user then uncovers a cell. If it is a bomb, the player loses. If it is a number, the number is exposed. If it is a blank cell, this cell and all adjacent blank cells (up to and including the surrounding numeric) are exposed. The player wins when all non-bomb cells are exposed. The player can also flag certain places as potential bombs. This doesn't affect game play, other than to block the user from accidentally clicking a cell that is thought to have a bomb. (Tip for the reader: if you're not familiar with this game, please play a few rounds online first

### 7.11 - File system
Explain the data structures and algorithms that you would use to design an in-memory file system. Illustrate with an example in code where possible.

### 7.12 - Hash Table
Design and implement a hash table which uses chaining (linked lists) to handle collisions.

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 8) Recursion and Dynamic Programming

### 8.1 - Triple Step
A child is running up a staircase and can either hop either 1, 2 or 3 steps at a time. Implement a method to count how many possible ways the child can run up the stairs.

### 8.2 - Robot in a Grid
Imagine a robot sitting on the upper left corner of grid with n rows and c columns. The robot can only move in two directions, right and down, but certain cells are "off limits" such that the robot cannot step on them. Design an algorithm to find a path for the robot from the top left to the bottom right.

### 8.3 - Madic Index
A magic index in an array A[0...n-1] is defined to be an index such that A[i] = i. Given a sorted array of distinct integers, write a method to find a magic index, if one exists, in array A.    
FOLLOW UP    
What if the values are not distinct?

### 8.4 - Power Set
Write a method to return all subsets of a set.

### 8.5 - Recursive Multiply
Write a recursive function to multiply two positive integers without using the * operator. You can use addition, subtraction, and bit shifting, but you should minimize the number of those operations.

### 8.6 - Towers of Hanoi
In the classic proble of the Towers of Hanoi, you have 3 towers and N disks of different sizes which can slide onto any tower. The puzzle starts with disks sorted in an ascending order of size from top to bottom (i.e., each disk sits on top of an even larder one). You have the following constraints:    
1) Only one disk can be moved at a time.    
2) A disk is slid off the top of one tower onto another.    
3) A disk cannot be placed on top of a smaller disk.    
Write a program to move the disks from the first tower to the last using stacks.

### 8.7 - Permutations without Dups
Write a method to compute all permutations of a string of unique characters.

### 8.8 - Permutations with Dups
Write a method to compute all permutations of a string whose charcters are not necessarily unique. The list of permutations should not have duplicates.

### 8.9 - Parens
Implement an algorithm to print all valid (e.g., properly opened and closed) combinations or n pairs of parentheses.     
EXAMPLE:    
Input: 3     
Output: ((())), (()()), (())(), ()(()), ()()()

### 8.10 - Paint Fill
Implement the "paint fill" function that one might see on many image editing programs. That is, given a screen (represented b a two-dimensional array of colors), a point, and a new color, fill in the surrounding area until the color changes from the original color.

### 8.11 - Coins
Given an infinite number of quarters (25 cents), dimes (10 cents), nickels (5 cents), and pennies (1 cent), write code to calculate the number of ways of representing n cents.

### 8.12 - Eight Queens
Write an algorithm to print all ways of arranging eight queens on an 8x8 chessboard so that none of them share the same row, column, or diagonal. In this case "diagonal" means all diagonals, not just the two that bisect the board.

### 8.13 - Stack of Boxes
You have a stack of n boxes, with widths w[i], heights h[i] and depths d[i]. The boxes cannot be rotated and can only be stacked on top of one another if each box in the stack is strictly larger than the box above it in width, height and depth. Implement a method to compute the height of the tallest possible stack. The height of a stack is the sum of the heights of each box.

### 8.14 - Boolean Evaluation
Given a boolean expression consisting of the symbols 0 (false), 1 (true), & (AND), | (OR), and ^ (XOR), and a desired boolean result value result, implement a function to count the number of ways of parenthesizing the expression such that it evaluates to result.     
EXAMPLE:     
countEval("1^0|0|1", false) -> 2     
countEval("0&0&0&1^1|0", true) -> 10

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 9) System Design and Scalability

### 9.1 - Stock Data
Imagine you are building some sort of service that will be called by up to 1,000 client applications to get simple end-of-day stock price information (open, close, high, low). You may assume that you already have the data, and you can store it in any format you wish. How would you design the client-facing service that provides the information to client applications? You are responsible for the development, rollout and ongoing monitoring and maintenance of the feed. Describe the different methods you considered and why you would recommend your approach. Your service can use any technologies you wish, and can distribute the information to the client application in any mechanism you choose.

### 9.2 - Social Network
How would you design the data structures for a very large social network like Facebook or Linkedin? DEscribe how you would design an algorithm to show the shortest path between two people (e.g., Me -> Bob -> Susan -> Jason -> You).

### 9.3 - Web Crawler
If you were designing a web crawler, how would you avoid getting into infinite loops?

### 9.4 - Duplicate URLs
You have 10 billion URLs. How do you detect the duplicate documents? In this case, assume "duplicate" means that the URLs are identical.

### 9.5 - Cache
Imagine a web server for a simplified search engine. This system has 100 machines to respond to search queries, which may then call out using processSearch(string query) to another cluster of machines to actually get the result. The machine which responds to a given query is chosen at random, so you cannot guarantee that the same machine will always respond to the same request. The method processSearch is very expensive. Design a caching mechanism for the most recent queries. Be sure to explain how you would update the cache when data changes.

### 9.6 - Sales Rank
A large eCommerce company wishes to list the best-selling products, overall and by categor. For example, one product might be the #1056th best-selling product overall, but the #13th best-selling product under "Sports Equipment" and the #24th best selling-product under "Safety". Describe how you would design this system.

### 9.7 - Personal Finance Manager
Explain how you would design a personal financial manager (like Mint.com). This system would connect to your bank accounts, analyze your spending habits, and make recommendations. 

### 9.8 - Pastebin
Design a system like Pastebin, where a user can enter a piece of text and get a randomly generated URL to access it.

*****************************************************************************************************************************************************************************************************************************************************************************************************************************************

## 10) Sorting and Searching

### 10.1 - Sorted Merge
You are given two sorted arrays, A and B, where A has a lerge enough buffer at the end to hold B. Write a method to merge B into A in sorted order.

### 10.2 - Group Anagrams
Write a method to sort an array of strings so that all the anagrams are next to each other.

### 10.3 - Search in Rotated Array
Given a sorted array of n intergers that has been rotated an unknown number of times, write code to find an element in the array. You may assume that the array was originally sorted in increasing order.     
EXAMPLE     
Input: find 5 in [15,16,19,20,25,1,3,4,5,7,10,14]     
Output: 8 (the index of 5 in the array)

### 10.4 - Sorted Search, No Size
You are given an array-like data structure Listy which lacks a size method. It does, however, hae an elementAt(i) method that returns the element at index i in O(1) time. If i is beyond the bounds of the data structure, it returns -1. (For this reason, the data structure only supports positive integers.) Given a Listy which contains sorted, positive integers, find the index at which an element x occurs. If x occurs multiple times, you may return any index.     

### 10.5 - Sparse Search
Given a sorted array of strings that is interspersed with empty strings, write a method to find the location of a given string.     
EXAMPLE     
Input: ball, ["at","","","","ball","","","car","","","dad","",""]     
Output: 4

### 10.6 - Sort Big File
Imagine you have a 20 GB file with one string per line. Explain how you would sort the file.

### 10.7 - Missing Int
Given an input file with four billion non-negative integers, provide an algorithm to generate an integer that is not contained in the file. Assume you have 1GB of memory available for this task.     
FOLLOW UP     
What if you only have 10MB of memory? Assume that all the values are distinct and we now have no more than one billion non-negative integers.

### 10.8 - Find Duplicates
You have an array with all the numbers from 1 to N, where N is at most 32,000. The array may have duplicate entries and you do not know what N is. With only 4 kilobytes of memory available, how would you print all duplicate elements in the array?

### 10.9 - Sorted Matric Search
Given an MxN matrix in which each row and each column is sorted in ascending order, write a method to find an element.

### 10.10 - Rank from Stream
Imagine you are reading from a stream of integers. Periodically, you wish to be able to look up the rank of a number x (the number of values less than or equal to x). Implement the data structures and algorithms to support these operations. That is, implement the method track( int x), which is called when each number is generated, and the method getRankOfNumber(int x), which returns the number of values less than or equal to x (not including x itself).     
EXAMPLE     
Stream(in order of appearance): 5,1,4,4,5,9,7,13,3     
getRankOfNumber(1) = 0     
getRankOfNumber(3) = 1     
getRankOfNumber(4) = 3     

### 10.11 - Peaks and Valleys
In an array of integers, a "peak" is an element which is greater than or equal to the adjacent integers and a "valley" is an element which is less than or equal to the adjacent integers. For example, in the array [5,8,6,2,3,4,6], [8,6] are peaks and [5,2] are valleys. Given an array of integers, sort the array into an alternating sequence of peaks and valleys.     
EXAMPLE     
Input: [5,3,1,2,3]     
Output: [5,1,3,2,3]

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
