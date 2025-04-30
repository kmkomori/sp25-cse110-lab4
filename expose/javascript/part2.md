1. What will happen at line 12 and why? If the code causes an error, explain why.

    Line 12 prints "3". This is because there were 3 prices to be discounted, and the index variable in the for loop was declared using the keyword 'var'. This means the variable value persists outside of the block, which is why we are still able to access and print it outside of the for loop.

2. What will happen at line 13 and why? If the code causes an error, explain why.

    Line 13 prints "150". This is because the variable 'discountedPrice' was declared using keyword 'var', meaning the value persists outside of its code block. In this case, the final value of 'discountedPrice' is the discounted price of the final item in the original 'prices' array, which is 300. At a 50% discount, the value printed is 150.

3. What will happen at line 14 and why? If the code causes an error, explain why.

    Line 14 prints "150". This is because the variable 'finalPrice' holds the discounted version of the current item's price when parsing through the list of item prices. The value persists even after the loop ends due to the fact that it is declared with the keyword 'var'. So the value of the 'finalPrice' variable will be the discounted (50%) price of the last item in the list (300), which is 150.

4. What will this function return? Give a brief explanation why. If the code causes an error, explain why.

    This function returns an array of the discounted prices, based on the array of prices and discount rate passed into the function. This code works because the return variable 'discounted' is well maintained (i.e. not overwritten, lost, etc.) and the logic of the function is correct.

5. What will happen at line 12 and why?  If the code causes an error, explain why.

    Line 15 causes the error "ReferenceError: i is not defined". This is because 'i' refers to the indexing variable for the for loop. But the variable is declared using the keyword 'let'. This means the variable is block scoped, and cannot be accessed outside of its scope. In this case, the scope of the variable is the for loop. Therefore, we are unable to access the variable outside of the for loop, such as the console log called in line 12.

6. What will happen at line 13 and why? If the code causes an error, explain why.

    Line 13 causes the error "ReferenceError: discountedPrice is not defined". This happens because discountedPrice is declared using the 'let' keyword. That means it is block scoped, and cannot be accessed outside of the block of code in which it is declared. Because the console.log command is called outside of the for loop, it is unable to access the variable.

7. What will happen at line 14 and why? If the code causes an error, explain why.

    Line 14 prints "150". This is because although the variable is declared using the 'let' keyword, it is declared at the beginning of the function, outside of any code blocks. The 'let' keyword is block scoped, but if a variable is declared inside a function but outside of any code blocks, it is accessible anywhere inside the function. So our console.log is able to access the variables value, which is the discounted price of the last item in the 'prices' array.

8. What will this function return? Give a brief explanation. If the code causes an error, explain why.

    This function returns the array of discounted prices based on the array of prices and discount rate passed into the function. It is able to implement this functionality because the 'let' variable declaration of the returned array 'discounted' allows for the array to be persistently maintained within the function, so it returns the correct value.

9. What will happen at line 11 and why? If the code causes an error, explain why.

    Line 11 causes the error "ReferenceError: i is not defined". This is because the variable 'i' was declared using the 'let' keyword, which is block scoped. This means the variable is inaccessible outside of the code block in which it is declared. Because we try to reference 'i' outside of the for loop it's declared in it causes an error.

10. What will happen at line 12 and why? If the code causes an error, explain why.

    Line 12 prints "3". This is because the variable 'length', although const and block scoped, is declared at the beginning of the function. That means it is accessible at any point within the function, including after the for loop. So we print its value, which is the length of the input 'prices' array.

11. What will this function return? Give a brief explanation. If the code causes an error, explain why.

    This function returns an array of the discounted prices based on the input prices array and the discount rate. In this specific case, with the inputs [100, 200, 300] and 0.5, it returns the array [50, 100, 150]. We would expect this to not work because the return array is declared as a const. But it works becasue the const refers to a constant reference to an array location, not necessarily the contents of the array being constant.

12. Given the above Object, write the notation for:

    A. Accessing the value of the name property in the student object = student.name

    B. Accessing the value of the Grad Year property in the student object = student['Grad Year']

    C. Calling the function for the greeting property in the student object = student.greeting()

    D. Accessing the name property of the object in the Favorite Teacher property in student = student['Favorite Teacher'].name

    E. Access index zero in the array of the courseLoad property of the student object = student.courseLoad[0]

13. Arithmetic

    A. '3' + 2 outputs '32' because the number 2 is converted to a string then concatenated using the + operator.

    B. '3' - 2 outputs 1 because the subtraction operator converts the string into a number and then operates on the two values.

    C. 3 + null outputs 3 because null is converted to a 0 due to the numeric operator +.

    D. '3' + null outputs '3null' because the first value is a string and + concats strings together, so null is converted to a string.

    E. true + 3 outputs 4 because the + is a numeric operator, so the true value is converted to its numeric counterpart 1.

    F. false + null outputs 0 because the + is a numeric operation, so both false and null were converted to their numeric counterpart 0.

    G. '3' + undefined outputs '3undefined' because '3' is a string and in the context of strings + is for concatenation, so undefined is converted to its string counterpart, 'undefined'.

    H. '3' - undefined outputs NaN because the - is a numeric operator. The string '3' can be converted to a number, but undefined cannot, so the result of the operation is NaN (not a number).

14. Comparison

    A. '2' > 1 outputs true because one of the values is numeric, so the string '2' is converted to a number and compared, which results in true.

    B. '2' < '12' outputs false because they are both strings, so are compared lexicographically. '1' is lexicographically less than '2', so this operation returns false (even though mathematically 2 is less than 12).

    C. 2 == '2' outputs true because this is the equality operator, so one value is converted to match the other then compared for equality (in this case, the string should be converted to a number). Once converted, they have the same value, so the output is true.

    D. 2 === '2' outputs false because this is the strict equality operator, which means the type and value must both be equal. Because one is a string and the other is a number, it automatically fails and returns false.

    E. true == 2 outputs false because the boolean is converted to its numeric counterpart 1 for this comparison, and 1 does not equal 2.

    F. true === Boolean(2) outputs true because the Boolean() function converts any variable to a boolean. For numbers, 0 and NaN is false, while every other value is true. 2 is converted to the boolean true, so it is equal to true.

15. Explain the difference between the == and === operators.

    '==' is the equality operator. It compares the values of the two objects after converting them to the same type. '===' is the strict equality operator. It compares both the value and type of both objects. In that sense it is stricter than the equality operator, as it does not convert the types of the two objects before comparing them.

17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result.

    The function returns the array [2,4,6]. Into the modifyArray function we pass in the array [1,2,3] with the doSomething function as the callback. The doSomething function takes in a number as a parameter and returns that number doubled. In modifyArray, they take each element of the parameter array and put it through the doSomething (callback) function before adding it to the new return array. Thus, the variable returned is an array of every element in the input array doubled.

19. What is the output of the above code?

    The output of printNums() is:

        1
        4
        3
        2

    Each line of code is put onto the stack. Line 2 is executed immediately. Line 3 puts a console.log on the stack with a delay of one second. Line 4 puts a console.log on the stack with no delay. The next line on the stack is line 5, which executes immediately. Then the next line on the stack is the console.log from line 4, which executes with no delay. Then, the console.log from line 3 executes with a delay of one second.