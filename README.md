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
    ```java
        boolean myBoolean = false;
        Boolean myBoolean1 = true; // autoboxing primitive to wrapper type
        Boolean myBoolean2 = Boolean.valueOf(false); // boxing primitive to wrapper type
        Boolean myBoolean3 = Boolean.parseBoolean("true");
        Boolean myBoolean4 = null;

        char myChar = 'a';
        Character myCharacter1 = 'b'; // autoboxing primitive to wrapper type
        Character myCharacter2 = Character.valueOf('c'); // boxing primitive to wrapper type

        byte myByte = 10;
        Byte myByte1 = 20; // autoboxing primitive to wrapper type
        Byte myByte2 = Byte.valueOf((byte)30); // boxing primitive to wrapper type
        Byte myByte3 = Byte.parseByte("40");
        Byte myByte4 = null;

        short myShort = 10;
        Short myShort1 = 20; // autoboxing primitive to wrapper type
        Short myShort2 = Short.valueOf((short)30); // boxing primitive to wrapper type
        Short myShort3 = Short.parseShort("40");
        Short myShort4 = null;

        int myInt = 10;
        Integer myInteger = 20; // autoboxing primitive to wrapper type
        Integer myInteger2 = 30; // autoboxing primitive to wrapper type
        Integer myInteger3 = Integer.valueOf(30); // boxing primitive to wrapper type
        Integer myInteger4 = Integer.parseInt("40");
        Integer myInteger5 = null;
        // int myInt2 = null;

        long myLong = 10;
        Long myLong1 = 20L; // autoboxing primitive to wrapper type
        Long myLong2 = Long.valueOf(30L); // boxing primitive to wrapper type
        Long myLong3 = Long.parseLong("40");
        Long myLong4 = null;

        float myFloat = 10.0F;
        Float myFloat1 = 20.0F; // autoboxing primitive to wrapper type
        Float myFloat2 = Float.valueOf(30.0F); // boxing primitive to wrapper type
        Float myFloat3 = Float.parseFloat("40");
        Float myFloat4 = null;

        double myDouble = 10.0;
        Double myDouble1 = 20.0; // autoboxing primitive to wrapper type
        Double myDouble2 = Double.valueOf(30.0); // boxing primitive to wrapper type
        Double myDouble3 = Double.parseDouble("40.0");
        Double myDouble4 = null;
    ```
1.  Operators
    - Arithmetic Operators
    ```java
    int result = 3 - 2 + 2 * 2 + 3; // multiplication first
        // 3 - 2 + 4 + 3 // left to right
        // 1 + 4 + 3
        // 5 + 3
        // 8

        result = 4 / 2 + 1 - 4 * 2 + 10; // multiplication and division first
        // 2 + 1 - 8 + 10 // left to right
        // 3 - 8 + 10
        // -5 + 10
        // 5

        int a = 4;
        int b = 3 - 2 * --a; // decrement then use, a=a-1
        // 3 - 2 * 3
        // 3 - 6
        // b= -3 a=3

        a = 4;
        b = 3 - 2 * a--; // use a then decrement, a=a-1
        // 3 - 2 * 4
        // 3 - 8
        // b= -5 a=3 

        long c = 2;
        long d = 4 + 3 * c++; // use then increment, c=c+1
        // 4 + 3 * 2 // multiplication first
        // 4 + 6
        // d=10 c=3

        result = 10 - 3 * (2 + 1) - 4 / (1 + 3); // parenthesis first then multiplication and division
        // 10 - 3 * 3 - 4 / 4 // multiplication and division
        // 10 - 9 - 1 // left to right
        // 0

        int i = 10;
        int j = 3;

        // 10 % 3 = 10 / 3 = 3 -> 3 * 3 = 9 -> 10 - 9 = 1
        int k = i % j; // 1

        // 10%2 = 10/2=5 -> 2*5=10 -> 10-10=0
        int e = 10 % 2; // 0

        int f = 12;
        int g = 5;
        int h = 2;

        int m = f / 2 - 10 % (4 + 3) - 2 * f % g - h * 3; // parenthesis first
        // 12 / 2 - 10 % 7 - 2 * 12 % 5 - 2 * 3
        // 6 - 3 - 24 % 5 - 6
        // 6 - 3 - 4 - 6
        // 3 - 4 - 6
        // -1 - 6
        // -7
    ```
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
