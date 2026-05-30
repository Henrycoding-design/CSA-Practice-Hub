# ArrayLists in AP Java Subset

`ArrayList` is a dynamic array that can grow and shrink in size. It only stores **objects** (not primitives).

## Key Methods (AP Subset)

- `int size()`: Returns the number of elements.
- `boolean add(E obj)`: Appends `obj` to the end, returns `true`.
- `void add(int index, E obj)`: Inserts `obj` at `index`, shifting subsequent elements to the right.
- `E get(int index)`: Returns the element at `index`.
- `E set(int index, E obj)`: Replaces the element at `index` with `obj`, returns the **old** element.
- `E remove(int index)`: Removes and returns the element at `index`, shifting subsequent elements to the left.

## Initialization

```java
ArrayList<String> list = new ArrayList<String>();
```

## Autoboxing/Unboxing

Java automatically converts between primitives and their wrapper classes (e.g., `int` to `Integer`).

```java
ArrayList<Integer> nums = new ArrayList<Integer>();
nums.add(5); // Autoboxing: 5 becomes new Integer(5)
int x = nums.get(0); // Unboxing: Integer(5) becomes 5
```

## Traps

- **Index Shifting**: When you `remove(i)`, the element at `i+1` moves to `i`.
- **ConcurrentModificationException**: Don't `add` or `remove` while using a for-each loop.
