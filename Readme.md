# OOPs and Java Interview Questions with Answers

## Java Questions

### 1. Which company owns Java now, and what is the latest version?
- Java is owned by **Oracle Corporation**.
- The latest version of java is JDK 24 can be checked on [Oracle's official website](https://www.oracle.com/java/technologies/javase-downloads.html).

### 2. What are the 2 steps in Java compilation? Explain the 2 steps.
- **Compilation**: Java source code (`.java`) is compiled into bytecode (`.class`).
- **Execution**: JVM interprets bytecode and runs it on different platforms.

### 3. How does Java ensure portability?
- Java programs compile to **bytecode**, which runs on any JVM, making it platform-independent.

### 4. Explain JVM, JRE, JDK.
- **JVM (Java Virtual Machine)**: Runs Java bytecode.
- **JRE (Java Runtime Environment)**: Includes JVM + libraries.
- **JDK (Java Development Kit)**: Includes JRE + development tools (javac, debugger).

### 5. Explain the difference between Java compiler & Interpreter.
- **Compiler** (`javac`) converts Java source code to bytecode.
- **Interpreter** (JVM) executes bytecode line by line.

### 6. What is a class loader? What is its purpose?
- A **class loader** loads Java classes dynamically at runtime.
- Types: **Bootstrap, Extension, and Application class loaders**.

### 7. Explain each word `public static void main(String[] args)`.
- `public`: Accessible from anywhere.
- `static`: No need to create an object.
- `void`: Does not return a value.
- `main`: Entry point of Java programs.
- `String[] args`: Command-line arguments.

### 8. What is a wrapper class? What is auto boxing?
- **Wrapper class**: Converts primitives to objects (e.g., `Integer` for `int`).
- **Auto-boxing**: Automatic conversion of primitives to wrapper objects.

### 9. Explain the different access modifiers.
- **Private**: Accessible only within the same class.
- **Default**: Accessible within the same package.
- **Protected**: Accessible in the same package and subclasses.
- **Public**: Accessible everywhere.

### 10. What is the use of the `final` keyword?
- **final variable**: Cannot be changed.
- **final method**: Cannot be overridden.
- **final class**: Cannot be inherited.

### 11. What is method overloading and method overriding?
- **Overloading**: Same method name, different parameters (compile-time polymorphism).
- **Overriding**: Redefining a parent method in a child class (runtime polymorphism).

### 12. What is an abstract class?
- A class that **cannot** be instantiated but can have both abstract & concrete methods.
  ```java
  abstract class Animal { abstract void makeSound(); }
  ```

### 13. What is an interface? How is it different from an abstract class?
- **Interface**: A contract with abstract methods only (Java 8 allows default/static methods).
- **Difference**: Abstract classes allow instance variables & method implementations, interfaces do not.

### 14. What are checked and unchecked exceptions?
- **Checked Exceptions**: Must be handled during compilation (e.g., `IOException`).
- **Unchecked Exceptions**: Runtime exceptions (e.g., `NullPointerException`).

### 15. What is the difference between `==` and `.equals()` in Java?
- `==` compares memory addresses (reference comparison).
- `.equals()` compares the actual content (value comparison).

### 16. What is a singleton class?
- A class that allows only one instance.
  ```java
  class Singleton {
      private static Singleton instance;
      private Singleton() {}
      public static Singleton getInstance() {
          if (instance == null) instance = new Singleton();
          return instance;
      }
  }
  ```

### 17. What is garbage collection in Java?
- Automatic memory management where unused objects are deleted by the JVM.

### 18. What is the difference between an Array and an ArrayList?
- **Array**: Fixed size, can store both primitives & objects.
- **ArrayList**: Dynamic size, can only store objects.

### 19. What is the difference between HashMap and HashTable?
- **HashMap**: Not synchronized, allows `null` keys.
- **HashTable**: Synchronized, does not allow `null` keys.

### 20. What is a static block in Java?
- A block that runs once when the class is loaded.
  ```java
  static { System.out.println("Static Block Executed"); }
  ```

### 21. Can an abstract class contain non-abstract methods?
- Yes, an **abstract class** can have **both abstract and non-abstract methods**.

### 22. Can a normal class contain abstract methods?
- No, a **non-abstract (concrete) class** **cannot** have abstract methods.

### 23. Can an interface contain variables?
- Yes, but they are implicitly **public, static, and final**.

### 24. What is the default value of a reference variable in Java?
- The default value is **null**.

### 25. What is the difference between `this` and `super` keywords?
- `this` refers to the **current class instance**.
- `super` refers to the **parent class instance**.

### 26. What is the difference between `throw` and `throws`?
- `throw`: Used to **explicitly throw** an exception.
- `throws`: Declares exceptions that a method **may** throw.

### 27. Can we override the `main` method in Java?
- No, but we can **overload** it with different parameters.

### 28. Can a static method access instance variables?
- No, a **static method** cannot directly access **instance variables**.

### 29. What is the purpose of the `transient` keyword?
- **Marks a variable as non-serializable** (ignored during serialization).

### 30. Can we make the constructor `final` in Java?
- No, a **constructor cannot be final**.

### 31. What is the difference between `String`, `StringBuilder`, and `StringBuffer`?
- **String**: Immutable.
- **StringBuilder**: Mutable, not synchronized.
- **StringBuffer**: Mutable, synchronized.

### 32. What is method hiding in Java?
- When a **static method** in a subclass **redefines** a **static method** in its parent class.

### 33. Can we have multiple public classes in a Java file?
- No, **only one public class** per `.java` file.

### 34. What is a `volatile` variable in Java?
- A **volatile variable** ensures visibility of changes across **multiple threads**.

### 35. What is the difference between deep copy and shallow copy?
- **Shallow copy**: Copies references, not objects.
- **Deep copy**: Creates a new independent copy of objects.

---

