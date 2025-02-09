# OOPs and Java Interview Questions with Answers

## Java Questions

### 1. Which company owns Java now, and what is the latest version?
- Java is owned by **Oracle Corporation**.
- The latest version can be checked on [Oracle's official website](https://www.oracle.com/java/technologies/javase-downloads.html).

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

---

This file now contains **all Java and OOPs interview questions** extracted from the **Excel sheet**, along with concise answers. Let me know if you need any modifications! 🚀

