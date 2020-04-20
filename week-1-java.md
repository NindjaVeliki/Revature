# Week 1 - Java 
## Concepts
- Environment: PATH, CLASSPATH, JAVA_HOME, command vs flags vs args
- Platform Independence: JVM
- Memory model: Stack, Heap, String Pool, Garbage Collection, Concurrency
- Compile time vs Runtime: Source code vs Bytecode
- Object Oriented Programming: Polymorphism, Encapsulation, Inheritance, and Abstraction
- Source Code Management: Gitflow
- Project, Dependency, Build Management
- Unit testing: Test Driven Development, Red-Green-Refactor

## Tools 
- JDK: `javac`, `java`, `jar`
- Git
  - Gitflow: init, add, commit
  - Branching & Merging: checkout, merge
  - Local & Remote Repositories: clone, remote, pull, push
  - Git vs GitHub
- Maven (`mvn`)
  - Project Object Model (POM) XML manifest file
  - Management: clean, archetype:generate, exec
  - Build Lifecycle: compile, test, package
- JUnit
  - Assert API
  - Annotations: @Test, @Before, @After

## Language Features
- Default Constructor
- Overloading and Overriding
- Checked vs Unchecked Exceptions
- Variable scopes: class/global, object/instance, method, block/loop, bracket
- Interfaces: functional vs marker, default fields & methods
- Abstract Classes
- Anonymous Classes
- Lambdas & Streams
- Generics: type inference, type erasure, bounded types

## Language Syntax
- Package & Import
- Class & method signatures: parameters, access modifiers, return types, constructors, varargs
- Access modfiers: public, protected, (default), private
- Non-access modifiers: static, final, abstract, synchronized
- Control statements: if, if else, else, while, do/while, for, switch, continue, break
- Primitive types: byte, short, int, long, char, boolean, float, double
- Reference types: Classes, Enums, Interfaces, Arrays
- Inheritance: extends, implements
- Exception handling: try, catch, finally

## Standard Library
- [java.lang](https://docs.oracle.com/javase/8/docs/api/java/lang/package-summary.html)
  - [Object](https://docs.oracle.com/javase/8/docs/api/java/lang/Object.html): `toString()`, `hashcode()`, `equals()`, `finalize()`, `notify()`
  - [String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html), [StringBuilder](https://docs.oracle.com/javase/8/docs/api/java/lang/StringBuilder.html) & [StringBuffer](https://docs.oracle.com/javase/8/docs/api/java/lang/StringBuffer.html)
  - Wrapper Classes: [Integer](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html), [Double](https://docs.oracle.com/javase/8/docs/api/java/lang/Double.html), etc.
  - [Iterable](https://docs.oracle.com/javase/8/docs/api/java/lang/Iterable.html): `forEach()`
  - [Comparable](https://docs.oracle.com/javase/8/docs/api/java/lang/Comparable.html): `compareTo()`
  - [AutoCloseable](https://docs.oracle.com/javase/8/docs/api/java/lang/AutoCloseable.html) (try-with-resources): close()
  - [System](https://docs.oracle.com/javase/8/docs/api/java/lang/System.html): `in`, `out`, `getenv()`, `gc()`
  - [Runnable](https://docs.oracle.com/javase/8/docs/api/java/lang/Runnable.html) & [Thread](https://docs.oracle.com/javase/8/docs/api/java/lang/Thread.html): `run()`, `start()`, `isAlive()`, `join()`
  - Reflection: [java.lang.reflect](https://docs.oracle.com/javase/8/docs/api/java/lang/reflect/package-summary.html), [Class](https://docs.oracle.com/javase/8/docs/api/java/lang/Class.html)
  - [Throwable](https://docs.oracle.com/javase/8/docs/api/java/lang/Throwable.html): [Error](https://docs.oracle.com/javase/8/docs/api/java/lang/Error.html), [Exception](https://docs.oracle.com/javase/8/docs/api/java/lang/Exception.html), [RuntimeException](https://docs.oracle.com/javase/8/docs/api/java/lang/RuntimeException.html)
- [java.io](https://docs.oracle.com/javase/8/docs/api/java/io/package-summary.html)
  - [File](https://docs.oracle.com/javase/8/docs/api/java/io/File.html)
  - InputStream/OutputStream vs Reader/Writer
  - [BufferedReader](https://docs.oracle.com/javase/8/docs/api/java/io/BufferedReader.html) & [BufferedWriter](https://docs.oracle.com/javase/8/docs/api/java/io/BufferedWriter.html)
  - [Serializable](https://docs.oracle.com/javase/8/docs/api/java/io/Serializable.html)
  - [ObjectInputStream](https://docs.oracle.com/javase/8/docs/api/java/io/ObjectInputStream.html) & [ObjectOutputStream](https://docs.oracle.com/javase/8/docs/api/java/io/ObjectOutputStream.html)
- [java.util](https://docs.oracle.com/javase/8/docs/api/java/util/package-summary.html)
  - [StringTokenizer](https://docs.oracle.com/javase/8/docs/api/java/util/StringTokenizer.html)
  - [Scanner](https://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html)
  - [Properties](https://docs.oracle.com/javase/8/docs/api/java/util/Properties.html)
  - [Java Collections Framework](https://docs.oracle.com/javase/8/docs/technotes/guides/collections/index.html):
    - [Arrays](https://docs.oracle.com/javase/8/docs/api/java/util/Arrays.html)
    - [Collections](https://docs.oracle.com/javase/8/docs/api/java/util/Collections.html)
    - [Collection](https://docs.oracle.com/javase/8/docs/api/java/util/Collection.html):
      - [Map](https://docs.oracle.com/javase/8/docs/api/java/util/Map.html): [Hashtable](https://docs.oracle.com/javase/8/docs/api/java/util/Hashtable.html), [HashMap](https://docs.oracle.com/javase/8/docs/api/java/util/HashMap.html), [TreeMap](https://docs.oracle.com/javase/8/docs/api/java/util/TreeMap.html)
      - [List](https://docs.oracle.com/javase/8/docs/api/java/util/List.html): [ArrayList](https://docs.oracle.com/javase/8/docs/api/java/util/ArrayList.html)
      - [Set](https://docs.oracle.com/javase/8/docs/api/java/util/Set.html)/[SortedSet](https://docs.oracle.com/javase/8/docs/api/java/util/SortedSet.html): [HashSet](https://docs.oracle.com/javase/8/docs/api/java/util/HashSet.html), [TreeSet](https://docs.oracle.com/javase/8/docs/api/java/util/TreeSet.html)
      - [Queue](https://docs.oracle.com/javase/8/docs/api/java/util/Queue.html)
      - [Deque](https://docs.oracle.com/javase/8/docs/api/java/util/Deque.html)
    - [Iterator](https://docs.oracle.com/javase/8/docs/api/java/util/Iterator.html)
    - [Comparator](https://docs.oracle.com/javase/8/docs/api/java/util/Comparator.html)

## Design patterns
  - Singleton
  - Factory
  - Dependency Injection
  - Data Access Object

