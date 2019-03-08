### Java Fields

##### Instance variables
```java
class FieldsExamples {

      private int i;  // Initialized to 0
      private long l; // Initialized to 0
      private String s; // Initialized to null
      
      // Instance Initializer Block
      {
            i=1;
            l=2;
            s="Hello World";
      }
}
```

### Java Methods
```java
class MethodsExamples {

      private int i;
      private int j;
      
      // Public Access
      public int getI() {
            return i; // Or return this.i
      }
      
      // Default Package Access
      int getJ() {
            return j; // Or return this.j
      }
      
      // Public Access
      public void setI(int value) {
            i=value; // Or this.i=value;
      }
      
      // Default Package Access
      void setJ(int value) {
            j=value; // Or this.j=value;
      }
```
