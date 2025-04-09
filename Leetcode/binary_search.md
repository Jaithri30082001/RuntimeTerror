TIME COMPLEXITY - O(logN) and SPACE COMPLEXITY - O(1)

 APPROACH:
 - we have to initialize three variables - low, high and mid -> apparently low being the 0 at the beginning, high being the size of the array and mid being the avg(low and high)
 - and while low is less than or equal to high - we keep on checking if the mid is equal to the target
 - if the target is greater than the mid - then we increase the low to the next position of the mid (low = mid + 1)
 - if the target is less than the mid - then we decrease the high to the previous position of the mid (high = mid - 1)
 - eventually at one point you either find out the targer OR low will be greater than high
 - if you find the target - you return true or the index of the element - and if the target is not found - we return -1 or false
 - AND IT IS IMPORTANT FOR THE ARRAY TO BE SORTED FOR US TO PERFORM BINARY SEARCH
