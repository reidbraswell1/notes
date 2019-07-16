1. [Java Basics](java-basics/README.md)
1. [Operators & (Loop) Statements](operators-statements/README.md)
1. [Core API's](core-api/README.md)
1. [Methods & Encapsulation]()
1. [Class Design]()
1. [Exceptions]()
1. [Lambda's]()

<hr/>

1. Java Basics
    - Class Structure
    - Main Method
    ```java
    // Bracket may be after the String[] or after the variable args[]
    // Most widely used is String[]
    public static void main(String[] args) {
    }
    public static void main(String args[]) {
    }
    // Var args Representation
    public static void main(String... args) {
    }
    public static void main(String ...args) {
    }
    // Will compile but not run main method must be public
    private static void main(String[] args) {
    }
    ```
    - [Comments](java-basics/class-structure/comments/#for)
    - Static Imports
    ```java
    // Note the name of the field(Property) must come after the class or a * wildcard to import all fields
    import static java.lang.Math.PI;
    import static java.lang.Math.min;
    import static java.lang.System.out;
    import static java.lang.Byte.*; // Imports all fields in the Byte class
    ```
    - Decimal Numeric Primitives
    ```java
        float myNumber = 25.4F;
         
   //   double before = 10_.25; // does not compile
   //   double after = 10._25; // does not compile
   //   double first = _10.25; // does not compile
   //   double last = 10.25_; // does not compile

        double myDouble = 2.54;
        double myDouble2 = 2.54F;
        double anotherDouble = 2.45D; // d can be used for double it is optional

        double scientific = 5.000125E03;
        double scientific2 = 5.000125E3;
        double myDouble3 = 5000.125;

        double hexPi = 0x1.91eb851eb851fp1; // p indicates hexadecimal floating point number
    ```
    - Whole Numeric Primitives
    ```java
        byte myByte = 127;
        short myShort = 25; 
        
        long max = 32_123_456_789L;
        long n = 2_300;

        // octal (0-7)
        int oct = 07;
        int firstOct = 010; // 8 decimal
        int secondOct = 022; // 18 decimal
        
        // hexadecimal (0-9 and A-F)
        int firstHex = 0xF; // 15 decimal
        int secondHex = 0x1E; // 30 decimal
        
        // binary
        int firstBin = 0b1001; // 9 decimal
        int secondBin = 0b0111; // 7 decimal
        
        // int thirdBin = 0b2; // Won't compile
    ```
    - Primitive char and boolean
    ```java
        char ch = 'a';

        // char ch1 = 'ab'; // Won't compile
        char ch1 = '1';
        char ch2 = 49; // Ascii decimal for 1
        char uniChar = '\u03A9'; // upper case greek omega character
        char romanNumber = '\u216C'; // roman 50 number
        
        boolean myBoolean = true;
        boolean myFalseBoolean = false;
    ```
    - Declaring and initializing variables
    ```java
        // declaring and initializing in two lines
        int myNumber; // declaration
        // System.out.println("myNumber= " + myNumber);  // Won't compile myNumber may not have been declared
        myNumber = 10; // initialization
        
        // one line
        double myDouble = 7.50;

        // Have not been initialized yet
        float myFloat1, myFloat2, myFloat3;
        float myFloat4;
        float myFloat5;

        // Initializing myFloat6 myFloat7 but myFloat8 is not initialized only declared
        float myFloat6 = 5f, myFloat7 = 10f, myFloat8;
        
        // Declared but no value
        boolean b1, b2;

        // double d1, double d2; // does not compile
        double d1, d2; // does compile

        int i1;
        int i2;
        // int i3; i4; // does not compile
        int i3, i4; // does compile

        // int int = 10; // does not compile reserved word
        // cHaR and CHar are not reserved words so they are valid variables
        char cHaR;
        char Char;

        float okFloat;
        double $Ok2Double1;
        double _alsoDouble;
        float __OkButNotNice$_123;

        // illegal examples
        // double 3point; // may not begin with a number
        // double my@street; // no special characters @
        // float *$coffee; // no special characters * may begin with $ or _
        // float double; // double reserved word
        // double public; // public reserved modifier
    ```
    - Understanding Default Initialization of Primitives
    ```java
    static boolean myBoolean;  // false
    static byte myByte; // 0
    static short myShort; // 0
    static int myInt; // 0
    static long myLong; // 0
    static float myFloat; // 0.0
    static double myDouble; // 0.0
    static char myChar;  // 0 
    ```
    - Variable Scope
    - Ordering Elements In Class
    - Understanding Null
    - Primitive Wrapper Types
1.  Operators
    - Arithmetic Operators
    - Numeric Promotion and Casting
    - Unary Operators
    - Assignment Operators
    - Relational Operators
    - Conditional Operators
    - Equality Operators
    - Understanding == and equals() Method
    - Character Arithmetic
1. Basic Control Flow
    - [If Else](operators-statements/statements/)
    - [Ternary Operator](operators-statements/operators/)
    - [Switch Statement](operators-statements/statements/)
    - [While Loop](operators-statements/statements/)
    - [Do While Loop](operators-statements/statements/)
    - [For Loop](operators-statements/statements/)
1. Strings
    - String Creation and Concatenation
    - Immutability
    - String Pool and String Equality
    - String Methods
    - Method Chaining
    - StringBuilder
    - Understanding Equality
1. Arrays
    - Understanding and Using Arrays
    - For Each Loop
    - Break Statement and Labels
    - Continue Statement
    - Sorting Arrays
    - Searching Arrays
    - Variable Arguments
    - Multidimensional Arrays
    - Nested Loops
1. ArrayList
    - Understanding ArrayList
    - ArrayList Methods
    - Wrapper Classes With ArrayList
    - ArrayList And Array Conversion
    - ArrayList Sorting
    - ArrayList Searching
    - ArrayList Iterating
1. Methods
    - Designing Methods
    - Return Type
    - Parameter List
    - Variable Arguments
    - Static Methods And Fields
    - Using Static Methods And Fields
    - Final Variables
    - Static Initialization
    - Passing Data Between Methods
    - Returning Data From Methods
    - Overloading
    - Overriding
1. Class Design
    

[Back](../../tree/master)
