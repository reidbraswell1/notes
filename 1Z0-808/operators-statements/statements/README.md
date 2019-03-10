### JAVA Statements

1. [if-then](if-then/README.md)
2. [if-then-else](if-then-else/README.md)
3. [switch](switch/README.md)
4. [while](while/README.md)
5. [do-while](do-while/README.md)
6. [for](for/README.md)
7. [for-each](for-each/README.md)

[Back](../)


#### switch
```java
switch(variableToTest) {
    case constantExpression1:
        // statements to execute
        break; // optional break
    case canstantExpression2:
        // statements to execute
        break; // optional break
    default: // optional may appear anywhere in switch statement
        // statements to execute
}
```

##### while
```java
// while executes 0 or more times
// brackets required if multiple statements
// parenthesis required
while(booleanExpression) {
    // body
}
```

##### do-while
```java
// do-while executes at least 1 time
// brackets required if multiple statements
// parenthesis required
do {
    // body
} while (booleanExpression);
```

##### for
```java
for(initialization; booleanExpression; updateStatement) {
    // body
}

// alternate 1
for(init1, init2, ... ,initN; booleanExpression; update1, update2, ... ,updateN) {
    // body
}

// alternate 2
for(;booleanExpression;) {
    // body
}   
```

##### for-each
```

