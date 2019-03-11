### Numeric Promotion

##### Numeric Promotion Rules
1. If 2 values have different data types one will be promoted to the larger of the two data types. 
```java
  int x = 1;
  long y = 10;
  
  long = x * y; // x will be promoted to long before the multiplication
```
2. If 1 of the values is integer and the other is floating-point, the integer value will be promoted to the floating-point type.
