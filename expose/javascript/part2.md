## 1 
Line 12 prints `3` to the console. This is because `var i` on line 6 in the for loop declared `i` with ` var`, making it a function-scoped variable. The parameter `prices` has 3 elements inside, so it has length 3, the for loop will end when `i = 3`, so on line 12, it will log `3` to the console. 

## 2 
Line 13 prints `150` to the console. This is because `var discountedPrice` declared on line 7 is a function-scoped variable. According to the pass-in parameters, `discount = 0.5`, `prices = [100, 200, 300]`, so since the `var discountedPrice` is declared in the for loop, its value on line 13 will be its value in the last iteration of the for loop. Thus, `discountedPrice = 300 * (1-0.5) = 150` is logged to the console at line 13. 

## 3
Line 14 prints `150` to the console. This is because `var finalPrice` declared on line 4 is also function-scoped. It is updated in the last iteration of the for loop where `discountedPrice = 150` as calculated in #2, so `finalPrice = 15000 / 100 = 150` is logged to the console at line 14. 

## 4 
This function will return `[50, 100, 150]`. For each element in the first parameter `prices`, the function `discountPrices` will calculate the `discountedPrice` and round it, make it have at most two decimals, to `finalPrice` which is pushed to the return array each time. Thus, the return array will be each price in the parameter, applying the passed-in discount. In this case, it becomes `[50, 100, 150]`. 

## 5 
The code causes an error, because `let i` declared in the for-loop is block-scoped, meaning that `i` is only defined inside the for-loop, so when accessing `i` on line 12, it is not defined and an error occur. 

## 6 
The code causes an error, because `let discountedPrice` declared inside the for-loop is block-scoped, meaning that `discountedPrice` is only defined inside the for-loop, so when trying to access it on line 13, `discountedPrice` is not defined, so an error occur. 

## 7 
Line 14 prints `150` to the console. This is because `let finalPrice` declared on line 4 is block-scoped, so it is defined in this `discountedPrices` function after the initialization. It is updated in the last iteration of the for loop where `discountedPrice = 150` as calculated in #2, so `finalPrice = 15000 / 100 = 150` is logged to the console at line 14. 

## 8 
This function will return `[50, 100, 150]`. For each price in `prices`, the function `discountPrices` will apply the `discount` to calculate the `discountedPrice` and round it, make it have at most two decimals, to `finalPrice` which is pushed to the return array each time. Thus, in this case, it becomes `[50, 100, 150]` from the `prices = [100, 200, 300]` and `discount = 0.5`.

## 9 
The code causes an error, because `let i` declared in the for-loop is block-scoped, meaning that `i` is only defined inside the for-loop, so when accessing `i` on line 11, it is not defined and an error occur. 

## 10 
Line 12 prints `3` to the console, because `const length` declared at line 4 is initialized to be the length of `prices`. In this case, `prices` has 3 elements, so `length = 3` is logged to the console at line 14. 

## 11 
This function will return `[50, 100, 150]`. For each price in `prices`, the function `discountPrices` will apply the `discount` to calculate the `discountedPrice` and pushed it to the return array. Although `const discounted` is declared at line 3, pushing `discountedPrice` to the array `discounted` does not reassign `discounted` to other things, so the error won't occur. Thus, in this case, it becomes `[50, 100, 150]` from the `prices = [100, 200, 300]` and `discount = 0.5`.

## 12 
### A 
`student.name`

### B 
`student["Grad Year"]`

### C
`student.greeting()`

### D
`student["Favorite Teacher"].name`

### E
`student.courseLoad[0]`


## 13
### A 
`'3' + 2 = '32'` since integers map to their exact string representation, `2` is converted to `'2'`

### B 
`'3' - 2 = 1` because `'3'` is converted to `3`

### C 
`3 + null = 3` since `null` maps to `0`, and `3 + 0 = 3`

### D
`'3' + null = '3null'` because `null` is converted to `'null'`

### E
`true + 3 = 4` since `true` maps to `1`, and `1 + 3 = 4`

### F
`false + null = 0` because both `false` and `null` are converted to `0`

### G
`'3' + undefined = '3undefined'` because `undefined` is converted to `'undefined'`

### H
`'3' - undefined = NaN` because `'3'` is converted to `3`, `undefined` is converted to `NaN`, so the result is `NaN`


## 14
### A 
`true`, string `'2'` becomes a number `2`, `2 > 1`

### B
`false`, lexicographically `'2' > '1'`, so `'2' > '12'`

### C 
`true`, `'2'` is converted to number `2`, 2 = 2

### D
`false`, because their types are different and `===` checks the equality without type conversion

### E
`false`, for boolean values, `true` becomes `1` instead of `2`

### F
`true`, `Boolean(2)` is `true` since `2` is a non-zero number, and `true === true`


## 15

`===` is a strict equality operator that checks the equality without type conversion. 
`==` is a non-strict check operator which will converts the values to numbers to compare values of different types. 

## 16
[part2-question16.js](part2-question16.js)

## 17

The result is `[2, 4, 6]`. `modifyArray([1,2,3], doSomething)` called `modifyArray` with parameters a array `[1,2,3]` and a function `doSomething` which will return its input times 2. In the function `modifyArray`, it creates a new array `newArr`, for each element in the input array, it calls the input function `doSomething`, adding the result to the `newArr`, and return `newArr` after the for-loop. Thus, every element in `newArr` is doubled than the corresponding element in the input array. 

## 18
[part2-question18.js](part2-question18.js)


## 19
The output is the following: 
```
1
4
3
2
```