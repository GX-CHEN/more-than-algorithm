## Java Fundamental Knowledge

- What is strongly typed?
    > A strongly typed language has stricter typing rules at compile time, which implies that errors and exceptions are more likely to happen during compilation.

- What is the advantage of strongly type? Disadvantage?
    > 1. Advantages: 
    >   1. Earlier detection of errors in compiling, speeds development 
    >   2. Type helps team members understand code easier 
    >   3. The posed type restriction can avoid code confusions (in JS, we can add string to number "2"+3=5, which could cause bugs)
    > 2. Disadvantage: Not much, if really want to have some disadvantage, since strongly typed need more code for specification, it might affect early stage of development speed, but in big project, strongly type will speed up development  

- What is difference between run-time error and compiling error. Example for each.
    > A run time error will only occur when the code is actually running. These are the most difficult, can be hard to track down.
    > 1. Example of compiling error (checked)
    >   1. Syntax Error (mismatch braces/brackets; missing semi-colon) 
    >   2. Type mismatch
    >   3. Missing Return Statement
    > 2. Example of run time error (unchecked)
    >   1. Incorrect comparison operators (e.g., not using double equal signs to indicate assignment)
    >   2. Referencing objects that don't exist, or don't exist using the capitalization supplied in the code
    >   3. Referencing an object that has no properties

- What is Data Abstract in Java, how can it be achieved?
    > Data abstraction is the process of hiding certain details and showing only essential information to the user. 
    > In Java, Abstraction can be achieved with either abstract classes or interfaces

- What is difference between interface and abstract class?
    > 1. Type of methods: Interface can have only abstract methods. Abstract class can have abstract and non-abstract methods. From Java 8, it can have default and static methods also.
    > 2. Final Variables: Variables declared in a Java interface are by default final. An abstract class may contain non-final variables.
    > 3. Type of variables: Abstract class can have final, non-final, static and non-static variables. Interface has only static and final variables.
    > 4. Implementation: Abstract class can provide the implementation of interface. Interface can’t provide the implementation of abstract class.
    > 5. Inheritance vs Abstraction: A Java interface can be implemented using keyword “implements” and abstract class can be extended using keyword “extends”.
    > 6. Multiple implementation: An interface can extend another Java interface only, an abstract class can extend another Java class and implement multiple Java interfaces.
    > 7. Accessibility of Data Members: Members of a Java interface are public by default. A Java abstract class can have class members like private, protected, etc.

- Which is better? Interface or subclassing?
    > (Arguably) Interface is generally considered to be better
    > 1. More flexible, since a class can extends only 1 class, but can implement multiple interfaces 
    > 2. Separate the implementation and abstraction

- Different between Array and ArrayList
    > 1. Implementation of array is simple fixed sized array but Implementation of ArrayList is dynamic sized array.
    > 2. Array can contain both primitives and objects but ArrayList can contain only object elements
    > 3. You can’t use generics along with array but ArrayList allows us to use generics to ensure type safety.
    > 4. You can use length variable to calculate length of an array but size() method to calculate size of ArrayList.
    > 5. Array use assignment operator to store elements but ArrayList use add() to insert elements.

- Priority Queue in Java (Very important for Heap data structure)
    > 1. A PriorityQueue is used when the objects are supposed to be processed based on the priority. It is known that a queue follows First-In-First-Out algorithm, but sometimes the elements of the queue are needed to be processed according to the priority, that’s when the PriorityQueue comes into play.
    > 2. Make sure to know the **Exact Syntax** of priority queue to implement Heap Data Structure 

- try/catch/finally
    > 1. The finally block always executes when the try block exits. This ensures that the finally block is executed even if an unexpected exception occurs
    > 2.  The finally block is a key tool for preventing resource leaks. When closing a file or otherwise recovering resources, place the code in a finally block to ensure that resource is always recovered.

- final keyword
    > In Java the final keyword is used in several contexts to **define an entity that can only be assigned once**, examples: 
    > 1，A final class cannot be subclassed. 
    > 2，A final method cannot be overridden or hidden by subclasses.
    > 3，A final variable can only be initialized once, either via an initializer or an assignment statement.

- Mutable/Immutable data structure

- What is serialization/de-serialization? What is Json?

- Java naming convention

- import static

- HasMap vs. TreeMap

- Java Enum (very important)

- List all the collection types you know

- Overriding vs Overloading

- Classic OOP concepts
    - Inheritance
    - Encapsulation
    - Polymorphism
    - Abstraction
    - Interface

- When to use public, when to use protected, when to use private?

- Boxing, unboxing, auto-unboxing

- default constructor

- What is extends, what is implement?

- What is the purpose of getter/setter? Why not just all use public?

- If we do not provide a constructor for Java class, what will happen?

- What is Singleton, and its use case

- How to manage memory in Java? What could cause memory leak?

- this() and super()
    > 1. super() as well as this() both are used to make constructor calls. 
    > 2. super() is used to call Base class’s constructor(i.e, Parent’s class) while this() is used to call current class’s constructor.

- How to clone an object and Java? Clone array, ArrayList, set etc.
    > You can manually create a new object and copy each field, but you can also use clone() method

- What is the default value of the local variables? 
    > 1. The local variables are not initialized to any default values. 
    > 2. We should not use local variables with out initialization.

- Is everything in Java an Object?
    > Every object is a java.lang.Object (NOTE:java.lang.Object has no super class.) 
    > However, there are many things which are not Objects.
     > 1. primitives and references. **You can ignore all the other things, and only remember primitive**
     > 2. fields (the fields themselves not the contents)
     > 3. local variables and parameters.
     > 4. generic classes (that may change in Java 8)
     > 5. methods (that will change in Java 8)
     > 6. blocks of code (that will change in Java 8)

- How many Primitive Types does Java have
    > 1. byte      1 byte
    > 2. short     2 bytes
    > 3. int       4 bytes
    > 4. long      8 bytes	
    > 5. float     4 bytes	
    > 6. double    8 bytes	
    > 7. boolean   1 bit
    > 8. char      2 bytes	

