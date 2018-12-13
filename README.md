# Merge-Sort



Implementation of data structures and algorithms  
Fall 2018  
Short Project 9: Divide and conquer algorithms  

Authors - Team SP7 2
- Prateek Sarna (pxs180012)
- Bharath Rudra (bxr180008)

Files Included
- SP9.java

Task
- Implement and compare the running times of the following algorithms on randomly generated arrays:  
(a) Insertion sort,  
(b) Merge sort (take 1),  
(c) Merge sort (take 2),  
(d) Merge sort (take 3).  
Do not run more than one algorithm in each trial.  
For Insertion sort, if the running time exceeds 2 min, write the time as infinity.  
For Merge sort, in each trial, run only one algorithm, for one value of n, 100 times in a loop, and taking the average time.  
Try the following values of n: 8M, 16M, 32M, 64M, ..., until you get out of memory exception.

Merge Sort (take 1)
- Normal merge sort done by splitting the given array and merging them in a sorted order

Merge Sort (take 2)
- Improvements
  - Do not allocate new arrays each time in merge
  - Stop recursion below a threshold
  
Merge Sort (take 3)
- More Improvements
  - Avoid unnecessary copying from A to B in merge
  - Change for loop to while loop (only java)
  
Results
- Here, n is the size of the array(number of inputs).
- For merge sort, the time reported is the observed average of 100 trials.
- Insertion Sort would take over 2 minutes for input size of about 1000000, hence marked as infinity.

- For n = 8M
  - Insertion Sort	: Infinity
  - Merge Sort Take1: Time: 2184 msec. Memory: 110 MB / 157 MB
  - Merge Sort Take2: Time: 1942 msec. Memory: 79 MB / 129 MB
  - Merge Sort Take3: Time: 1805 msec. Memory: 79 MB / 129 MB

- For n = 16M
  - Insertion Sort	: Infinity
  - Merge Sort Take1: Time: 3883 msec. Memory: 125 MB / 165 MB
  - Merge Sort Take2: Time: 3056 msec. Memory: 125 MB / 128 MB
  - Merge Sort Take3: Time: 3757 msec. Memory: 94 MB / 129 MB

- For n = 32M
  - Insertion Sort	: Infinity
  - Merge Sort Take1: Time: 8819 msec. Memory: 248 MB / 275 MB
  - Merge Sort Take2: Time: 6380 msec. Memory: 247 MB / 251 MB
  - Merge Sort Take3: Time: 5880 msec. Memory: 247 MB / 251 MB

- For n = 64M
  - Insertion Sort	: Infinity
  - Merge Sort Take1: Time: 16517 msec. Memory: 492 MB / 681 MB
  - Merge Sort Take2: Time: 13472 msec. Memory: 491 MB / 618 MB
  - Merge Sort Take3: Time: 12184 msec. Memory: 491 MB / 618 MB

- For n >= 128M	: Memory Exception
