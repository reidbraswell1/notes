### Numeric Promotion

##### Numeric Promotion Rules
1. If 2 values have different data types one will be promoted to the larger of the two data types. 
```java
  int x = 1;
  long y = 10;
  
  long z = x * y; // x will be promoted to long before the multiplication
```
2. If 1 of the values is integer and the other is floating-point, the integer value will be promoted to the floating-point type.
```java
  int x = 1;
  float y = 12.5f;
  
  float z = x * y;  // x will be promoted to float before the multiplication
```  
3. Smaller data types: byte, short and char are promoted to int when they are used with a binary arithmetic operator.
```java
  byte x = 12;
  byte y = 15;
  
  int z = x + y;  // result is int as x and y are promoted to int
  ```
4. The resulting value will have the same data type as its promoted operands.
```java
  short x = 15;
  double y = 3;
  
  double z = x / y;  // x promoted to int then promoted to double
```  
