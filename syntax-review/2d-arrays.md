# 2D Arrays

A 2D array stores values in rows and columns.

## Access Pattern

```java
int[][] grid = new int[3][4];
grid[0][2] = 7;
```

The first index is the row. The second index is the column.

## Traversal

```java
for (int row = 0; row < grid.length; row++) {
    for (int col = 0; col < grid[0].length; col++) {
        System.out.println(grid[row][col]);
    }
}
```

## Enhanced For Loop

```java
for (int[] row : grid) {
    for (int value : row) {
        System.out.println(value);
    }
}
```

## AP CSA Traps

- Using `grid.length` for columns.
- Using `grid[0].length` for rows.
- Swapping row and column variables.
- Assuming every 2D array problem should use an enhanced `for` loop.
- Forgetting that position-based problems usually need index loops.
