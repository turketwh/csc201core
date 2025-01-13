***Note**: This document is a draft until this header is removed...*

# CSC 201: Preparation Guide For Module 2

## Read

Read the following sections of the OpenDSA textbook linked from the course Canvas site Module 0: (the first link below will take you to the appropriate starting point)
* [Section 8.4](https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/AnalCases.html) 
* Section 13.2
* Section 13.3

You may find my Java instructions below of an insertion sort for `int` arrays easier to read than the one shown in Section 13.3 (which is generic (can apply to more types than `int`)).
```
public void insertion_sort(int[] data) {  
	int temp;  
	int i;  
	int j;  
	for (i = 1; i < data.length; i++) { // Insert ith record  
		for (j = i; (j > 0) && (data[j] < data[j-1]); j--) {  
			temp = data[j];
			data[j] = data[j-1];
			data[j-1] = temp;
		}
	}  
}  
```

The major points to focus on in the reading are:
* The key difference in the concepts of *best case*, *worst case*, and *average case* costs (cost meaning "amount of work required") for an algorithm
* Which of the cases (*best*, *worst*, and *average*) we are usually most interested in for an algorithm
* The definition of the *sorting problem*
* The fundamental *operation* traditionally used when analyzing sorting algorithms
* The general idea of how the *insertion sort algorithm* does its work of putting a collection of values in sorted order

The notation of $O$ and $\theta$ appear in the reading. If you don't remember those from or weren't exposed to those in a previous course, no worries - we'll formally define them ourselves soon.
## Assess
After completing the work indicated above, answer the questions in the *Module 2 Preparation Assessment* in the course Canvas site by the deadline indicated in Canvas.
