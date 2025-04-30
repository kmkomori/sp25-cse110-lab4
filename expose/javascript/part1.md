Answers to CSE 110 Lab 4 Part 1

1. What is printed by line 9? If the code returns an error, explain why.

    Line 9 prints "values added:  20".

2. What is printed by line 13? If the code returns an error, explain why. 

    Line 13 prints "final result:  20".

3. Why should you not use var? Explain why. 

    We should not use var because it has no block scope. This can lead to conflicts and scoping issues in variables between different parts of code. It also has hoisting, which might result in unexpected behavior if the code isn't written in the order it is performed (i.e. the var is declared at the end of the function but is then hoisted to the top of the function).

4. What is printed by line 9? If the code returns an error, explain why.

    Line 9 prints "values added:  20".

5. What is printed by line 13? If the code returns an error, explain why. 

    Line 13 returns the error "ReferenceError: result is not defined". This error is returned because variable declaration using the keyword 'let' results in variables with block scoping. This means, the scope of the variable is only inside the block in which the variable is declared. In this specific function, result is declared in the 'if' block, and therefore cannot be accessed outside of the block (i.e. at the end of the program in the 'console.log()' call).

6. What is printed by line 9? If the code returns an error, explain why.

    Line 9 does not run as the program runs into an error in line 7 ("TypeError: Assignment to constant variable."). We get this error because we are trying to assign a new value to a const variable.

7. What is printed by line 13? If the code returns an error, explain why. 

    We run into the same issue as problem 6. Line 13 does not run as the program runs into an error at line 7 ("TypeError: Assignment to constant variable."). We get this error because we are trying to assign a new value to a const variable.