# Arrays in AP Java Subset

Arrays are fixed-size collections of elements of the same type.

## Key Facts

- **Indexing**: Starts at `0`, ends at `length - 1`.
- **Initialization**:

  ```java
  int[] nums = new int[5]; // All elements initialized to 0
  String[] names = {"Alice", "Bob", "Charlie"};
  ```

- **Length**: Use `.length` (no parentheses).
- **Accessing**: `nums[0] = 10;`.

## Common Operations

### Traversal (Standard For Loop)

```java
for (int i = 0; i < arr.length; i++) {
    System.out.println(arr[i]);
}
```

### Enhanced For Loop (For-Each)

*Note: Use this when you only need to access elements, not modify them or use their index.*

```java
for (int num : nums) {
    System.out.println(num);
}
```

## Traps

- **ArrayIndexOutOfBoundsException**: Accessing `arr[arr.length]`.
- **Modification in For-Each**: You cannot change the elements of an array of primitives using a for-each loop.
