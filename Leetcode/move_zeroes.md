TIME COMPLEXITY - O(N) and SPACE COMPELXITY - O(1)
Approach:
- given an array that contains zeroes in between and we have to move those zeroes to the end of the array, without changing the order of the other elements
- there are two functions that we can use here - the first one - we can use remove (remove takes all the mentioned elements to the end of the array and gives
you the iterator of the same)
- and then we use the erase function to erase all the elements from the given iterator, we have to note that there will be no change in the order of the elements when
we remove the zeroes
- and once we remove them all - we must have counted the zeroes at the beginning, i.e. before removing them and then we run a for loop till the value of the number of
zeroes and add those many zeroes to the end of the array
- and all of this is done inplace - without using extra space

END;
