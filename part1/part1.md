# Part 1a
## var declaration
1) "values added: 20" 
   > This is the case because in the function call, we passed true for the value of add and therefore we will enter into the block of code. Inside the block of code, we will declare 
   a variable result which stores the value of the added numbers which is then returned.

2) "final result: 20"
   > In this case, after we have exited the block of code, the value of the variable result is still present and therefore we will return the same value as above.

## let declaration
1)  "values added: 20"
   > In this case, because the print statement in line 9 is in the same block of code as the variable declaration, we still have access to the variable and therefore we are able to
   print this as normal.

2) The code will return an error.
   > Due to the variable being declared using the let keyword, the print statement in line 13 will not have access to the result variable and therefore will not be able to print
   the value that was held by the result variable. Because it tries to print the value of a variable that it does not have access to, this statement will throw an error.

## const declaration
1) This line of code will throw an error
   > Because the const keyword does not allow for the user to reassign the value of the variable after it has already been assigned, the line where the code assigns the sum of the numbers to the result will end up throwing an error.

2) This line will throw an error
   > Using the same reasoning as above, because the line above it would have tried to reassign the value of the variable, this will throw an error. Also, in the end, due to the scope of the const keyword, we would not be able to access the variable anyways when printing which would also result in an error.

# Part 1b
1) This will print the length of the prices array which is 3 in this case.
   > By going through the for loop, starting at 0, it will iterate through the value until the value of i is no longer less than the length of the array. This occurs when the value of i is exactly equal to the length of the array and therefore will return the length of the array.

2) This will print the discount price of the last element in the array which would be 150.
   > In this case, discountedPrice stores the discounted price of each value in the array as the iterate through the array. After the loop is over, it will retain the value of the discounted price of the last item used to calculate it which is the discounted price of 300, or 150.

3) This line will print the value of the discounted price rounded to the nearest cent of the last value in the array which is 150
   > This is the same as above where the variable will take on the last value that was passed to it. The math.round will round the value to the nearest integer but because we are dealing with integers already, there is no rounding occuring.

4) This function will return the array of prices given after the discounts are applied.
   > In the loop, after everything is calculated, the final value is pushed into the empty discount array. The push operation will add the value to the back of the array and therefore will return the discounted prices in the same order they were added in.

5) This will throw an error.
   > Because we used the let keyword in the for loop declaration, we are able to only use the variable i within the for loop. Therefore, when we call the print statement outside of the for loop, it will throw an error as it no longer has access to the variable i declared.

6) This will throw an error.
   > Using the same reasoning as above, because the variable discountedPrice is declared within the for loop using let, the print statement will not have access to the variable and therefore, when accessing it, it will not find a variable to access and will throw an error.

7) This will return the final price of the last element in the passed array.
   > Unlike the past two cases, this will work because the variable was declared in the same block as the print statement using let. Because they are in the same block, the print statement will have access to it and therefore will have a value to print.

8) This will return an array of discounted prices in the order they were passed.
   > Again, because the variable was declared using let within the same block as the print statment, the values will be added and printed as intended as there will be no access issues in this case.

9) This will again throw an error.
   > This will throw an error because the variable i will have been declared using let within the for loop and therefore cannot be accessed by the print statement afterwards.

10) This will print the length of the array which is 3.
   > The variable length is initialized to the value 3 from the declaration and it is within the same block as the print statement therefore the length of the array will be printed.

11) This function will return the discount prices in the order they were passed.
   > Even though the array was declared as a constant and the variable discountedPrice is also declared as a const, this code will still work as intended. The constant array, although it is constant, can still have values added to it and the const variable within the array is redeclared at every loop meaning that nothing is violated by this code.

12a) student.name;
12b) student["Grad Year"];
12c) student.greeting();
12d) student["Favorite Teacher"].name;
12e) student.courseLoad[0]

13a) '32'
   > This is because when adding a string of an integer to another integer, it is the same as concatenating two strings together and therefore will produce the merged string.
13b) 1
   > When subtracting, there is no string equivalent for subtracting and therefore, javascipt will convert the string integer into a regular integer then subtract.
13c) 3
   > This is because the null data value evaluates to the value of 0 when being added to an integer. Therefore, this statement is the same as adding 0 to 3.
13d) 3null
   > The null value can also be treated as a string and therefore, with the addition operation, will be concatenated to the end of the 3 string to form the above output.
13e) 4
   > True evaluates to 1 in terms of integers and therefore will simply be added to the integer 3 to get 4.
13f) 0
   > Both false and null are treated as integers when it comes to the addition operation. Also javascript treats both these values as 0 so this is equivalent to adding 0 to 0.
13g) 3undefined
   > Because the 3 is a string with the addition operation, it will treat the undefined as a string as well and concatenate the values together.
13h) NaN
   > Because the string type does not have a subtraction operation to it, it will try to convert the values into integers. Then, because we are operating with undefined, we will get NaN as an output.

14a) True
   > Javascript will convert the string to its integer equivalent which is simply the same but as an integer. Then because the integer 2 is greater than the integer 1, this statement will return true.
14b) False
   > Javascript will go letter by letter and therefore will compare the string 2 to the string 1. In this case, the string 1 is less than the string 2 and therefore this statement will return false.
14c) True
   > JS will convert the string into its integer equivalent then compare. In this case, the string of 2 will also become the integer 2 and therefore the comparison will also evaluate to true.
14d) False
   > This function will always return false when the items are of different types. In this case we are comparing strings to integers and therefore this will return false.
14e) False
   > This will also return false because the integer value of true is always equal to 1 meaning that when the integers are compared, the statement will return false.
14f) True
   > The boolean function will equate to true as long as the value passed is not equal to 0. In this case, we are passing the value of 2 and therefore the boolean function will evaluate to true which is equivalent to true.

15) The == operators will just try to see if the values, regardless of data type, are the same. In order to do this, it might convert the values to similar data types in order to compare. The === operator on the other hand checks if the objects are strictly equal to one another data type and all. This means that if the data types are different, it will always return false.

16) See file.

17) The function will return an array that contains the doubled values of the passed in array meaning the result will be: [2, 4, 6].
   > The function defined in the first block of code takes in parameters that specify an original array as well as the function that will be used on the array. Then, in the first line, the function will create a new empty array that will be used to store the new values generated from the old array. In the for loop, the block of code will iterate through all items within the passed array and pass the value in the array through the passed function. After the array value is processed, the new value will be added to the new array then returned at the end. In this case, the function passed, acts to multiply the value of the array element by 2 meaning that the returned array will contain values equal to two times the values of the original array values.

18) See file.

19) This will print the values: 1 4 3 2.
   > In the function, the print statement for the values of 1 and 4 are placed on their own while the print statement for the values of 2 and 3 are placed within setTimeout blocks. This means that when the function is called, it will immediately run the code for printing 1 and 4, in that order because that is the order it is defined, then it will procede to run the print statements within the setTimeout blocks. The print statement for the value 3 will run immediately at this point because the delay set by the function is set to 0 meaning that the code will run immediately in the next cycle. Then, because the delay for the print statement of the value 2 is set to 1000, the function will wait for 1 second before printing the value of 2.