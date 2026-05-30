# Index Errors

Index errors happen when code uses a position outside the valid range of an array, string, or `ArrayList`.

## Valid Ranges

- Array: `0` through `arr.length - 1`
- String: `0` through `str.length() - 1`
- `ArrayList`: `0` through `list.size() - 1`

## Common Causes

- Using `<=` instead of `<`.
- Starting at `1` instead of `0`.
- Removing from an `ArrayList` while moving forward.
- Calling `substring` with invalid bounds.
- Mixing row and column lengths in a 2D array.

## Fix Pattern

```java
for (int i = 0; i < values.length; i++) {
    System.out.println(values[i]);
}
```

## Debug Question

Ask: "What is the largest index this loop can produce, and is that index valid?"
