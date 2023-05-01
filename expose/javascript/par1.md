### 1

`values added: 20` is printed by line 9

### 2

`final result: 20` is printed by line 13

### 3

`values added: 20` is printed by line 9

### 4 

The code returns an reference error, because `result` is defined using `let` in the scope of `if`, but line 13 is outside the `if` scope, so `result` is not defined on line 13. 

### 5

The code returns an error. Declaring a variable with the `const` keyword prevents the variable from being reassigned. However, on line 7, it changes the content of `result`, so the error occur. 

### 6

The code returns an error. `result` was declared by `const` keyword, so when calling the function the error occured at line 7 where the code tries to assign an other value to `result`.
