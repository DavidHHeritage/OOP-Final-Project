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
        ```
          
 
        
      
      
    
