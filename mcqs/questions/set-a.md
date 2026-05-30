# MCQ Set: Set A (AP CSA Practice)

## Instructions
- Time: 30 minutes
- Number of Questions: 21
- No calculators permitted.

---

## Question 1
What is the value of `x` after the following code execution?

```java
double d = 7.5;
int i = 2;
int x = (int) d / i;
```

(A) 3.75
(B) 3.5
(C) 3
(D) 4

---

## Question 2
What is the result of the following expression?

```java
15 % 4 + 7 / 2
```

(A) 6
(B) 6.5
(C) 7
(D) 5

---

## Question 3
Consider the following code segment:

```java
int a = 10;
int b = 4;
double result = (double) (a / b);
```

What is the value of `result`?

(A) 2.5
(B) 2.0
(C) 2
(D) 3.0

---

## Question 4
Which of the following will result in a compiler error?

I. `int x = 5.0;`
II. `double y = 5;`
III. `int z = (int) 5.5;`

(A) I only
(B) II only
(C) III only
(D) I and II

---

## Question 5
What does the following code print?

```java
String s = "ComputerScience";
System.out.println(s.substring(3, 7));
```

(A) "pute"
(B) "puter"
(C) "mput"
(D) "uter"

---

## Question 6
What is returned by the method call `"Mississippi".indexOf("ss", 3)`?

(A) 2
(B) 3
(C) 5
(D) -1

---

## Question 7
What is the output of the following code?

```java
String s1 = new String("Java");
String s2 = "Java";
String s3 = s2;
System.out.println((s1 == s2) + " " + s1.equals(s2) + " " + (s2 == s3));
```

(A) true true true
(B) false true true
(C) false false true
(D) true false true

---

## Question 8
What is the value of `val` after the following code segment?

```java
String a = "123";
String b = "456";
int val = (a + b).length();
```

(A) 6
(B) 7
(C) 3
(D) 9

---

## Question 9
According to De Morgan's Laws, which of the following is equivalent to `!(a && b)` where `a` and `b` are boolean variables?

(A) `!a && !b`
(B) `!a || !b`
(C) `a || b`
(D) `!(a || b)`

---

## Question 10
What is printed when the following code is executed?

```java
int x = 5;
int y = 10;
if (x > 0 && y / (x - 5) > 10) {
    System.out.println("A");
} else {
    System.out.println("B");
}
```

(A) A
(B) B
(C) Runtime error (ArithmeticException)
(D) Compiler error

---

## Question 11
What is printed when the following code is executed?

```java
int x = 0;
if (x != 0 && 10 / x > 1) {
    System.out.println("True");
} else {
    System.out.println("False");
}
```

(A) True
(B) False
(C) Runtime error
(D) Compiler error

---

## Question 12
For which values of `a` and `b` is the expression `(a || !b) && (!a || b)` false?

(A) a = true, b = true
(B) a = false, b = false
(C) a = true, b = false
(D) It is always true

---

## Question 13
How many times does "Hello" print?

```java
for (int i = 1; i <= 10; i += 2) {
    System.out.println("Hello");
}
```

(A) 10
(B) 5
(C) 4
(D) 6

---

## Question 14
What is the final value of `count` after the code segment?

```java
int count = 0;
int k = 1;
while (k < 100) {
    k *= 2;
    count++;
}
```

(A) 6
(B) 7
(C) 100
(D) 99

---

## Question 15
What is printed when the following code is executed?

```java
int sum = 0;
for (int i = 0; i < 3; i++) {
    for (int j = i; j < 3; j++) {
        sum++;
    }
}
System.out.println(sum);
```

(A) 9
(B) 6
(C) 3
(D) 4

---

## Question 16
Which code segment results in an infinite loop?

(A) `for (int i = 0; i < 10; i--)`
(B) `for (int i = 10; i > 0; i--)`
(C) `while (false) {}`
(D) `for (int i = 0; i < 10; i++)`

---

## Question 17
Consider the following class:

```java
public class Point {
    private int x, y;
    public Point(int xVal, int yVal) {
        x = xVal;
        y = yVal;
    }
}
```

Which of the following is a valid instantiation of a `Point` object in a client class?

(A) `Point p = new Point();`
(B) `Point p = new Point(5);`
(C) `Point p = new Point(5, 10);`
(D) `Point p = Point(5, 10);`

---

## Question 18
Which constructor implementation correctly initializes the instance variable `id` with the parameter `id`?

```java
public class Gadget {
    private int id;
    public Gadget(int id) {
        /* implementation */
    }
}
```

(A) `id = id;`
(B) `this.id = id;`
(C) `id = this.id;`
(D) `this.id = this.id;`

---

## Question 19
Given the following class, how should a client get the value of the private instance variable `score`?

```java
public class Player {
    private int score;
    public Player(int s) { score = s; }
    public int getScore() { return score; }
}
```

(Assume `p` is an initialized `Player` object)

(A) `int s = p.score;`
(B) `int s = p.getScore();`
(C) `int s = Player.score;`
(D) `int s = Player.getScore();`

---

## Question 20
What happens when the following code segment is executed?

```java
String s = null;
System.out.println(s.length());
```

(A) Prints 0
(B) Prints null
(C) Compiler error
(D) NullPointerException

---

## Question 21
Which of the following statements is true about `static` methods in Java?

(A) They can access all instance variables of the class.
(B) They are called using the class name, not necessarily an instance of the class.
(C) They cannot be overloaded within the same class.
(D) They must be declared with `private` access.
