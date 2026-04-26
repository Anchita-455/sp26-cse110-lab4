1. The output is 3. This is because i is declared as a var, so it has global access, so it is accessible outside the for loop. The loop stops when i = 3 because the condition i < 3 becomes false, so the loop body is not executed for that value. The value 3 is only printed outside the for loop after it finishes. 
   
2. The output is 150. It just prints the discounted price for the last item in the prices array, which is 300 * 0.5 = 150. This is accessible from outside the for loop since discountedPrice is declared as a var. 
   
3. The output is 150. This just rounds the final price. This is accessible from outside the for loop since finalPrice is declared as a var.
    
4. This function just returns the discounted array. Nothing is printed since there is no "console.log". 
   
5. Gives error. "ReferenceError: i is not defined". This is because i is defined by "let" keyword here, so its scope is limited to the for-loop only, not outside of it.
   
6. Gives error. "ReferenceError: discountedPrice is not defined". This is because discountedPrice's scope is only within the for-loop. 
   
7. The result is 150 because finalPrice is updated during each iteration of the loop, and after the loop finishes it holds the last computed value. Since it’s defined outside the loop (but inside the function), it can be accessed and printed after the loop.
   
8. This function just returns the discounted array. Nothing is printed since there is no "console.log". 
   
9.  Gives error. "ReferenceError: i is not defined". This is because i is defined using let and it's scope is limited to the for-loop only. 
    
10. This outputs 3, since the length of the prices array is 3. It is a const, and it is declared within the function but outside the for-loop, so it is accessible after the for-loop. 
    
11. This function just returns the discounted array. Nothing is printed since there is no "console.log".
    
12. A. student.name <br>
    B. student["Grad Year"] <br>
    C. student.greeting() <br>
    D. student["Favorite Teacher"].name <br>
    E. student.courseLoad[0] <br>

13. A. "32" - this performs string concatenation so "3" is combined with "2" result is "32". <br>
    B.  1 - converts the 3 to a number and does regular subtraction and output is the number 1. <br>
    C. 3 - "null" is converted to 0 for arithmetic and it does 3 + 0 which is 3 and returns the result 3 thats a number. <br>
    D. "3null" - performs string concatenation, by adding string "null" to "3" <br>
    E. 4 - in numeric operations the boolean true is converted to the number 1, so 3 + 1 = 4, so the number 4 is returned <br>
    F. 0 - in numeric operations, null is converted to 0 and false is also converted to 0, so 0 + 0 = 0. The number 0 is returned. <br>
    G. "3undefined" - performs string concatenation, combines "3" with "undefined" <br>
    H. NaN - "undefined" is converted to NaN, and "3" is converted to 3, but 3 - NaN = NaN. <br>

14. A. true, the string 2 becomes the number 2, and 2 > 1, so returns true <br>
    B. false, since both are strings, this does lexicographical check, "2" > "12" lexicographically. <br>
    C. true, string 2 gets converted to number 2, and they're equal so returns true <br>
    D. false, checks both the value and the type, string and number are not equal, so returns false <br>
    E. false, true is converted to the number 1, and 1 != 2 <br>
    F. true, Boolean(2) is true since its non-zero, so both values and type match here and it returns true. <br>

15. "==" - regular equality check, this checks equality after performing type conversion if needed. <br>
    "===" - strict equality check, this checks the value and the type as well and if the types don't match, immediately returns false without type conversion. <br>

16. check part2-question16.js file

17. First, we call modifyArray with the array [1,2,3] and the function doSomething. Inside modifyArray, we loop through the array. For each element, we call the callback function, which is doSomething, and pass the current element. The doSomething function multiplies the value by 2 and returns the result back to modifyArray. This returned value is then pushed into a new array. After the loop finishes, the new array (with all elements multiplied by 2) is returned.

18. check part2-question18.js file

19. The output of the code is: <br>
    1 <br>
    4 <br>
    3 <br>
    2 <br>

    First, 1 is printed. The setTimeout calls are scheduled, but they don’t run yet.
    Then 4 is printed because JavaScript finishes all normal code first. After that, the timeout with 0ms runs, so 3 is printed. Finally, after 1 second, 2 is printed.