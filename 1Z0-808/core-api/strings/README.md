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

1. length()
1. charAt()
1. indexOf()
1. substring()
1. toLowerCase() toUpperCase()
1. equals() equalsIgnoreCase()
1. startsWith() endsWith()
1. contains()
1. replace()
1. trim()
