reverse_integer
Time complexity - O(log(N))
Space complexity - O(1)
The approach is as follows:

step 1 - we declare a long long variable - cause - the reversed integer might be turning into something which is more than an integer - so we declare a long long

step 2 - then we copy the given integer into another variable - cause it is a bad idea to alter the given data 

step 3 - we run a while loop for a condition where temp is greater than 0 - and in that for loop - we extract the last digit of the given integer - check the status of ans (it is mentioned in the question that the ans should not exceed the range of a 32 bit integer) - hence we check it with INT_MAX / 10 and INT_MIN / 10 - if at all any of the conditions are true  - we immediately return a zero - else we add the last digit to the ans multiplied by 10 and then reduce temp to temp / 10 - and this entire process repeats 

step 4 - we return the ans

THE END
