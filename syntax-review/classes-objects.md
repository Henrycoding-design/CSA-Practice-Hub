# Classes and Objects

Classes define types. Objects are individual instances of those types.

## Class Anatomy

```java
public class ScoreCard {
    private String name;
    private int score;

    public ScoreCard(String studentName) {
        name = studentName;
        score = 0;
    }

    public void addPoints(int points) {
        score += points;
    }

    public int getScore() {
        return score;
    }
}
```

## Instance vs Local Variables

- Instance variables belong to the object and persist between method calls.
- Local variables exist only inside the method or block where they are declared.
- Constructors initialize new objects.
- Accessor methods return information.
- Mutator methods change object state.

## AP CSA Traps

- Shadowing an instance variable with a constructor parameter and forgetting assignment.
- Returning a local variable when the field should be returned.
- Making fields public instead of private.
- Forgetting `new` when constructing an object.
- Calling an instance method without an object reference.
