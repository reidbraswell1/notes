### Declare a Package & Import a Package

##### File written to disk looks like /home/a/A.java
```java
package a;
public class A {

}
```

##### File written to disk looks like /home/b/B.java
```java
package b;
import packagea.A;
public class B {

}
```

##### Wild card notation
```java
package b;
import packagea.*;
public class B {

}
```
```
