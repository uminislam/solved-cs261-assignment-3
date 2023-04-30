Download Link: https://assignmentchef.com/product/solved-cs261-assignment-3
<br>
<h2>Problem 1: Linked List Deque and Bag implementation</h2>

First, complete the linked list implementation of the deque (as in Worksheet 19) and bag ADTs (Worksheet 22). To do this, implement all functions with the // FIXME… comments in

<h2>Problem 2: Linked List vs Dynamic Array performance comparison</h2>

The files linkedListMain.c and dynamicArrayMain.c each contain code which does the following:

<ol>

 <li>Takes an integer argument (say n) from the command line and adds that many elements to the bag.</li>

 <li>Prints the memory in KB used by the bag.</li>

 <li>Calls the contains function for each element in the bag.</li>

 <li>Prints the time taken by these contains calls in milliseconds.</li>

</ol>

Your job is to compare the performance of the linked list implementation vs the dynamic array implementation over various numbers of elements. Create a plot comparing performance over element counts from n=2<sup>10</sup> to n=2<sup>18</sup>, doubling n for each data point, for each of the following metrics:

<ol>

 <li>Memory usage ­­ linked list vs dynamic array for n in [2<sup>10</sup>, 2<sup>18</sup>].</li>

 <li>Running time ­­ linked list vs dynamic array for n in [2<sup>10</sup>, 2<sup>18</sup>].</li>

</ol>

Important: Please run all memory usage and timing tests using <strong>valgrind </strong>on flip for consistency. The memory calculation code runs on flip only. Please follow the instructions in linkedListMain.c and dynamicArrayMain.c to comment out the memory code if you develop your programs in Visual Studio.

You must also implement the dynamic array. Use the implementation from Assignment 2 or the previous week’s worksheets. Note that in dynamicArrayMain.c the dynamic array must have a capacity of 2<sup>10</sup> to start with.

After creating the two plots, answer the following questions:

<ol>

 <li>Which of the implementations uses more memory? Explain why.</li>

 <li>Which of the implementations is the fastest? Explain why.</li>

 <li>Would you expect anything to change if the loop performed remove() instead of contains()? If so, why?</li>

</ol>

<h2>Problem 3: Circularly Linked List Deque implementation</h2>

For this problem, you will implement the Deque ADT with a Circularly­Doubly­Linked List with a Sentinel. As you know, the sentinel is a special link, does not contain a meaningful value, and should not be removed. Using a sentinel makes some linked list operations easier and cleaner in implementation. This list is circular, meaning the end points back to the beginning, thus one sentinel suffices. Implement all functions with the // FIXME… comments in circularList.c .