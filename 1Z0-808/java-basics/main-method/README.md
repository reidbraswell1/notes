### Various Methods of Writing the main method

1.
```java
public static void main(String[] args) {
    // Method Body
}
```
2. ##### Will Compile But Not Run (main method must be public to run)
```java
static void main(String[] args) {
    // Method Body
}
```

```java
public static final void main(String[] args) {
    // Method Body
}
```

```java
public static void main(String args[]){
    // Method Body
}
```


##### varargs
```java
public static void main(String ...args){
  // Method Body
}
```

