DevTools - Debugging (Questions + Answers)

---

Answer the following questions:

1. What was the bug?

    The inputs num1 and num2 were taken in as strings instead of numbers, so the "sum" operation (+) ended up just concatenating the two strings rather than adding the two numbers together.

2. How would you fix it?

    I wrapped num1 and num2 in the Number() function, to convert the strings to numbers before using the + operator. So rather than concatenating strings, the actual numbers get added instead.