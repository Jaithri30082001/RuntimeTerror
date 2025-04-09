TIME COMPLEXITY - O(N) and SPACE COMPLEXITY - O(N)

APPROACH: 
- for the given string - the first step is to remove the spaces and extra spaces in the given string - we do that using erase and remove
- the second step is to consider only letter and digits - if at all the letters are upper case
- we have to convert the upper cased letters into lower case and then append these to an empty string.
- to check if the character is an alphabet we use - isalpha(ch)
- to check if the character is a digit we use - isdigit(ch)
- to check if the character is uppercase we use - isupper(ch)
- to convert a character to lower case we use - to_lower(ch)

- and then one we get a string with all lower case alphabets and digits only - we consider two pointer
- i beign 0 (initial index of the string) and j being the last position of the string
- while i is less than or equal to j - we keep on comparing the character at ith position and jth position - if at all they are not equal - we return false
- else the loop continues and once the loop is completed - we will return true
- 
END;
