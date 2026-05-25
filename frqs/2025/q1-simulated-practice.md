# 2025 Simulated FRQ: Question 1 (Data Management)

*Note: This is a simulated practice problem for the 2025 prep cycle.*

## The Problem Statement
You are asked to implement a method `cleanData` that removes all null or empty strings from an `ArrayList<String>` and returns the count of elements removed.

## The Core Trick
**ArrayList Mutation during Traversal.** The key is handling the shifting indices when an element is removed. If you move forward and remove, you will skip the next element unless you adjust the index.

## Step-by-Step Logic Breakdown
1.  Initialize a `count` variable to 0.
2.  Loop through the `ArrayList` from index 0 to `size() - 1`.
3.  Check if the current element is `null` or has a `.length() == 0`.
4.  If it matches, remove the element, increment `count`, and **decrement the index `i`** to ensure the next element (which shifted down) is checked.
5.  Return the `count`.

## The Canonical Java Solution
```java
public int cleanData(ArrayList<String> data) {
    int count = 0;
    for (int i = 0; i < data.size(); i++) {
        if (data.get(i) == null || data.get(i).length() == 0) {
            data.remove(i);
            count++;
            i--; // The "Magic Fix" for shifting indices
        }
    }
    return count;
}
```

## Common Ways to Lose Points
- **Forgetting to decrement `i`**: This results in skipping the element immediately following a removed one.
- **Using `== ""` instead of `.equals("")` or `.length() == 0`**: Strings should not be compared with `==`.
- **NullPointerException**: Checking `.length()` before checking `== null`. (Always check `null` first!).
