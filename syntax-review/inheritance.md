# Inheritance

Inheritance lets one class reuse and specialize another class.

## Core Vocabulary

- **Superclass:** the parent class.
- **Subclass:** the child class that extends the superclass.
- **Override:** a subclass method with the same signature as a superclass method.
- **Polymorphism:** a superclass reference can refer to a subclass object.

## Pattern

```java
public class Dog extends Pet {
    public Dog(String name) {
        super(name);
    }

    public String speak() {
        return "woof";
    }
}
```

## AP CSA Traps

- Constructors are not inherited.
- `super(...)` must be the first statement in a subclass constructor.
- Private superclass fields cannot be accessed directly by subclasses.
- Method overriding requires the same method signature.
- The declared reference type controls what methods can be called at compile time.

## Quick Check

If `Pet p = new Dog("Miso");`, Java chooses overridden methods using the actual object type at runtime, but it only allows method calls that exist in the `Pet` type at compile time.
