# Java Fundementals

This topic is really important to know your langauge more and more let's dive in.

## What does “strong typed” mean?

Strong typed means that you need to identify each variable with it's own data type such you want to identfiy let's say a number you will type `int x = 10;` in this example as you see the data type is int and the value is a number but if you want to initialize a decmial number you have to do this `float x = 10.5f;` or `double x = 12.45d;` where the `float is 32 bit and the double is 64 bit`.

## What are the primitive data types?
`Boolean, byte, character, short, int, long, float, and double` are the eight primitive data types. These data types serve as the foundation for data manipulation in a programming language.


## Does code complining mean that it works correctly?

Not necessarily. compiling means that your code does not have any syntax error and follows the rules of your programming language. However code compliations does not gurantee for you that your code does not has any logic errors you may face run time errors this is why you need to debug your code.

## How many keywords does Java have?

| Keyword        | Description                                                                                    |
|----------------|------------------------------------------------------------------------------------------------|
| abstract       | Indicates the class or method that follows this keyword is abstract and must be implemented by a subclass.   |
| assert         | Assert keyword helps the programmer declare assertions or assumptions in a program. If false, an AssertionError is thrown at runtime.   |
| boolean        | Defines two values, true or false.                                                             |
| break          | Used to break out of loops or iterative constructs.                                            |
| byte           | Data type capable of holding 8-bit data.                                                        |
| case           | Marks blocks of text (cases) in a Switch statement.                                            |
| catch          | Used to catch exceptions generated in the try block.                                           |
| char           | Data type able to hold unsigned 16-bit Unicode characters.                                      |
| class          | Used to declare a new class.                                                                   |
| continue       | Helps take control outside the loop and continue to the next iteration.                          |
| default        | Defines the “block of code” that will execute by default in a Switch statement.                |
| do             | Starting keyword for “do-while” loop.                                                          |
| double         | Data type holding 64-bit numbers (floating-point).                                             |
| else           | Defines the else part in ‘if’ statements.                                                      |
| enum           | Used to declare enumerations in Java.                                                          |
| extends        | Indicates inheritance. A class is derived or inherited from another class.                      |
| final          | Defines a variable holding constant values or a method that cannot be overridden.               |
| finally        | Defines the finally block that executes after the try-catch block, irrespective of exceptions. |
| float          | Data type able to hold 32-bit floating-point values.                                           |
| for            | Indicates the start of a ‘for’ loop.                                                           |
| if             | Start of ‘if’ statement.                                                                       |
| implements     | Indicates that a class implements an interface.                                                |
| import         | Used to include or reference other packages/classes into the program.                           |
| instanceof     | Used to check if an object is an instance of another class.                                    |
| int            | Data type to hold a 32-bit integer value.                                                      |
| interface      | Used for declaring an interface.                                                               |
| long           | Data type holding 64-bit integer values.                                                        |
| native         | Used to indicate native code (platform-specific).                                              |
| new            | Operator to create a new object.                                                               |
| null           | Indicates null reference.                                                                      |
| package        | Keyword to declare a Java package.                                                             |
| private        | Indicates private access specified, accessible only by the declaring class.                    |
| protected      | Indicates protected access specifier, accessible within the class, subclass, and same package. |
| public         | Indicates public access specifier, accessible throughout the application.                      |
| return         | Used to send back the value of a method to the calling method and return control.              |
| short          | Data type holding 16-bit integer number values.                                                |
| static         | Indicates the method or a variable is static and cannot be instantiated.                       |
| strictfp       | Restricts the rounding and precision of floating point values calculation.                      |
| super          | Indicates base or superclass of the class.                                                     |
| switch         | Indicates a Switch statement that tests a condition and executes multiple cases.               |
| synchronized   | Indicates synchronized sections for multithreaded code, like critical sections.                |
| this           | Indicates the current object.                                                                  |
| throw          | Throws an exception.                                                                           |
| throws         | Indicates the exception that can be thrown by a method.                                        |
| transient      | Specifies a transient variable that is not part of the persistent state of an object.         |
| try            | Starts a block that contains code that might raise exceptions.                                 |
| void           | Indicates no return value.                                                                     |
| volatile       | Used to define variables that are not stored in Main Memory, allowing asynchronous changes.   |
| while          | Starts a while loop.                                                                           |
| const          | The ‘const’ keyword is no longer supported in Java.                                            |
| goto           | The ‘goto’ keyword is no longer supported in Java.                                             |
| true, false, and null | These words are literals and cannot be used as identifiers in the program.                  |


## How do you print words to the console in Java?

using the `System.out.println(Your variable);`
