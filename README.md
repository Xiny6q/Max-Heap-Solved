Download link :https://programming.engineering/product/max-heap-solved/

# Max-Heap-Solved
Max Heap Solved
A MaxHeap is a type of binary tree with two main properties.

Shape Property: The tree must be complete. All levels of the tree must be full except the bottom-most level. If the bottom-most level is not full, it must be filled from left to right without any ’gaps’ between nodes.

Order Property: Each node’s data is larger than the data in its two children. There is no explicit relationship between sibling nodes.

These properties guarantee that the largest element in the heap will be at the root of the heap.

Although heaps are usually classified as a type of tree, they are commonly implemented using an array due to their completeness. In your implementation, you should leave index 0 empty and begin your heap at index 1. This will make the arithmetic to find parents and children simpler.

To find the children of index i, 2i is the index of the left child (if one exists) and 2i + 1 is the in-dex of the right child (if one exists). Conversely, the parent of index i is index i/2 (integer division). Recall that Java automatically performs integer division when dividing two ints.

You should implement two constructors for this heap. One constructor initializes an empty heap with the capacity specified by a constant in MaxHeap.java. The other constructor should implement the BuildHeap algorithm that was taught in lecture, which is an algorithm that creates a heap in O(n) time. Simply adding the elements one by one will not receive credit since it would be O(n log(n)) in the worst case; see the javadocs for this constructor for more specifications.

You may assume that your implementation does not need to handle duplicate elements. That is, the add method will never be passed duplicates and the remove method will never have to deal with the heap having duplicates. To be clear, your implementation would most likely work even if we were to test for duplicates; however, this will help remove ambiguity surrounding grading and testing your implementation.

Unlike your BST homework, you are not required to use recursion in this assignment. Use whatever you find most intuitive – recursion, iteration, or both. However, regardless of the technique you use, make sure to meet efficiency requirements as discussed in lecture.

Homework 5: MaxHeap Due: See Canvas

Grading

Here is the grading breakdown for the assignment. There are various deductions not listed that are incurred when breaking the rules listed in this PDF and in other various circumstances.

Methods:

constructor / buildHeap

20pts

add

20pts

remove

20pts

getMax

5pts

isEmpty

5pts

clear

5pts

Other:

Checkstyle

10pts

Efficiency

15pts

Total:

100pts

Provided

The following file(s) have been provided to you. There are several, but we’ve noted the ones to edit.

MaxHeap.java

This is the class in which you will implement the MaxHeap. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance variables, or static variables.

MaxHeapStudentTest.java

This is the test class that contains a set of tests covering the basic operations on the MaxHeap class. It is not intended to be exhaustive and does not guarantee any type of grade. Write your own tests to ensure you cover all edge cases.

Deliverables

You must submit all of the following file(s) to the course Gradescope. Make sure all file(s) listed below are in each submission, as only the last submission will be graded. Make sure the filename(s) matches the filename(s) below, and thatonly the following file(s) are present. If you resubmit, be sure only one copy of each file is present in the submission. If there are multiple files, do not zip up the files before submitting; submit them all as separate files.

Once submitted, double check that it has uploaded properly on Gradescope. To do this, download your uploaded file(s) to a new folder, copy over the support file(s), recompile, and run. It is your sole responsibility to re-test your submission and discover editing oddities, upload issues, etc.

MaxHeap.java
