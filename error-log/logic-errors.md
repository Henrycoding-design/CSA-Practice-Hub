# Logic Errors

Logic errors happen when code runs but produces the wrong answer.

## Common Causes

- Correct syntax with the wrong condition.
- Updating the wrong variable.
- Returning too early.
- Forgetting to handle a boundary case.
- Accumulating a count, sum, or result in the wrong place.

## Example

```java
int count = 0;
for (int value : nums) {
    if (value > 0) {
        count = 1; // should usually be count++
    }
}
```

## Fix Pattern

1. Write the expected output for a tiny test case.
2. Trace each variable after every loop iteration.
3. Circle the first value that becomes wrong.
4. Fix the condition or update that caused the divergence.

## FRQ Habit

When a solution feels "almost right," trace it. Reading code silently is how logic bugs sneak past you wearing a tiny cape.
