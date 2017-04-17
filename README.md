# final-project
4330 Final Project

Group Members: David Heritage<br />
Languages: Java & C#<br />

* Language purpose/genesis (Why was it created, what problem was it trying to solve?. is teh language a reaction to a previos language fr a replacement for another?)

  * Java
     * The Java programming language was originally designed by James Gosling and was created in hopes of creating a less implementation dependant language. This language was trying to create the "write once, run anywhere" method for developers. By this I mean, the code written would be able to be ran on any and all platforms that support Java without need of recompilation. Most Java applications are compiled using bytecode whcih can be ran on any Java virtual machine reguardless of the computers operating system and architecture. By creating this language Mr Gosling was able to create a independent platform programming language.

  * C#
    * The C# programming language was created by Microsoft and when they made it they had a small list of objectives for C#. These objectives that were accomplished can be interpretted as the languages purpose of creation. They claimed that C# was simple, modern, object-oriented, powerful/flexible, a language of few words, modular, and that it would be popular.
     
      * Why is it simple?
        * The syntax for C# is based off of the languages C and C++ so that the code can be easily understood for most begginer level programmers. To make the language even easier to use they altered some of the syntax. The language also tried to simplify concepts of object oriented languages by removing aspects such as macros, templates, multiple inheritance, and virtual base classes. 
       * Why is it modern?
         * This language is considered modern simply due to the fact that it is capable of using features such as exception handling, garbage collection, and extensible data types.
       * Why is it powerful/flexible?
         * When programming in C# there are no limitations to what you are capable of doing. The language can be used for things such as word processors, graphics, compilers for other languages, etc.
       * Why is C# a language of few words?
         * C# only has a small list of keywords. By having a small list of keywords the language is further simplified and easily understood.
       * Why is C# modular?
         * C# can be written in chunks of code named classes and the classes can conatian routines known as member methods. Using these classes and methods you are able to create useful, reusable code.
         
   * Unique Features
     * Java
       * Objects are the primary unit of composition.
         * In Java there are no standalone functions, and design patterns can be used to describe high level object coordination patterns.
       * Checked Exceptions.
         * By using exceptions, it will force the program to handle expected error conditions and resolve the problem if needed.
       * Unicode strings.
         * Many other programming languages use "byte strings" as their main string type. This can cause several issues when using international characters, however Java does not use the byte strings.
       * Compatibility focus.
         * Java is one language in which developers have worked on maintaining backwards compatibility with its libraries. It has libraries for almost everything including binary compatibility.
       * Garbage Collection.
         * This is a feature that most developers use to highlight Java. The garbage collection feature allows to developer to code and worry less about manual memory management.
     * C#
       * Assemblies
         * The assemblies feature is a type of encapsulation that is viewed as better than other languages when discussing modules or namesapces. They are similar to static or dynamic libraries you would find in C file in Java.
       * Cross-language compatibility is first-class
         * The C# language is run in the Common Language Runtime, which allows the langauge to support a variety of languages.
       * Properties are first-class
         * This feature makes it so that writing explicit getter and the optional setter methods is not neccessary.
       * Partial Classes
         * This feature allows a class's members to be defined in various files. This can be usefull in adding functionality to the classes that have been created.
       
   * Name spaces
   
     * How are they used?
         * Namespaces are used in both Java and C# are used for the same purpose, they are used to organize code into smaller groups in order to organize work as well as avoid naming errors. They can also be used to limit the scope of variables in a program. 
     * Java
       * Implementing namespaces in Java:
         ```Java
          package example.final;
         ```
     * C#
       * Implementing namespaces in C#:
         ```csharp
         namespace ExampleFinal{}
         ```
         
  * Types
    * Java vs C#
      * When it comes to types, Java and C# are actually very similar. The Java and C# programming languages are both capable of supporting both value and reference types. They are also capable of ceating new/custom data types. The two languages are very similar in the way that they are able to use types, however there are some monior differences between the two. For example in C#, all primitive data types are represented as objects rather than variables.Although they have subtle differences these two languages are very similar in the way that types are used. A list of supported types is shown below.
        1. primitive
          - example: int, short, double char, boolean etc.
        2. class
          - example: String, Integer, Boolean, ArrayList, etc.
        3. interface
          - Collection, Serialization, List, etc.
        4. array
          - int[], String[], etc.
          
          
  * Classes 
    * A class in object oriented programming is defined as an "extensible program-code-template for creating objects, providing intial values for state, and implementations of behavior". This statement simply means that a class is used as a blueprint for creating objects. Each class that is created is able to contain methods and or fields to describe the way that the objects will function.
    * Java
      * Defining a Class example:
        ```Java
        //Create class
        public class Cat{
        String name;
        
        //This is how you would create a constructor for the newly defined class.
        public Cat(String name){
            System.out.println("Name of cat is :" + name);
        } 
        
        void hungry(){}
        public static void main(String []args){
          
          //Object creation, name set.
          Cat myCat = new Cat("Tom");
          }
        }
        
        ```
        
    * C#
      * Defining a Class example:
        ```csharp
        //Create class
        public class Mouse{
            public String name;
            
            //Constructor
            public Mouse(String name){
                Console.WriteLine("Object being created.");
            }
            
            static void Main(string[] args){
            
            //new instance of object.
            Mouse mouse = new Mouse("Jerry");
            Console.WriteLine("Name of mouse is: {0}", mouse);
            }
        }
        //class destructor
        ~Mouse()
        ```
          
     * Instance reference name in data type
       * The "this" keyword is commonly used inside of a method or a constructor of a class as a reference to the object that is currently being invoked in a method or constructor. It is very helpful to use when you are working with variable hiding as well. For example, it is not possible to create two instance variables with the same name. A way to get around this is by using the this keyword. By using "this", we are able to use both a local variable and an instance variable of the same name. That is just one example in which you can use the this keyword in object oriented programming.
        <br/>example:
        ```Java
        class Example{
            int variable = 2;
            
            public static void main(String args[]){
                Example num = new Example();
                
                num.method(5);
                num.method();
            }
            void method(int variable){
                variable = 10;
                System.out.println("Value of Instance variable: " + this.variable)
                System.out.println("Value of variable : " + variable);
            }
        }
        
        /* OUTPUT:
        Value of Instance variable: 2
        Value of variable: 10
        */
        ```
        
       
         * Java and C#
          * There are several ways in which you can use the keyword "this" in C# as well as Java. Below is a list of some of the ways in which "this" can be used.
            1. To qualify members hidden by similar name.
            2. To have an object pass itself as a parameter to other methods.
            3. To have an object return itsefl from a method.
            4. To delcare indexers
            5. To declare extension methods
            6. To pass parameters between constructors.
            7. To internally reassign value type value.
            8. To invoke an extension method on the current instance.
            9. To cast itself to another type.
            10. TO chain constructors defined in the same class.
            
  * Properties
    * When it comes to properties, Java and C# vary in a few aspects. One of the largest differences between the two languages is the way that get/set concepts are used. As well as how backing variables are created and used.
    * Java
      * In Java the properties are not automatically generated, in order to use getters and setters you must create them as methods.If you wish to create computed properties you can simply add code to your getter or setter methods to do so.
      
        ```Java
        private String field;
        
        //get method
        public String getfield(){
          return this.field;
        }
        
        //set method
        public void setfield(String value){
        this.field = value;
        }
        ```
        
      
    * C#
      * In C# it is favorable to use auto properties as opposed to using set/get methods. This is due to the fact that the auto-implemented property takes up the least amount of space and if you wish to be more explicit and create a computed property with your delcaration you are capable of doing so. After the program is compiling a backing field will automatically be created.
        ```csharp
        //auto-implemented property
        public string Info {get; set;}  
        ```
        
  * Interfaces/ protocols
    * In object oriented programming you often will find yourself using interfaces. An interface is a reference type that is used in both Java and C#. It is a collection of abstract methods and one would use classes to implement the interface. An interface may also have constants, default methods, static methods, and nested types. C# and Java are almost identical in how they use interfaces, however, they do differ slightly in in the syntax in declaring the interface.
    <br /> Java Example:
      ```Java
      interface Example{
          void Method();
      }
      interface Sample extends Example{
          void SetText(String Text);
      }
      ```
      
      C# Example:
      ```csharp
      interface Example{
          void Method();
      }
      interface Sample: Example{
          void SetText(String Text);
      }
      ```

  * Inheritance/ extension
    * Both Java and C# use the concept inheritance. In object oriented programming inheritance is used to help save the developer time and help them avoid repeating code. It accomplishes this goal by creating a parent class that has multiple child classes. These child classes are able to overload methods from their parents class. An example in which inheritance would be useful would be if a developer were creating an eagle, a falcon, and a robin. If all three of these birds were of the same breed, all could fly the same, and all ate the same. Without inheritance you would have to copy the code for the three different birds for their abililites to fly breed and eat. However, with inheritance you could refer to the same block of code three times and avoid writing it out three times. In both Java and C# multiple inheritance is not supported.  
    <br />Both C# and Java use inheritance for this purpose, but again, the syntax is slightly different.
    
    <br />Java Example:
    ```Java
      class Super{
          void Method();
      }
      class Sample extends Super{
          void SetText(String Text);
      }
    ```
   <br /> C# Example:
    ```csharp
    public class Example{
          void Method();
      }
      public class Sample: Example{
          void SetText(String Text);
      }
    ```
    
    
  * Reflection
  
    * Reflection is the concept in object oriented programming that gives the program the ability to read its own data for the purpose fo finding assemblies, modules and type information at runtime. By using Reflection in both C# and in Java, you are able to discover the details of an object, method, as well as create objects or invoke methods at runtime. Generally this is why one would use the reflection function in Java or C#.
    
    
  * Memory Management
    * In the Java programming language all the objects that are created are stored in an area called the heap. The heap is a runtime data zone that allocates all class instances and arrays. This data area is created whenever the Java Virtual Machine is booted up. This memory source is dynamic in the sense, that the heap may increase or decrease in size as the application runs. If and when the heap becomes full, Java will take out the already used objects with the garbage collection feature that it has. The garbage collector looks for objects that are no longer being referenced, if one is found then it no longer obtainable by the application code and the garbage collector deletes it. In doing so it creates more space for the application to continue to run and create new objects.
    
    * Similarly, C# also uses this same methodology to manage its memory. It also creates a heap upon boot up and will store the created objects in a heap and store the information and it uses a pointer in order to keep track of its location for future use. When the application is finished using it, the objects are automatically freed from memory.
    
    https://www.google.com/webhp?sourceid=chrome-instant&rlz=1C1CHBF_enUS722US722&ion=1&espv=2&ie=UTF-8#q=how+is+memory+managed+in+Java
    
    
  *  Comparisons of references and Values
    * Often times in programming one might need to compare two values in order to test whether or not the are equivalent. In Java the two main ways of comparing data is by using both value comparisons and reference comparisons. When attempting to test whether two values/objects are equal one should use the == operator. If one is wanting to test whether or not overriden references are equal then they should use the equals() function.
    
    ```Java
    // In this situation we will use the == operator.
    
    int x, y;
    x = 10;
    y = 5
    if (x == y)
        System.out.println("The values of x and y are equal.");
    else
        System.out.println("The values of x and y are NOT equal.");
    
    
    /*OUTPUT: The values of x and y are NOT equal.*/
    ```
    ```Java
    String s1 = "test";
    String s2 = "test";
    String s3 = "test2";
    
    //test the equivalence of the objects s1 and s2
    System.out.println(s1.equals(s2));
    //test the equivalence of the objects s1 and s3
    System.out.println(s1.equals(s3));
    
    /*OUTPUT:
    true
    false*/
    ```
    
        
     * C# is very similar to that of Java when comparing values or references. By this I mean that C# also uses the == operator as well as the equals() function, the difference is that it also uses the ReferenceEquals() function. The ReferenceEquals function will test whether or not two objects are the same instance as well as if they can be overriden. An example is provied below.
     
     ```csharp
     object test1 = null;
     object test2 = new object();
     
     object.ReferenceEquals(test1, test1);
     object.ReferenceEquals(test1, test2);
     
     test1.Equals(test1);
     test1.Equals(test2);
     test2.Equals(test1);
     test2.Equals(test2);
     
     /*OUTPUT:
     true
     false
     NULL
     NULL
     false
     true*/
     ```
     
  * Null/nil references (EXAMPLE???)
    * In object oriented programming the null/nil keyword is used frequently. The languages Java and C# both use the keyword null as opposed ot the keyword nil. By definition, the null keyword is a literal that represents a null reference. To be a null reference means that the reference refers to an object that does not exist. By default, reference type varialbes are given the value null if one is not assigned to it.
    
      * In general, Java and C# are very similar when it comes to the usage of the keyword null. However, one of the changes that was made in C# 2.0 made it so that value types could be defined as null. In Java, this is not possible. 
      
    * Unfortunately, in both Java and C#, there is no set solution for handling null cases. More times than not, a null situation appears due to a logic error made by the programmer. Simply debuging the code is about the extent of how to handle these situations in both C# and Java. 
    
  *  Errors and exception handling
    * Both Error and Exception are subclasses in the the java.lang.Throwable class and they are both automatically created by the Java Virtual Machine. In Java, runtime errors are represented by the subclass Exception and an Error is thrown when a serious problem occurs during runtime that is not able to be fixed. Exceptions are typically followed by "catch", which is a way in which one can try to resolve an issue that was previously experienced. In both Java and C# exceptions are handled in try/catch blocks of code. The try keyword will execute a block of code and if an exception is needed to be used then the program will refer to the catch block of code to try and resolve the issue.
      * An example of exception and error handling is demonstrated below.
      
      ```Java
      try {
          file = new FileInputStream(fileName);
          x = (byte) file.read();
          }
      catch(IOException i){
      i.printStackTrace();
      return -1;
      }
      ```
      
      ```csharp
      try {
          object answer = processClass.InvokeMethod("Create", methodArgs);
      }
      catch(Exception e){
      if (ExceptionContainsErrorCode(e, 1))
      {
      return 1;
      }
      }
      ```
      
  * Lamda Expressions, closures, or functions as types
    * Java
      * Java represents lambda expressions as objects, and must be bound to a partibular functional interface.
      * A closure is a block of code that can be referenced with access to the variablesof the enclosing scope.
    * C#
      * A lambda expression is an anonymous function that you can use to create delegates(pointers) or expression tree types. USing these allows you to write local functions that can be passed as arguments or returned as the value of function calls. 
      * A closure in C# is an in-line delegae which is attached to its parent method. This allows the parents variables and methods to be referenced within the closure.
      ```csharp
      delegate int add(int a);
      static void Main(string[] args){
          add newDelegate = x => x * x;
          int b = newDelegate(2);
      }
      /*OUTPUT: 4*/
      ```
      
      ```csharp
      //example of closure in C#
      public Dog IdTage(int id){
          return this.Find(delegate(Dog a){
              return (a.Id == id);
          });
      }
      ```
