1. 20
2. 20
3. We should not use var since it leads to naming conflicts and scoping issues
4. 20
5. It returns an error that says : "ReferenceError: result is not defined". This is because let is only visible in the if-block. It cannot be accessed on line 13, since it is out of scope. 
6. Nothing is printed, it gives error on line 8. It returns an error that says "TypeError: Assignment to constant variable." This occurred because result is a constant and we cannot reassign a constant value to some other number. 
7. For running line 13, I commented out line 8 since it gives an error so that I can see the result of line 13 after. This gives an error as well. "ReferenceError: result is not defined". This is because const is defined inside that code block only. 