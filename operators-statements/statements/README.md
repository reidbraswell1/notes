### JAVA (Loop) Statements
1. [if-then](#if-then)
2. [if-then-else](#if-then-else)
3. [switch](#switch)
4. [while](#while)
5. [do-while](#do-while)
6. [for](#for)
7. [for-each](for-each/README.md)

<hr/>

#### <a name="if-then"></a>if-then

<hr/>

```java
if(booleanExpression) {
    // statements to execute if true
}
```
<hr/>

#### <a name="if-then-else"></a>if-then-else

<hr/>

```java
if(booleanExpression) {
    // statements to execute if true
} else {
    // statements to execute if false
}
```
<hr/>

#### <a name="switch"></a>switch

<hr/>

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

<hr/>

#### <a name="while"></a>while

<hr/>

```java
// while executes 0 or more times
// brackets required if multiple statements
// parenthesis required
while(booleanExpression) {
    // body
}
```

<hr/>

#### <a name="#while"></a>do-while

<hr/>

```java
// do-while executes at least 1 time
// brackets required if multiple statements
// parenthesis required
do {
    // body
} while (booleanExpression);
```
<hr/>

#### <a name="for"></a>for

<hr/>

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

// alternate 3
for(;;) {
    // endless loop
}
```
<hr/>

#### for-each

<hr/>

```java
for(datatype instance : collection) {
  // Body
}
```

[Back](../)

