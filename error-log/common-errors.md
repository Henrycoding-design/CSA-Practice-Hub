# Common Errors & How to Fix Them

A quick reference for the most common mistakes in AP CSA code.

## 1. Off-By-One Errors
- **The Error**: `for (int i = 0; i <= arr.length; i++)`
- **The Fix**: Use `< arr.length` or `i <= arr.length - 1`.

## 2. NullPointerException
- **The Error**: Calling a method on a variable that hasn't been initialized.
- **The Fix**: Check if the variable is `null` before calling the method, or ensure it's initialized.

## 3. Comparison with `==` for Objects
- **The Error**: `if (list1 == list2)` or `if (str1 == str2)`.
- **The Fix**: Use `.equals()`.

## 4. Forgetting `return`
- **The Error**: Method is declared to return `int` but ends without a return statement.
- **The Fix**: Ensure all possible execution paths (including `else` blocks) return a value.

## 5. Scope Errors
- **The Error**: Trying to use a variable outside the block `{ }` where it was declared.
- **The Fix**: Declare the variable at a higher scope if it needs to be accessed later.
