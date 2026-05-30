# MCQ Explanations: Set B (Advanced Topics)

## Answer Key

| Question | Answer | Topic |
|----------|--------|-------|
| 1        | C      | Unit 4 |
| 2        | C      | Unit 4 |
| 3        | B      | Unit 4 |
| 4        | D      | Unit 4 |
| 5        | B      | Unit 4 |
| 6        | B      | Unit 4 |
| 7        | A      | Unit 4 |
| 8        | C      | Unit 4 |
| 9        | D      | Unit 4 |
| 10       | B      | Unit 4 |
| 11       | A      | Unit 4 |
| 12       | A      | Unit 4 |
| 13       | D      | Unit 3 |
| 14       | B      | Unit 3 |
| 15       | C      | Unit 3 |
| 16       | C      | Unit 3 |
| 17       | E      | Unit 3 |
| 18       | C      | Unit 4 |
| 19       | B      | Unit 4 |
| 20       | B      | Unit 4 |
| 21       | C      | Unit 4 |

---

## Question 1 Walkthrough

### Correct Answer: **C**

### Explanation
The loop condition is `i <= nums.length`. In Java, array indices range from `0` to `length - 1`. When `i` reaches `nums.length` (which is 5 in this case), the access `nums[i]` attempts to access `nums[5]`, which is out of bounds.

### Distractor Analysis
- **(A)**: This would happen if the loop used `i < nums.length`.
- **(B)**: This would happen if the code squared the numbers instead of doubling them.
- **(D)**: Arrays are objects, but `nums` is initialized, so it's not null.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Array Traversal)

---

## Question 2 Walkthrough

### Correct Answer: **C**

### Explanation
To find the maximum, you should compare the current element `arr[i]` with the current `max`. If `arr[i]` is larger, update `max` to `arr[i]`.

### Distractor Analysis
- **(A)**: Updates `max` to the index `i` instead of the value `arr[i]`.
- **(B)**: This logic would find the minimum value.
- **(D)**: This logic would also find the minimum value.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Array Algorithms)

---

## Question 3 Walkthrough

### Correct Answer: **B**

### Explanation
This is a standard array reversal algorithm. It swaps the first and last elements, then the second and second-to-last, and so on, until it reaches the middle (`arr.length / 2`).

### Distractor Analysis
- **(A)**: This is the original array.
- **(C)**: Incorrect swap logic.
- **(D)**: This might happen if the swap logic was incomplete (e.g., overwriting without a temp variable).

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Array Algorithms)

---

## Question 4 Walkthrough

### Correct Answer: **D**

### Explanation
II and III use standard indexing to modify the array elements directly. I uses an enhanced for-loop. In Java, the enhanced for-loop variable `x` is a copy of the value in the array (for primitives); modifying `x` does not change the value stored in the array.

### Distractor Analysis
- **(A)**: I does not work for modifying primitive arrays.
- **(B)**: II is correct, but III is also correct.
- **(C)**: I is incorrect.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Enhanced for-loop vs standard loop)

---

## Question 5 Walkthrough

### Correct Answer: **B**

### Explanation
1. `add("apple")` -> `["apple"]`
2. `add("banana")` -> `["apple", "banana"]`
3. `add(1, "cherry")` -> `["apple", "cherry", "banana"]` (inserts at index 1, shifts "banana" right)
4. `remove(2)` -> `["apple", "cherry"]` (removes "banana" at index 2)
5. `add("date")` -> `["apple", "cherry", "date"]`

### Distractor Analysis
- **(A)**: Forgot to remove the element at index 2.
- **(C)**: Incorrect insertion or removal logic.
- **(D)**: Removed "cherry" instead of "banana".

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (ArrayList Methods)

---

## Question 6 Walkthrough

### Correct Answer: **B**

### Explanation
When `words.remove(i)` is called, the elements shift left. If there are two consecutive "bug" strings, the second "bug" shifts into index `i` while the loop increment `i++` moves to index `i+1`, skipping the second "bug".

### Distractor Analysis
- **(A)**: This would be correct if the loop decremented `i` after removal or iterated backwards.
- **(C)**: The loop condition `i < words.size()` prevents index out of bounds.
- **(D)**: Incorrect removal logic.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (ArrayList Traversal Pitfalls)

---

## Question 7 Walkthrough

### Correct Answer: **A**

### Explanation
1. `nums` starts as `[5, 10, 15]`.
2. `nums.set(1, 20)` replaces the element at index 1 (10) with 20. The method returns the old value: `x = 10`.
3. `nums` is now `[5, 20, 15]`.
4. `nums.add(x)` adds 10 to the end.
5. Final list: `[5, 20, 15, 10]`.

### Distractor Analysis
- **(B)**: Thinks `set` behaves like `add(index, element)`.
- **(C)**: Thinks `set` returns the new value (20).
- **(D)**: Incorrect placement of the added element.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (ArrayList set() and add())

---

## Question 8 Walkthrough

### Correct Answer: **C**

### Explanation
`ArrayList` uses the `size()` method to determine how many elements are currently in it. Arrays use the `length` property (field).

### Distractor Analysis
- **(A)**: `ArrayList` can only store Objects. Primitives are auto-boxed (e.g., `int` to `Integer`).
- **(B)**: Array sizes are fixed once initialized.
- **(D)**: Standard Arrays do not have an `add()` method.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (ArrayList vs Array)

---

## Question 9 Walkthrough

### Correct Answer: **D**

### Explanation
`mat[1]` refers to the second row `{4, 5, 6}`. `mat[1][2]` refers to the third element in that row, which is `6`.

### Distractor Analysis
- **(A)**: This is `mat[0][1]`.
- **(B)**: This is `mat[0][2]`.
- **(C)**: This is `mat[1][1]`.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (2D Array Indexing)

---

## Question 10 Walkthrough

### Correct Answer: **B**

### Explanation
The outer loop iterates through columns (`j`), and the inner loop iterates through rows (`i`). This means it finishes one column before moving to the next, which is column-major order.

### Distractor Analysis
- **(A)**: Row-major order iterates through rows in the outer loop and columns in the inner loop.
- **(C), (D)**: These are non-standard traversals.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (2D Array Traversal)

---

## Question 11 Walkthrough

### Correct Answer: **A**

### Explanation
`table.length` gives the number of rows (3). `table[0].length` gives the number of columns (4).

### Distractor Analysis
- **(B)**: Swapped rows and columns.
- **(C)**: This is the total number of elements.
- **(D)**: Only shows rows.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (2D Array Dimensions)

---

## Question 12 Walkthrough

### Correct Answer: **A**

### Explanation
The condition `if (r == c)` checks if the element is on the main diagonal (where row index equals column index). Elements `arr[0][0]`, `arr[1][1]`, and `arr[2][2]` are set to 0.

### Distractor Analysis
- **(B)**: This logic sets everything *except* the diagonal to 0.
- **(C)**: Sets the first row to 0.
- **(D)**: Sets the anti-diagonal to 0.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (2D Array Algorithms)

---

## Question 13 Walkthrough

### Correct Answer: **D**

### Explanation
When a subclass object is instantiated, the superclass constructor is called first (implicitly or explicitly via `super()`), followed by the subclass constructor.

### Distractor Analysis
- **(A)**: Ignores the implicit call to the parent constructor.
- **(B)**: Only calls the parent constructor.
- **(C)**: Swaps the order of execution.

### AP CSA Unit / Topic
- **Unit 3**: Class Creation (Inheritance Constructors)

---

## Question 14 Walkthrough

### Correct Answer: **B**

### Explanation
This is dynamic binding (polymorphism). Since the actual object is a `Dog`, the JVM calls the overridden `speak()` method in the `Dog` class, even though the reference type is `Animal`.

### Distractor Analysis
- **(A)**: This would happen if the method was not overridden or if it was static.
- **(B)**: Correct.
- **(C)**: Only one version of the method is executed.
- **(D)**: Incorrect order/logic.

### AP CSA Unit / Topic
- **Unit 3**: Class Creation (Polymorphism / Overriding)

---

## Question 15 Walkthrough

### Correct Answer: **C**

### Explanation
`super` is used to call parent constructors (I) and parent methods (III), especially when they are overridden. It cannot access `private` members of the parent class (II).

### Distractor Analysis
- **(A)**: III is also true.
- **(B)**: II is false because private members are not accessible even to subclasses.
- **(D)**: II is false.

### AP CSA Unit / Topic
- **Unit 3**: Class Creation (super Keyword)

---

## Question 16 Walkthrough

### Correct Answer: **C**

### Explanation
At compile time, Java checks the declared type of the reference. `p` is declared as a `Person`, and the `Person` class does not have an `getId()` method. This results in a compiler error.

### Distractor Analysis
- **(A)**: This would only happen if `p` was cast to `Student` or if the reference type was `Student`.
- **(B)**: Incorrect logic.
- **(D)**: This is a compile-time error, not a runtime error.

### AP CSA Unit / Topic
- **Unit 3**: Class Creation (Compile-time vs Runtime types)

---

## Question 17 Walkthrough

### Correct Answer: **E**

### Explanation
A child class reference *cannot* point to a parent class object without an explicit cast (and even then, it will throw a `ClassCastException` at runtime unless the object is actually an instance of the child class).

### Distractor Analysis
- **(A)**: This is the definition of overriding.
- **(B)**: Correct; this is how the compiler ensures type safety.
- **(C)**: Correct; this is dynamic binding.
- **(D)**: Correct; this is the basis for polymorphism.

### AP CSA Unit / Topic
- **Unit 3**: Class Creation (Inheritance Rules)

---

## Question 18 Walkthrough

### Correct Answer: **C**

### Explanation
Tracing `mystery(4)`:
- `mystery(4)` = 4 + `mystery(3)`
- `mystery(3)` = 3 + `mystery(2)`
- `mystery(2)` = 2 + `mystery(1)`
- `mystery(1)` = 1 (base case)
Sum: 4 + 3 + 2 + 1 = 10.

### Distractor Analysis
- **(A)**: Just the input value.
- **(B)**: Incorrect summation.
- **(D)**: This would be the result of a factorial (4 * 3 * 2 * 1).

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Recursion Tracing)

---

## Question 19 Walkthrough

### Correct Answer: **B**

### Explanation
This is a "head recursion" example. The print statement occurs *after* the recursive call.
1. `trace(3)` calls `trace(2)`
2. `trace(2)` calls `trace(1)`
3. `trace(1)` calls `trace(0)`
4. `trace(0)` returns (base case)
5. `trace(1)` prints "1 "
6. `trace(2)` prints "2 "
7. `trace(3)` prints "3 "
Output: `1 2 3 `

### Distractor Analysis
- **(A)**: This would happen if the print statement was *before* the recursive call (tail recursion).
- **(C)**: Includes the base case `0`, but `n > 0` prevents this.
- **(D)**: Includes the base case `0`.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Recursion Tracing)

---

## Question 20 Walkthrough

### Correct Answer: **B**

### Explanation
This method reverses the string.
- `recur("abc")` -> `recur("bc") + 'a'`
- `recur("bc")` -> `recur("c") + 'b'`
- `recur("c")` -> `"c"` (base case)
Combining: `"c" + "b" + "a"` = `"cba"`.

### Distractor Analysis
- **(A)**: The original string.
- **(B)**: Correct.
- **(C)**: Incorrect character positioning.
- **(D)**: Repeats characters.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (String Recursion)

---

## Question 21 Walkthrough

### Correct Answer: **C**

### Explanation
The recursive call `inf(n + 1)` increases `n` with every call. Since the base case is `n == 0`, and the initial value is `5`, the condition `n == 0` will never be met as `n` moves further away from 0. This leads to infinite recursion and a `StackOverflowError`.

### Distractor Analysis
- **(A)**: Assumes it sums 5+4+3+2+1, which is `inf(n - 1)`.
- **(B)**: Assumes it reaches the base case.
- **(D)**: No division by zero occurs.

### AP CSA Unit / Topic
- **Unit 4**: Data Collections (Recursive logic / Stack Overflow)
