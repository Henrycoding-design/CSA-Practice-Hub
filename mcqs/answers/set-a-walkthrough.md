# MCQ Explanations: Set A

## Answer Key

| Question | Answer | Unit |
|----------|--------|------|
| 1        | C      | Unit 1 |
| 2        | A      | Unit 1 |
| 3        | B      | Unit 1 |
| 4        | A      | Unit 1 |
| 5        | A      | Unit 1 |
| 6        | C      | Unit 1 |
| 7        | B      | Unit 1 |
| 8        | A      | Unit 1 |
| 9        | B      | Unit 2 |
| 10       | C      | Unit 2 |
| 11       | B      | Unit 2 |
| 12       | C      | Unit 2 |
| 13       | B      | Unit 2 |
| 14       | B      | Unit 2 |
| 15       | B      | Unit 2 |
| 16       | A      | Unit 2 |
| 17       | C      | Unit 1 |
| 18       | B      | Unit 3 |
| 19       | B      | Unit 3 |
| 20       | D      | Unit 1 |
| 21       | B      | Unit 3 |

---

## Question 1 Walkthrough

### Correct Answer: **C**

### Explanation
The code evaluates `(int) d / i`. Casting has higher precedence than division. `(int) 7.5` results in `7`. Then, `7 / 2` (integer division) results in `3`.

### Distractor Analysis
- **(A)**: Incorrectly assumes double division `7.5 / 2`.
- **(B)**: Incorrectly assumes the cast happens after the division `(int)(7.5 / 2)`.
- **(C)**: Correct.
- **(D)**: Incorrectly rounds up instead of truncating.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 2 Walkthrough

### Correct Answer: **A**

### Explanation
The expression is `15 % 4 + 7 / 2`.
1. `15 % 4` is the remainder of 15 divided by 4, which is `3`.
2. `7 / 2` is integer division, which is `3`.
3. `3 + 3 = 6`.

### Distractor Analysis
- **(A)**: Correct.
- **(B)**: Incorrectly assumes floating point division for `7 / 2`.
- **(C)**: Incorrectly calculates modulus or division.
- **(D)**: Incorrect calculation.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 3 Walkthrough

### Correct Answer: **B**

### Explanation
The expression `a / b` is evaluated first inside the parentheses. Since both `a` and `b` are integers (`10` and `4`), integer division occurs, resulting in `2`. This integer result is then cast to a `double`, resulting in `2.0`.

### Distractor Analysis
- **(A)**: Incorrectly assumes double division occurs before the cast.
- **(B)**: Correct.
- **(C)**: While the value is 2, the variable type is `double`, so it would be `2.0`.
- **(D)**: Incorrect calculation.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 4 Walkthrough

### Correct Answer: **A**

### Explanation
I. `int x = 5.0;` results in a compiler error because a `double` value cannot be assigned to an `int` variable without an explicit cast (narrowing conversion).

II. `double y = 5;` is valid (widening conversion).

III. `int z = (int) 5.5;` is valid due to the explicit cast.

### Distractor Analysis
- **(A)**: Correct.
- **(B)**: II is valid Java.
- **(C)**: III is valid Java.
- **(D)**: II is valid, only I is invalid.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 5 Walkthrough

### Correct Answer: **A**

### Explanation
`s.substring(3, 7)` returns a string starting at index 3 and ending at index 6 (7 is exclusive).
Indices: C(0) o(1) m(2) p(3) u(4) t(5) e(6) S(7) ...
Result: "pute".

### Distractor Analysis
- **(A)**: Correct.
- **(B)**: Includes index 7.
- **(C)**: Starts at index 2.
- **(D)**: Starts at index 4.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 6 Walkthrough

### Correct Answer: **C**

### Explanation
`"Mississippi".indexOf("ss", 3)` searches for "ss" starting from index 3.
M(0) i(1) s(2) s(3) i(4) s(5) s(6) ...
The first occurrence starting at or after index 3 begins at index 5.

### Distractor Analysis
- **(A)**: This is the first occurrence (at index 2), but the search starts at 3.
- **(B)**: There is no "ss" starting at index 3.
- **(C)**: Correct.
- **(D)**: Incorrectly assumes no other "ss" exists.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 7 Walkthrough

### Correct Answer: **B**

### Explanation
- `s1 == s2`: `s1` is a new object, `s2` is a literal. They point to different memory locations. Result: `false`.
- `s1.equals(s2)`: Compares content. Both are "Java". Result: `true`.
- `s2 == s3`: `s3` is assigned `s2`. They point to the same location. Result: `true`.
Output: `false true true`.

### Distractor Analysis
- **(A)**: Incorrectly assumes `==` compares content for `s1` and `s2`.
- **(B)**: Correct.
- **(C)**: Incorrectly assumes `equals` is false.
- **(D)**: Swaps the behavior of `==` and `equals`.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 8 Walkthrough

### Correct Answer: **A**

### Explanation
`a + b` results in string concatenation: `"123456"`. The length of this string is 6.

### Distractor Analysis
- **(A)**: Correct.
- **(B)**: Incorrectly counts length.
- **(C)**: Only counts length of one string.
- **(D)**: Incorrect calculation.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 9 Walkthrough

### Correct Answer: **B**

### Explanation
De Morgan's Laws state:
1. `!(A && B)` is equivalent to `!A || !B`
2. `!(A || B)` is equivalent to `!A && !B`

### Distractor Analysis
- **(A)**: This is equivalent to `!(a || b)`.
- **(B)**: Correct.
- **(C)**: Incorrect negation.
- **(D)**: Not equivalent.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 10 Walkthrough

### Correct Answer: **C**

### Explanation
Java evaluates boolean expressions from left to right. `x > 0` is `5 > 0`, which is `true`. Because of the `&&` operator, the second part `y / (x - 5) > 10` is evaluated. `x - 5` is `0`, leading to `10 / 0`, which throws an `ArithmeticException`.

### Distractor Analysis
- **(A)**: Would happen if the expression was true.
- **(B)**: Would happen if the first part was false (short-circuiting).
- **(C)**: Correct.
- **(D)**: The code is syntactically correct.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 11 Walkthrough

### Correct Answer: **B**

### Explanation
Java uses short-circuit evaluation. `x != 0` is `0 != 0`, which is `false`. Since the first part of the `&&` is `false`, the entire expression is `false`, and the second part (`10 / x > 1`) is never evaluated, avoiding a division by zero error. The `else` block executes, printing "False".

### Distractor Analysis
- **(A)**: Expression is false.
- **(B)**: Correct.
- **(C)**: Avoided due to short-circuiting.
- **(D)**: Syntax is correct.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 12 Walkthrough

### Correct Answer: **C**

### Explanation
- If `a=T, b=F`: `(T || T) && (F || F)` -> `T && F` -> `False`.
- If `a=T, b=T`: `(T || F) && (F || T)` -> `T && T` -> `True`.
- If `a=F, b=F`: `(F || T) && (T || F)` -> `T && T` -> `True`.

### Distractor Analysis
- **(A)**: Evaluates to true.
- **(B)**: Evaluates to true.
- **(C)**: Correct.
- **(D)**: It is not a tautology.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 13 Walkthrough

### Correct Answer: **B**

### Explanation
The loop starts at `i = 1`. Iterations:
1. `i = 1` (1 <= 10) - Print
2. `i = 3` (3 <= 10) - Print
3. `i = 5` (5 <= 10) - Print
4. `i = 7` (7 <= 10) - Print
5. `i = 9` (9 <= 10) - Print
6. `i = 11` (11 > 10) - Stop
Total prints: 5.

### Distractor Analysis
- **(A)**: Assumes `i++`.
- **(B)**: Correct.
- **(C)**: Off by one.
- **(D)**: Incorrectly rounds.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 14 Walkthrough

### Correct Answer: **B**

### Explanation
`k` values: 1, 2, 4, 8, 16, 32, 64, 128.
`count` increments at each step:
1. k=2, count=1
2. k=4, count=2
3. k=8, count=3
4. k=16, count=4
5. k=32, count=5
6. k=64, count=6
7. k=128, count=7
At k=128, `k < 100` is false.

### Distractor Analysis
- **(A)**: Stops too early.
- **(B)**: Correct.
- **(C)**: Iteration is logarithmic, not linear.
- **(D)**: Incorrect logic.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 15 Walkthrough

### Correct Answer: **B**

### Explanation
- `i = 0`: `j` runs from 0 to 2 (0, 1, 2) -> 3 increments.
- `i = 1`: `j` runs from 1 to 2 (1, 2) -> 2 increments.
- `i = 2`: `j` runs from 2 to 2 (2) -> 1 increment.
Total = 3 + 2 + 1 = 6.

### Distractor Analysis
- **(A)**: Assumes 3*3 iterations.
- **(B)**: Correct.
- **(C)**: Only counts outer loop.
- **(D)**: Incorrectly calculates inner loop.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 16 Walkthrough

### Correct Answer: **A**

### Explanation
In `for (int i = 0; i < 10; i--)`, `i` starts at 0 and decreases (-1, -2, -3...). The condition `i < 10` will always be true (until integer underflow, which still behaves as an infinite loop conceptually in CSA).

### Distractor Analysis
- **(A)**: Correct.
- **(B)**: Standard loop from 10 down to 1.
- **(C)**: Never executes.
- **(D)**: Standard loop from 0 to 9.

### AP CSA Unit
- **Unit 2**: Selection and Iteration

---

## Question 17 Walkthrough

### Correct Answer: **C**

### Explanation
The class `Point` has one constructor `Point(int xVal, int yVal)`. A valid instantiation must match this signature using the `new` keyword.

### Distractor Analysis
- **(A)**: No default (no-arg) constructor exists.
- **(B)**: No constructor with one `int` exists.
- **(C)**: Correct.
- **(D)**: Missing `new` keyword.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 18 Walkthrough

### Correct Answer: **B**

### Explanation
When a parameter name matches an instance variable name, the `this` keyword must be used to refer to the instance variable. `this.id = id;` assigns the parameter `id` to the instance variable `id`.

### Distractor Analysis
- **(A)**: Assigns the parameter to itself (no effect on instance variable).
- **(B)**: Correct.
- **(C)**: Assigns instance variable to parameter.
- **(D)**: Assigns instance variable to itself.

### AP CSA Unit
- **Unit 3**: Class Creation

---

## Question 19 Walkthrough

### Correct Answer: **B**

### Explanation
`score` is private, so it cannot be accessed directly via `p.score`. The client must use the public "getter" method `p.getScore()`.

### Distractor Analysis
- **(A)**: Private access error.
- **(B)**: Correct.
- **(C)**: Cannot access instance variable via class name.
- **(D)**: Cannot access instance method via class name.

### AP CSA Unit
- **Unit 3**: Class Creation

---

## Question 20 Walkthrough

### Correct Answer: **D**

### Explanation
Attempting to call a method (like `length()`) on a `null` object reference results in a `NullPointerException` at runtime.

### Distractor Analysis
- **(A)**: `null` does not have a length of 0.
- **(B)**: It doesn't print "null", it crashes.
- **(C)**: The syntax is valid, so it compiles.
- **(D)**: Correct.

### AP CSA Unit
- **Unit 1**: Using Objects and Methods

---

## Question 21 Walkthrough

### Correct Answer: **B**

### Explanation
Static methods belong to the class rather than any specific instance. They are called using the class name (e.g., `Math.abs(-5)`).

### Distractor Analysis
- **(A)**: Static methods cannot access instance variables directly.
- **(B)**: Correct.
- **(C)**: Static methods can be overloaded.
- **(D)**: They can be public or private.

### AP CSA Unit
- **Unit 3**: Class Creation
