# Recursion

Recursion is when a method solves a problem by calling itself on a smaller version of the same problem.

## Required Parts

- **Base case:** stops the recursion.
- **Recursive call:** moves toward the base case.
- **Combination step:** uses the recursive result if needed.

## Example

```java
public int sumTo(int n) {
    if (n == 1) {
        return 1;
    }
    return n + sumTo(n - 1);
}
```

## Trace

```text
sumTo(4)
4 + sumTo(3)
4 + 3 + sumTo(2)
4 + 3 + 2 + sumTo(1)
4 + 3 + 2 + 1
```

## AP CSA Traps

- Missing a base case.
- Recursive call does not move closer to the base case.
- Returning only the recursive call when the current value must be included.
- Using recursion when a loop would be clearer in an FRQ.
- Forgetting that each call has its own local variables.
