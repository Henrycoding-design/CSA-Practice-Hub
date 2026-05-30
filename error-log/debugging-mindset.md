# Debugging Mindset

Don't panic when your code crashes. Errors are just clues.

## How to Read a Stack Trace

When Java throws an exception, it gives you a "Stack Trace."

```text
Exception in thread "main" java.lang.NullPointerException
    at MyClass.process(MyClass.java:15)
    at MyClass.main(MyClass.java:5)
```

1. **Look for the Exception Name**: `NullPointerException` means you tried to call a method on a variable that is `null`.
2. **Look for the Line Number**: `MyClass.java:15` tells you exactly where it happened.

## The Big Three Exceptions

1. **NullPointerException (NPE)**: You forgot to initialize an object or a method returned `null`.
2. **ArrayIndexOutOfBoundsException**: You tried to access `arr[arr.length]`. Remember, the last index is `length - 1`.
3. **ArithmeticException**: Usually `divide by zero`.

## Debugging Strategy

1. **Print Statements**: The "Poor Man's Debugger." Print your variables before the line that crashes.
2. **Rubber Ducking**: Explain your code line-by-line to an object (or a friend). You'll often find the mistake while explaining it.
3. **Simplify**: Comment out parts of your code until the error disappears, then add them back one by one.
