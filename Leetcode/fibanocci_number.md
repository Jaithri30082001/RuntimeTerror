There are three approaches for this - the normal recursive approach - the top - down approach in DP and - the bottom - up approach in DP
The recursive approach is inefficient cause it takes O(2 ^ n) TC and O(n) - call stack for the Space complexiy
The other two approaches take O(n) Time complexity and O(n) Space complexity respectively

The recursive approach: TC - O(2 ^ n) and SC - O(n)[call stack]
- First we identify the base case - if n is less than or equal to one - then we return n it self
- else we keep on recursively calling the function with parameters n - 1 adding it with recursive calling of the function with parameters n - 2

The Bottom - up approach: TC - O(n) and SC - O(n)
- For this we initialize an array with 0 and 1 at the beginning only - as the fibanocci series starts with 0 and 1
- later we take a for loop and till n - we keep on adding the last two numbers of the vector and push the result back into the vector
- and finally after the for loop is done - we return the value at nth index

The Top - down approach: TC - O(n) and SC - O(n)
- For this we make use of memoization - we initialize a dp array - with -1
- and in the function fib - if the value of n is less than 1 then we return n (base case)
- if the value is already present in the dp array (i.e., if dp[n] is not -1) then we return dp[n]
- else we replace the calculated value (fib(n - 1) + fib(n - 2)) at the nth position in the dp array (so that we need not calculate the value always)

END/
