TIME COMPLEXITY - O(N) and SPACE COMPLEXITY - O(1)
APPROACH:
- According to the question - you have to rotate the given array by k positions
- there might be test cases where the value of k > the length of the given array - in such cases we have to reduce k to k % nums.size() - and also rotating an array k
and k * n times give same result anyway. So it is better to reduce k to k % nums.size()
- and then we first reverse the entire array
- next we reverse the first part of the array till k positions
- and next we reverse the second part of the array from k positions to the end
- that way we will have an array that is roated by k positions - for this in c++ we made use of the reverse fucntion
- reverse(nums.begin(), nums.end) -> reverses the entire array
- reverse(nums.begin(), nums.begin() + k) -> reverses the array but only till k positions from the start
- reverse(nums.begin() + k, nums.end()) -> reverses the remaining portion of the array.
