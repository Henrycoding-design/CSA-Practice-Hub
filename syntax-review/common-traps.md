# Common Syntax Traps

Focus on the mistakes that cost students points on the AP Exam.

## 1. Array vs. ArrayList Size
| Structure | Syntax | Common Mistake |
| :--- | :--- | :--- |
| **Array** | `arr.length` | `arr.length()` (Wrong!) |
| **String** | `str.length()` | `str.length` (Wrong!) |
| **ArrayList** | `list.size()` | `list.length` (Wrong!) |

## 2. The String Equality Trap
**The Mistake:**
```java
if (name == "Smith") { ... } // WRONG
```
**The "Why":** `==` compares memory addresses (references), not the content of the strings.
**The Fix:**
```java
if (name.equals("Smith")) { ... } // CORRECT
```

## 3. Integer Division
**The Mistake:**
```java
double average = (1 + 2) / 2; // average becomes 1.0, not 1.5
```
**The "Why":** `int / int` always results in an `int` (truncating the decimal).
**The Fix:**
```java
double average = (1 + 2) / 2.0; // CORRECT: average becomes 1.5
```

## 4. ArrayList Concurrent Modification
**The Mistake:** Removing elements in a for-each loop.
```java
for (String s : list) {
    if (s.isEmpty()) list.remove(s); // Will throw ConcurrentModificationException
}
```
**The Fix:** Use a standard for-loop with index adjustment or an `Iterator`.
