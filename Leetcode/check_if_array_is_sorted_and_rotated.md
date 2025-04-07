TIME COMPLEXITY - O(NlogN) and SPACE COMPLEXITY - O(N)
Approach: 
-  For this particular problem, we have to check if the given array is a sorted array which is rotated by x positions
-  for this we have to divide the array into two parts
-  the roated portion and the beginning portion, that starts with the first element of the sorted array
-  it was given in the question that a sorted array A is rotated by x positions if B[i] == A[(i + x) % A.lenght]
-  based on this condition we have to find x. Once x is foundthen we can validate this condition by running a for loop and for the value of x to be found
-  we iterate through the array and get the index of the element where the B[i] > B[i + 1] where i < B.length.
-  Since this is a sorted array every first element will be smaller than the next element
-  when this condition is broken - we can say that that is the index where the array has been rotated
-  and on substracting that index from the length of the array - we will get the number of positions that the array has been roated by
-  then we can find if the array is sorted and rotated or not by the condition given
-  if sorted we return true else we return false;
