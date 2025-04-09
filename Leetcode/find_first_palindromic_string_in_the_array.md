TIME COMPLEXITY - O(N * M) and SPACE COMPLEXITY - O(1)
APPROACH:
- for every word in the string
- you place two pointers - one at the beginning and the other at the ending
- and declare a temp variable - which is zero
- while i is less than or equal to j - you check if the characters at the positions i and j are same or not
- if they are not same - then you make temp = 1 and then break the while loop - moving to the next word
- if they are same - then you increase i by 1 and decrease j by 1 - and after the while loop is run successfully (without breaking) - that means the given word is a palindrome
and you return the word - that ends there
- if there are no such words - the previous return statement would not work - so after the for loop - you return an empty string
- if the word is not returned by the function - at the end the empty string will be returned
- 
