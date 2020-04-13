# Week 1 - Java Topics
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

# Articles
## Java Basics
- [Data Structures and Algorithms in Java](https://www.javaworld.com/article/3527188/data-structures-and-algorithms-in-java-a-beginners-guide.html)
- [SOLID Java](https://filippobuletto.github.io/solid-java/#)
- [Java Versions and Features](https://www.marcobehler.com/guides/a-guide-to-java-versions-and-features)
- [Java Programming Cheatsheet](https://introcs.cs.princeton.edu/java/11cheatsheet/)

## The JVM
- [Structure of Java Virtual Machine](https://jakubstransky.com/2017/11/27/structure-of-java-virtual-machine-jvm/)
- [JVM Internals](https://blog.jamesdbloom.com/JVMInternals.html)
- [JVM Performance Optimization](https://www.javaworld.com/article/2078623/core-java-jvm-performance-optimization-part-1-a-jvm-technology-primer.html)
- [How the JVM Handles Exceptions](https://www.javaworld.com/article/2076868/how-the-java-virtual-machine-handles-exceptions.html)
- [How the JVM Performs Thread Synchronization](https://www.javaworld.com/article/2076971/how-the-java-virtual-machine-performs-thread-synchronization.html)

## Tools
- [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
- [A guide to Logging in Java](https://www.marcobehler.com/guides/a-guide-to-logging-in-java)
- [A Short Guide to Maven](https://www.marcobehler.com/guides/mvn-clean-install-a-short-guide-to-maven)

# Books
- [Think Java](https://books.trinket.io/thinkjava/index.html)
- [Wikibooks - Object Oriented Programming](https://en.wikibooks.org/wiki/Object_Oriented_Programming)
- [Wikibooks - Java Programming](https://en.wikibooks.org/wiki/Java_Programming)
- [Introduction to Programming Using Java, Eighth Edition](http://math.hws.edu/eck/cs124/javanotes8/)
- [Java Notes for Professionals](https://goalkicker.com/JavaBook/)
- [Open Data Sructures (in Java)](http://opendatastructures.org/ods-java/)
- [Inside the Java Virtual Machine](https://www.artima.com/insidejvm/ed2/)
- [Pro Git](https://git-scm.com/book/en/v2)
- [Maven by Example](https://books.sonatype.com/mvnex-book/reference/index.html)

# Documentation
## Java
- [Java Platform Standard Edition 8 Documentation](https://docs.oracle.com/javase/8/docs/index.html)
- [Java Platform Overview](https://docs.oracle.com/javase/8/docs/technotes/guides/index.html)
- [Enhancements in Java SE 8](https://docs.oracle.com/javase/8/docs/technotes/guides/language/enhancements.html)
- [Java Virtual Machine and Language Specifications](https://docs.oracle.com/javase/specs/index.html)
- [The java.lang.* and java.util.* Packages](https://docs.oracle.com/javase/8/docs/technotes/guides/lang/index.html)
- [The Collections Framework](https://docs.oracle.com/javase/8/docs/technotes/guides/collections/index.html)
- [Java I/O](https://docs.oracle.com/javase/8/docs/technotes/guides/io/index.html)
- [Java Generics](https://docs.oracle.com/javase/tutorial/extra/generics/)
- [Java Archive (JAR) Files](https://docs.oracle.com/javase/8/docs/technotes/guides/jar/index.html)
- [Java Networking](https://docs.oracle.com/javase/8/docs/technotes/guides/net/index.html)
- [OpenJDK 8 documentation](https://devdocs.io/openjdk~8/)
- [OpenJDK 8 Standard Library](https://hg.openjdk.java.net/jdk8/jdk8/jdk/file/687fd7c7986d/src/share/classes/java)

## Git
- [Git Documentation](https://git-scm.com/doc)
- [Git Configuration](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)

## Maven
- [Maven Users Centre](https://maven.apache.org/users/index.html#)

## JUnit
- [JUnit 5](https://junit.org/junit5/docs/current/user-guide/)

# Tools
- [Chocolatey](https://chocolatey.org/)
- [Homebrew](https://brew.sh/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Eclipse](https://www.eclipse.org/downloads/packages/)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/)
- [Git](https://git-scm.com/)
- [Maven](https://maven.apache.org/)
- [JUnit](https://junit.org/junit5/)

# Tutorials
## Java
- [Oracle Java Tutorials](https://docs.oracle.com/javase/tutorial/index.html)
- [Java SE 8 Programmer I Exam Prep](https://docs.oracle.com/javase/tutorial/extra/certification/javase-8-programmer1.html)
- [IBM Intro to Java Programming](https://developer.ibm.com/series/intro-to-java-programming/)
- [Learn X in Y - Java](https://learnxinyminutes.com/docs/java/)
- [Baeldung](https://www.baeldung.com/)
- [Jenkov](http://tutorials.jenkov.com/)
- [Tutorialspoint](https://www.tutorialspoint.com/java/index.htm)

## Design Patterns
- [Java Design Patterns](https://java-design-patterns.com/)
- [The Catalog of Design Patterns](https://refactoring.guru/design-patterns/catalog)

## Git
- [GitHub - Resources to learn Git](http://try.github.io/)
- [Visualizing Git](https://git-school.github.io/visualizing-git/)
- [Git](https://www.vogella.com/tutorials/Git/article.html)

## Maven
- [Maven Getting Started Guide](https://maven.apache.org/guides/getting-started/index.html)

## IDE
- [Writing Java with Visual Studio Code](https://code.visualstudio.com/docs/java/java-tutorial)
- [Using the Eclipse IDE for Java Programming](https://www.vogella.com/tutorials/Eclipse/article.html)
- [Maven for building Java applications](https://www.vogella.com/tutorials/ApacheMaven/article.html)
- [Using Maven within the Eclipse IDE](https://www.vogella.com/tutorials/EclipseMaven/article.html)
- [Eclipse Git Tutorial](https://www.vogella.com/tutorials/EclipseGit/article.html)
