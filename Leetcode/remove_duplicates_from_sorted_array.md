APPROACH - 1
TIME COMPLEXITY - O(N**2) and SPACE COMPLEXITY - O(1)
- Here we made use of a two pointer appraoch - and whenever there are same elements - we pushed the second element to the end of the vector and then erased this
second element using an erase function.
- Since erase takes a time complexity of O(N) in worst case - when used inside a for loop makes the time complexity equal to O(N**2)
- and at last return i + 1 - which is the track of unique elements here

APPROACH - 2
TIME COMPLEXITY - O(N) and SPACE COMPLEXITY - O(1)
- Here we iterate through the entire vector using a for loop and there are two variables or points we may say - the first pointer i - keeps track of the unique elem
ments and the second pointer j - it helps us compare the ith element to the remaining elements of the vector
- whenever the ith element is not equal to the jth element - we make the i + 1th element equal to the jth element - this brings all the unique elements to the front
  of the array
- at last when j reaches the end of the array - i will have the last position in all the unique elements the array had - the number of unique elements will be given
by i + 1
