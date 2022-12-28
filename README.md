# MULTITHREADING:
Multithreading is the ability of a central processing unit (CPU, or a single core in a multi-core processor) or a single processing element within a multi-core processor to execute multiple threads concurrently, supported by the operating system. The various threads share the same process resources, including memory and open files.
Multithreading allows a program or an operating system to perform two or more tasks concurrently within a single process. This is done by allowing each task to interrupt the current task, and then resume it later.
There are two main types of multithreading:
•	Process-based multithreading: Each thread has its own process, which means that each thread has its own set of resources, such as memory and open files. This type of multithreading is more resource-intensive, but it allows for greater flexibility and control over the threads.
•	Thread-based multithreading: All threads share the same process, which means that they share the same set of resources. This type of multithreading is more efficient in terms of resource usage, but it requires more careful management to ensure that the threads do not interfere with each other.
Multithreading is commonly used in software applications to increase the performance and responsiveness of the program. For example, a web browser might use multithreading to allow the user to continue browsing while a large page is loading in the background.
In the task manager there are 4 cores in our system. As you can see in the attached image.

 

The python code uses the threading library to parallelize the merge sort function over 4 threads. The parallel_merge_sort function splits the input array into num_threads equally sized chunks and creates a thread for each chunk. Each thread sorts its chunk using the merge_sort function, and then the sorted chunks are merged using the merge function.
Steps to implement Multithreading in Merge sort is:
1.	Base case is if the array has length 1, it is already sorted. 
2.	Split the array in half and sort the two halves recursively.
3.	Merge the sorted halves and return the result.
4.	Initialize the merged array and the indices for the left and right halves.
5.	Iterate over the left and right halves, adding the smaller of the two elements.
6.	At each step to the merged array, add the remaining elements (if any) to the merged array.
7.	Create a list of threads.
8.	Split the array into num_threads equally sized chunks.
9.	Create a thread for each chunk and start it.
10.	Wait for all threads to finish.
11.	Merge the sorted chunks and return the result.
12.	Generate a random array of integers to sort.
13.	Sort the array using 4 threads.
14.	Print the sorted array.
