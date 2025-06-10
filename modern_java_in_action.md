# Modern Java in Action — Chapter 1

## 1. Why Did Java Need to Change?

- Java had to keep up with faster computers and better programming needs.
- Multi-core CPUs mean programs can do many things at once.
- Developers want clearer and simpler code.
- Modern problems require new tools.

## 2. Big New Features in Java 8+

- **Lambda Expressions:** Small anonymous functions.
- **Streams API:** Work on data collections like a conveyor belt.
- **Optional:** Safe way to avoid null errors.
- **Default Methods:** Interfaces can have actual methods.
- **Modules (Java 9):** Organize code like boxes.
- **Type Inference (Java 10):** Use `var` instead of full types.
- **New HTTP Client (Java 11):** Easier web calls.

## 3. Simple Example: Print names starting with “A”

**Old way:**

```java
List<String> names = Arrays.asList("Alice", "Bob", "Anna", "Mike");
for (String name : names) {
    if (name.startsWith("A")) {
        System.out.println(name);
    }
}
```

New way with streams and lambda:

```java
names.stream()
     .filter(name -> name.startsWith("A"))
     .forEach(System.out::println);
```
## Summary
- Java 8+ helps write clean, concise code.
- Lambdas and streams make working with lists easier.
- Optional helps avoid null-related bugs.
- Newer Java versions add modularity and easier coding.
