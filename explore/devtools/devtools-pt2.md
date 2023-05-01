## 1 

`result` is initialized by adding `num1` and `num2`. However, both `num1` and `num2` are strings when they were passed to the function `calculateSum`, so `result` become the concatenation of two strings instead of the result of adding two numbers. 

## 2

I will cast the result of `num1` and `num2` to numbers by using `Number()` before `calculateSum` is called. 