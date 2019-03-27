```java
import java.io.StringWriter;
import java.io.PrintWriter;

// ...

StringWriter sw = new StringWriter();
PrintWriter pw = new PrintWriter(sw); // Constructor for Writer sw extends Writer
e.printStackTrace(pw);
String sStackTrace = sw.toString(); // stack trace as a string
System.out.println(sStackTrace);
```
```java
StringWriter sw = new StringWriter();
e.printStackTrace(new PrintWriter(sw));
String exceptionAsString = sw.toString();
```
