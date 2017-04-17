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
         ```
          package example.final;
         ```
     * C#
       * Implementing namespaces in C#:
         ```
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
        ```
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
        ```
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
        ```
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
      
        ```
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
        ```
        //auto-implemented property
        public string Info {get; set;}  
        ```
        
  * Interfaces/ protocols
    * In object oriented programming you often will find yourself using interfaces. An interface is a reference type that is used in both Java and C#. It is a collection of abstract methods and one would use classes to implement the interface. An interface may also have constants, default methods, static methods, and nested types. C# and Java are almost identical in how they use interfaces, however, they do differ slightly in in the syntax in declaring the interface.
    <br /> Java Example:
      ```
      interface Example{
          void Method();
      }
      interface Sample extends Example{
          void SetText(String Text);
      }
      ```
      
      C# Example:
      ```
      interface Example{
          void Method();
      }
      interface Sample: Example{
          void SetText(String Text);
      }
      ```

  Inheritance/ extension
    * Both Java and C# use the concept inheritance. In object oriented programming inheritance is used to help save the developer time and help them avoid repeating code. It accomplishes this goal by creating a parent class that has multiple child classes. These child classes are able to overload methods from their parents class. An example in which inheritance would be useful would be if a developer were creating an eagle, a falcon, and a robin. If all three of these birds were of the same breed, all could fly the same, and all ate the same. Without inheritance you would have to copy the code for the three different birds for their abililites to fly breed and eat. However, with inheritance you could refer to the same block of code three times and avoid writing it out three times. In both Java and C# multiple inheritance is not supported.  
    <br />Both C# and Java use inheritance for this purpose, but again, the syntax is slightly different.
    
    <br />
    Java Example:
    ```
      class Super{
          void Method();
      }
      class Sample extends Super{
          void SetText(String Text);
      }
    ```
    C# Example:
    ```
    public class Example{
          void Method();
      }
      public class Sample: Example{
          void SetText(String Text);
      }
    ```
    
        
      
      
    
