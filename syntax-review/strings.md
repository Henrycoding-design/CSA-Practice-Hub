# Strings in AP Java Subset

Strings are **immutable** objects. Once created, they cannot be changed.

## Key Methods
- `int length()`: Returns the number of characters.
- `String substring(int from, int to)`: Returns characters from `from` (inclusive) to `to` (exclusive).
- `String substring(int from)`: Returns characters from `from` to the end.
- `int indexOf(String str)`: Returns the index of the first occurrence of `str`, or `-1` if not found.
- `boolean equals(String other)`: Compares content for equality.
- `int compareTo(String other)`: Returns 0 if equal, <0 if this comes before `other` alphabetically, >0 otherwise.

## Common Operations
### Concatenation
```java
String s = "Hello" + " " + "World";
```

### Equality
**ALWAYS** use `.equals()`:
```java
if (s1.equals(s2)) { ... }
```

## Traps
- **Immutable**: `s.toUpperCase()` does NOT change `s`. You must do `s = s.toUpperCase()`.
- **Out of Bounds**: `s.substring(0, 10)` will throw an exception if `s.length() < 10`.
