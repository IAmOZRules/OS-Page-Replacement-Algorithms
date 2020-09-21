# OS-Page-Replacement-Algorithms
FIFO, LRU and Optimal Page Replacement Algorithms in Python3

## **FIFO Page Replacement (First In First Out)**

This is the simplest page replacement algorithm. In this algorithm, the operating system keeps track of all pages in the memory in a queue, the oldest page is in the front of the queue. When a page needs to be replaced page in the front of the queue is selected for removal.

## **LRU Page Replacement (Last Recently Used)**

In this algorithm page will be replaced which is least recently used.

## **Optimal Page Replacement**

In this algorithm, pages are replaced which would not be used for the longest duration of time in the future.

### Sample (Using FIFO): 
Enter the number of frames: 3
Enter the reference string: 4 7 6 1 7 6 1 2 7 2

String|Frame →	0 1 2  Fault
   ↓

   4		      4      Yes
   7		      4 7    Yes
   6		      4 7 6  Yes
   1		      1 7 6  Yes
   7		      1 7 6  No
   6		      1 7 6  No
   1		      1 7 6  No
   2		      1 2 6  Yes
   7		      1 2 7  Yes
   2		      1 2 7  No

Total requests: 10
Total Page Faults: 6
