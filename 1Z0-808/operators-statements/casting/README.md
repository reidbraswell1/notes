### Casting Primitive Values

```java
    float g = 123.456f;
    int h = (int) g;  // 123 is stored in h
    
    int i = (int) 789.988;  // 789 is stored in i;
    
    short x = 10;
    short y = 20;
    short z = (short) (x * y); // x and y are cast to int before multiplying hence the cast back to short before storing in z
```    
