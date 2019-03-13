### Strings

##### Concatenation rules using +

1. If both operands are numeric then numeric addition will occur.
1. If either operand is a string then concatenation will occur.
1. Evaluation occurs from left to right.

```java
    System.out.println(1 + 2); // 3 use first rule
    System.out.println("A" + "B"); // AB use second rule
    System.out.println(1 + 2 + "C"); // 3C use 3rd rule. 1 + 2 numeric add to 3 then evaluate "C" using rule 2 
```

##### Strings are immutable.
##### String Pool - (intern pool) - contains all literal values that appear in a program.
##### Important string methods:

1. length() - returns the length of a string  
**int length()**
```java
    String car = "toyota";
    System.out.println(car.length());  // 6
```    
2. charAt() - returns the character at index  
**char charAt(int index)**
```java
    String car = "volvo";
    System.out.println(car.charAt(1)); // o
```    
3. indexOf() - overloaded - returns the index of character or string  
**int indexOf(int ch)**
**int indexOf(char ch, int fromIndex)**
**int indexOf(String str)**
**int indexOf(String str, index fromIndex)**
```java
    String car = "honda";
    System.out.println(car.indexOf('n')); // 2
```    
4. substring() - overloaded
```java
    String car = "nissan";
    System.out.println(car.substring(1,4)); // iss 
```    
5. toLowerCase() toUpperCase()
6. equals() equalsIgnoreCase()
7. startsWith() endsWith()
1. contains()
1. replace()
1. trim()
