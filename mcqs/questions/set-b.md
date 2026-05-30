# MCQ Set: Set B (Advanced Topics)

## Instructions
- Time: 45 minutes
- Number of Questions: 21
- No calculators permitted.

---

## Question 1
Consider the following code segment:

```java
int[] nums = {1, 2, 3, 4, 5};
for (int i = 0; i <= nums.length; i++) {
    nums[i] = nums[i] * 2;
}
```

What is the result of executing this code segment?

(A) `nums` becomes `{2, 4, 6, 8, 10}`
(B) `nums` becomes `{1, 4, 9, 16, 25}`
(C) An `ArrayIndexOutOfBoundsException` is thrown
(D) A `NullPointerException` is thrown

---

## Question 2
Consider the following method, which is intended to return the maximum value in an array of integers.

```java
public int findMax(int[] arr) {
    int max = arr[0];
    for (int i = 1; i < arr.length; i++) {
        /* missing code */
    }
    return max;
}
```

Which of the following should replace `/* missing code */` so that the method works as intended?

(A) `if (arr[i] > max) max = i;`
(B) `if (arr[i] < max) max = arr[i];`
(C) `if (arr[i] > max) max = arr[i];`
(D) `if (max > arr[i]) max = arr[i];`

---

## Question 3
What will be stored in `arr` after the following code executes?

```java
int[] arr = {10, 20, 30, 40, 50};
for (int i = 0; i < arr.length / 2; i++) {
    int temp = arr[i];
    arr[i] = arr[arr.length - 1 - i];
    arr[arr.length - 1 - i] = temp;
}
```

(A) `{10, 20, 30, 40, 50}`
(B) `{50, 40, 30, 20, 10}`
(C) `{50, 40, 10, 20, 30}`
(D) `{10, 20, 30, 20, 10}`

---

## Question 4
Which of the following code segments correctly doubles every element in an array `int[] data`?

I.
```java
for (int x : data) {
    x = x * 2;
}
```

II.
```java
for (int i = 0; i < data.length; i++) {
    data[i] *= 2;
}
```

III.
```java
int i = 0;
while (i < data.length) {
    data[i] = data[i] * 2;
    i++;
}
```

(A) I only
(B) II only
(C) I and II only
(D) II and III only

---

## Question 5
Consider the following code segment:

```java
ArrayList<String> list = new ArrayList<String>();
list.add("apple");
list.add("banana");
list.add(1, "cherry");
list.remove(2);
list.add("date");
```

What are the contents of `list` after the code executes?

(A) `["apple", "cherry", "banana", "date"]`
(B) `["apple", "cherry", "date"]`
(C) `["cherry", "banana", "date"]`
(D) `["apple", "banana", "date"]`

---

## Question 6
Consider the following method which is intended to remove all occurrences of "bug" from an `ArrayList`:

```java
public void removeBugs(ArrayList<String> words) {
    for (int i = 0; i < words.size(); i++) {
        if (words.get(i).equals("bug")) {
            words.remove(i);
        }
    }
}
```

Which of the following describes the behavior of `removeBugs` when passed `["bug", "bug", "fly"]`?

(A) It correctly removes all "bug" strings, resulting in `["fly"]`.
(B) It results in `["bug", "fly"]` because it skips the second "bug".
(C) It throws an `IndexOutOfBoundsException`.
(D) It results in `["fly", "bug"]`.

---

## Question 7
Consider the following code segment:

```java
ArrayList<Integer> nums = new ArrayList<Integer>();
nums.add(5);
nums.add(10);
nums.add(15);
int x = nums.set(1, 20);
nums.add(x);
```

What is the content of `nums` after this code executes?

(A) `[5, 20, 15, 10]`
(B) `[5, 10, 15, 20]`
(C) `[5, 20, 15, 20]`
(D) `[5, 20, 10, 15]`

---

## Question 8
Which of the following is true about `ArrayList` vs `Array` in Java?

(A) `ArrayList` can store primitive types like `int` and `double` directly.
(B) `Array` size can be changed after initialization using the `resize()` method.
(C) `ArrayList` uses `size()` to get the number of elements, while `Array` uses a `length` field.
(D) Both `ArrayList` and `Array` support the `add()` method.

---

## Question 9
Consider the following 2D array:

```java
int[][] mat = {{1, 2, 3}, {4, 5, 6}};
```

What is the value of `mat[1][2]`?

(A) 2
(B) 3
(C) 5
(D) 6

---

## Question 10
Consider the following code segment which traverses a 2D array:

```java
int[][] grid = {{1, 2}, {3, 4}, {5, 6}};
int sum = 0;
for (int j = 0; j < grid[0].length; j++) {
    for (int i = 0; i < grid.length; i++) {
        sum += grid[i][j];
    }
}
```

What kind of traversal is this?

(A) Row-major order
(B) Column-major order
(C) Diagonal order
(D) Spiral order

---

## Question 11
What does the following code segment print?

```java
int[][] table = new int[3][4];
System.out.println(table.length + " " + table[0].length);
```

(A) `3 4`
(B) `4 3`
(C) `12 12`
(D) `3 3`

---

## Question 12
Consider the following method:

```java
public void mystery(int[][] arr) {
    for (int r = 0; r < arr.length; r++) {
        for (int c = 0; c < arr[0].length; c++) {
            if (r == c) {
                arr[r][c] = 0;
            }
        }
    }
}
```

If `arr` is `{{1, 2, 3}, {4, 5, 6}, {7, 8, 9}}`, what will it be after `mystery(arr)`?

(A) `{{0, 2, 3}, {4, 0, 6}, {7, 8, 0}}`
(B) `{{1, 0, 0}, {0, 5, 0}, {0, 0, 9}}`
(C) `{{0, 0, 0}, {4, 5, 6}, {7, 8, 9}}`
(D) `{{1, 2, 0}, {4, 0, 6}, {0, 8, 9}}`

---

## Question 13
Consider the following classes:

```java
public class Base {
    public Base() {
        System.out.print("Base ");
    }
}

public class Derived extends Base {
    public Derived() {
        System.out.print("Derived ");
    }
}
```

What is printed when `Derived d = new Derived();` is executed?

(A) `Derived`
(B) `Base`
(C) `Derived Base`
(D) `Base Derived`

---

## Question 14
Consider the following code segment:

```java
public class Animal {
    public void speak() { System.out.print("Animal "); }
}

public class Dog extends Animal {
    public void speak() { System.out.print("Woof "); }
}

// In some other class
Animal myPet = new Dog();
myPet.speak();
```

What is printed?

(A) `Animal`
(B) `Woof`
(C) `Animal Woof`
(D) `Woof Animal`

---

## Question 15
Which of the following is true about the `super` keyword?

I. It can be used to call a constructor of the parent class.
II. It can be used to call a private method of the parent class.
III. It can be used to call an overridden method of the parent class.

(A) I only
(B) II only
(C) I and III only
(D) II and III only

---

## Question 16
Consider the following code:

```java
public class Person {
    private String name;
    public Person(String n) { name = n; }
    public String getName() { return name; }
}

public class Student extends Person {
    private int id;
    public Student(String n, int i) {
        super(n);
        id = i;
    }
    public int getId() { return id; }
}

// In main
Person p = new Student("Alex", 123);
System.out.println(p.getName() + " " + p.getId());
```

What happens when the code is compiled and executed?

(A) Prints `Alex 123`
(B) Prints `Alex 0`
(C) A compiler error occurs because `Person` does not have an `getId` method.
(D) A runtime error occurs because `p` is not a `Student`.

---

## Question 17
Which of the following statements about polymorphism is FALSE?

(A) Polymorphism allows a subclass to provide a specific implementation of a method that is already defined in its superclass.
(B) At compile time, the compiler checks if the method exists in the declared type of the reference.
(C) At runtime, the Java Virtual Machine (JVM) determines which method to call based on the actual object type.
(D) A parent class reference can point to a child class object.

---

## Question 18
Consider the following recursive method:

```java
public int mystery(int n) {
    if (n <= 1) {
        return 1;
    } else {
        return n + mystery(n - 1);
    }
}
```

What is the result of `mystery(4)`?

(A) 4
(B) 7
(C) 10
(D) 24

---

## Question 19
Consider the following recursive method:

```java
public void trace(int n) {
    if (n > 0) {
        trace(n - 1);
        System.out.print(n + " ");
    }
}
```

What is printed by `trace(3)`?

(A) `3 2 1`
(B) `1 2 3`
(C) `3 2 1 0`
(D) `0 1 2 3`

---

## Question 20
What is returned by `recur("abc")`?

```java
public String recur(String s) {
    if (s.length() <= 1) {
        return s;
    }
    return recur(s.substring(1)) + s.charAt(0);
}
```

(A) `"abc"`
(B) `"cba"`
(C) `"acb"`
(D) `"aaa"`

---

## Question 21
What happens when `inf(5)` is called?

```java
public int inf(int n) {
    if (n == 0) {
        return 0;
    }
    return n + inf(n + 1);
}
```

(A) Returns 15
(B) Returns 0
(C) Results in a `StackOverflowError`
(D) Results in an `ArithmeticException`
