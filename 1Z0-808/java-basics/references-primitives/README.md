### Java Primitive Types
---
| Keyword | Type                        | Example | Max Value - Min Value                    |
| :------ | :-------------------------- | :------ | :--------------------------------------- |
| boolean | true or false               | true    |                                          |
| byte    | 8-bit integral value        | 123     | Byte.MAX_VALUE, Byte.MIN_VALUE           |
| short   | 16-bit integral value       | 123     | Short.MAX_VALUE, Short.MIN_VALUE         |
| int     | 32-bit integral value       | 123     | Integer.MAX_VALUE, Integer.MIN_VALUE     |
| long    | 64-bit integral value       | 123     | Long.MAX_VALUE, Long.MIN_VALUE           |
| float   | 32-bit floating-point value | 123.45f | Float.MAX_VALUE, Float.MIN_VALUE         |
| double  | 64-bit floating-point value | 123.456 | Double.MAX_VALUE, Double.MIN_VALUE       |
| char    | 16-bit unicode value        | 'a'     | Character.MAX_VALUE, Character.MIN_VALUE |

##### Number System Constant Conversions
```java
// Base 10
System.out.println(56); // 56

// Binary
System.out.println(0b11); // 3
System.out.println(Integer.toBinaryString(56)); // 111000

// Octal
System.out.println(017); // 15 Octal
System.out.println(Integer.toOctalString(56)); // 70

// Hexadecimal
System.out.println(0x1F); // 31 Hexadecimal
System.out.println(Integer.toHexString(31)); // 1f
```

