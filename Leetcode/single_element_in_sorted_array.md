TIME COMPLEXITY - O(logN) and SPACE COMPLEXITY - O(1)
APPROACH - Binary Search
- let l - be the low of the array and h be the high of the array -> l = 0 and h = last index of the array
- check if the value at index l is equal to the next value -> i.e., nums[l] == nums[l + 1] if it is not equal then return l
- similarly check if the value at index h is equal to the previous value -> i.e., nums[h] == nums[h - 1] if it is not equal then return h
- if both the values are equal to the next and previous elements - then increae l by 2 and decrease h by 2 (since there are only 2 elements in the array)
- and hence the while loop runs till the value of l is less or equal h and l and h doesn't cross the array
- and if none of these cases are true - then that means there is only one element in the array - and you return that element at the end.
END /

Well done - you came with this solution in less than 15 minutes - you are definitely improving - keep going.
