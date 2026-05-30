# NullPointerException

`NullPointerException` happens when code tries to use an object reference that currently stores `null`.

## Common Causes

- Calling a method on `null`.
- Accessing an array or list element that was never initialized.
- Forgetting to construct an object with `new`.
- Returning `null` from a helper method and using the result immediately.

## Example

```java
String word = null;
int len = word.length(); // crash
```

## Fix Pattern

```java
if (word != null) {
    int len = word.length();
}
```

## FRQ Habit

Only add null checks when they match the prompt. AP CSA prompts often state that parameters are not `null`; unnecessary checks can distract from the required algorithm.
