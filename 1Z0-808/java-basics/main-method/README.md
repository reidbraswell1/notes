### Various Methods of Writing the main method

1. ##### Standard
```java
public static void main(String[] args) {
    // Method Body
}
```
2. ##### Alternate notation
```java
public static void main(String args[]){
    // Method Body
}
```
3. ##### Will Compile But Not Run (main method must be public to run)
```java
static void main(String[] args) {
    // Method Body
}
```
4. ##### Main method cannot be shadowed by a subclass
```java
public static final void main(String[] args) {
    // Method Body
}
```

5. ##### varargs
```java
public static void main(String ...args){
  // Method Body
}
```

