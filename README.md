Download Link : https://programming.engineering/product/stacks-and-queues-2/

# Stacks-n-Queues
Stacks and Queues



You are to code the following:

    A Stack backed by a singly-linked list without a tail reference.

    A Stack backed by an array

    A Queue backed by a singly-linked list with a tail reference

    A Queue backed by an array

A Stack is a last-in, first-out (LIFO) data structure; the last item to be inserted is the first item to be removed. A Queue is a first-in, first-out (FIFO) data structure; the first item inserted is the first item to be removed.

All your data structures must follow the requirements stated in the javadocs of each method you must implement.

Note that the linked versions of the data structures should NOT be circular.

Capacity

The starting capacity of the array classes should be the constant INITIAL CAPACITY defined in the .java files. Reference the constant as-is. Donot simply copy the value of the constant. Do not change the constant. If, while adding an element, the array class does not have enough space, you should regrow the backing array to twice its old capacity. Do not resize the backing array when removing elements.

Removing

With both array classes, when elements are deleted from the array, the index the element was removed from should be set to null. All unused positions in the backing array must be set to null.

Circular Arrays

The backing array in your ArrayQueue implementation must behave circularly. This means the front variable might wraparound to the beginning when you remove to take advantage of empty space while maintaining O(1) efficiency for all operations.

For this assignment, the front variable in ArrayQueue should represent the index that holds the next element to dequeue. Failure to follow this convention will result in major loss of points.

For enqueuing, add to the back of the queue. To access the back of the queue, you can add the size to the front variable to get the next index to add to, though you will have to account for the circular behavior yourself. If there are empty spaces at the front of the array, the back of the queue should wrap around to the front of the array and make use of those spaces.

For dequeuing, you should simply treat the next index in the array as the new front. Do not shift any elements during a remove.

When resizing the backing array, “unwrap” the data. Realign the queue with the front of the new array during the transfer. The front variable of the queue is once again at index 0.

Additionally, after removing the last element in the queue, move the front variable like you normally would. Do not explicitly reset it to 0. This effectively means that going from size 1 to size 0 should not

Homework 2: Stacks and Queues Due: See Canvas

be a special case for your code.

The examples below demonstrate what the queue should look like at various states.

In the example below, the queue begins empty (initial state). An element is added.

In the example below, adding to the back causes the newly added element to wrap around to the front.

In the example below, adding another element causes the queue to resize. The array capacity is doubled and the front element moves to index 0.

In the example below, the last element of the queue is removed, but front moves as expected. The front variable is not explicitly set to 0.

Homework 2: Stacks and Queues Due: See Canvas

Grading

Here is the grading breakdown for the assignment. There are various deductions not listed that are incurred when breaking the rules listed in this PDF and in other various circumstances.

Methods:
	
	

ArrayStack constructor
	

1pts
	

ArrayStack push
	

7pts
	

ArrayStack pop
	

6pts
	

ArrayStack peek
	

4pts
	

LinkedStack push
	

6pts
	

LinkedStack pop
	

7pts
	

LinkedStack peek
	

4pts
	

ArrayQueue constructor
	

1pts
	

ArrayQueue enqueue
	

10pts
	

ArrayQueue dequeue
	

8pts
	

ArrayQueue peek
	

4pts
	

LinkedQueue enqueue
	

6pts
	

LinkedQueue dequeue
	

7pts
	

LinkedQueue peek
	

4pts
	

Other:
	
	

Checkstyle
	

10pts
	

Efficiency
	

15pts
	

Total:
	

100pts
	

Provided

The following file(s) have been provided to you. There are several, but we’ve noted the ones to edit.

    ArrayStack.java

This is the class in which you will implement the ArrayStack. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance vari-ables, or static variables.

    LinkedStack.java

This is the class in which you will implement the LinkedStack. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance vari-ables, or static variables.

    ArrayQueue.java

This is the class in which you will implement the ArrayQueue. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance vari-ables, or static variables.

    LinkedQueue.java

This is the class in which you will implement the LinkedQueue. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance vari-ables, or static variables.

    LinkedNode.java

Homework 2: Stacks and Queues Due: See Canvas

This class represents a single node in the linked list. It encapsulates the data and the next reference. Do not alter this file.

    StackStudentTest.java

This is the test class that contains a set of tests covering the basic operations on the Stack classes. It is not intended to be exhaustive and does not guarantee any type of grade. Write your own tests to ensure you cover all edge cases.

    QueueStudentTest.java

This is the test class that contains a set of tests covering the basic operations on the Queue classes. It is not intended to be exhaustive and does not guarantee any type of grade. Write your own tests to ensure you cover all edge cases.

Deliverables

You must submit all of the following file(s). Make sure all file(s) listed below are in each submission, as only the last submission will be graded. Make sure the filename(s) matches the filename(s) below, and that only the following file(s) are present. If there are multiple files, do not zip up the files before submitting; submit them all as separate files.

Once submitted, double check that it has uploaded properly on Gradescope. To do this, download your uploaded file(s) to a new folder, copy over the support file(s), recompile, and run. It is your sole responsibility to re-test your submission and discover editing oddities, upload issues, etc.

    ArrayStack.java

    LinkedStack.java

    ArrayQueue.java

    LinkedQueue.java

