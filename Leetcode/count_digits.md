cout_digits
Time Complexity - O(logN)
Space Complexity - O(1)

Approach:
step - 1: we declare a vector - to hold all the digits individually of the given number

step - 2: we copy the given number into a variable called copy_num and declare the count to be zero (this is where we store the count of the digits that exactly divide the number)

step - 3: we start a for loop for the condition where the copy num should be greater than zero only - cause the this number will be divided by 10 for every iteration 

step - 4: in the while loop - we extract the last digit of the given number by using mod and the divisor is 10

step - 5: we check if the extracted last digit is equal to zero or not - if it is not equal then we add it to the vector we declared earlier using emplace_back() 

step - 6: and then we do copy_num = copy_num / 10 - inorder to get just the quotient which now no longer has the last digit

step - 7: after all of the digits are extracted into the vector - then we run a for each loop and check if the digits in the vector divide the given number exactly or not - we know the condition that is - if the mod of the given number and the digit are zero - then we increase the count of the number of divisors.

step - 8: return the count

THE END
