# Fifo answer to write 

## AIM: To write c program to implement FIFO page replacement algorithm.

## Description:
### In an operating system that uses paging for memory management, a page replacement algorithm is needed to decide which page needs to be replaced when new page comes in. 
### Page Fault – A page fault happens when a running program accesses a memory page that is mapped into the virtual address space, but not loaded in physical memory. 
### First In First Out (FIFO) – 
### This is the simplest page replacement algorithm. In this algorithm, the operating system keeps track of all pages in the memory in a queue, the oldest page is in the front of the queue. When a page needs to be replaced page in the front of the queue is selected for removal. 

## Algorithm:

### 1. Initialize an empty frame of size frames.
### 2. Set pageFault = 0 and frameCount = 0.
### 3. For each page in the pages array:
### 4. If the page is not in the frame:
### 5. Replace the page at frameCount with the current page.
### 6. Increment frameCount (modulo the frame size for circular replacement).
### 7. Increment pageFault.
### 8. If the page is already in the frame, do nothing.
### 9. At the end, return pageFault.

## Output :

Enter the number of pages (<1000):

10

Enter 10 pages:

2 3 2 1 1 4 5 3 4 6

PAGE FAULTS = 7
