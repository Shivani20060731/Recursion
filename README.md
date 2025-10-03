# Recursion
Aim

To understand and implement various recursive functions in C++ to:

1. Reverse an integer.
2. Reverse a string.
3. Calculate the factorial of a number.
4. Calculate the sum of first `n` natural numbers.


Apparatus 
 C++ compiler


Theory

Recursion is a programming technique where a function calls itself to solve a smaller instance of the problem, with a **base condition** to stop the recursion.

Each recursive function must have:

1. Base Case – when the recursion should stop.
2. Recursive Case– the function calling itself with modified parameters to reach the base case.



Algorithm

 1. Reverse an Integer

Input: An integer `n`
Output**: Digits of `n` printed in reverse
Steps:

1. If `n == 0`, return.
2. Print `n % 10` (last digit).
3. Call the function recursively with `n / 10`.


 2. Reverse a String

Input: A string `str`
Output: Characters of `str` printed in reverse
Steps:

1. If `index < 0`, return.
2. Print `str[index]`.
3. Call the function recursively with `index - 1`.



3. **Factorial of a Number

**Input**: An integer `n`
**Output**: `n!` (factorial)
**Steps**:

1. If `n == 0 || n == 1`, return 1.
2. Else return `n * factorial(n - 1)`.

 4. Sum of First `n` Natural Numbers

**Input**: A positive integer `n`
**Output**: Sum of numbers from 1 to `n`
**Steps**:

1. If `n <= 1`, return `n`.
2. Else return `n + sumUp(n - 1)`.

Types of Recursion Used

| Program         | Type of Recursion | Description                                                  |
| --------------- | ----------------- | ------------------------------------------------------------ |
| Reverse Integer | Tail Recursion    | Function call is the last operation.                         |
| Reverse String  | Tail Recursion    | Function call is the last operation.                         |
| Factorial       | Head Recursion    | The multiplication happens after the recursive call returns. |
| Sum of Integers | Head Recursion    | Addition is done after recursive call returns.               |


Conclusion

Recursion is an effective way to solve problems by breaking them into smaller parts and solving each part with the same method. These programs demonstrate how recursive calls work with a base case to stop the process. They also show different types of recursion and how recursion can simplify complex tasks like reversing numbers, strings, and calculating factorials or sums. Overall, recursion is a useful and elegant programming technique.


