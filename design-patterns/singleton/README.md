### Singleton - Classic Not Thread Safe
```java
class Singleton 
{ 
	private static Singleton instance; 

	// private constructor
        // object can only be created by calling getInstance()
	private Singleton() {
        } 

	public static Singleton getInstance() 
	{ 
		if (instance==null) 
			instance = new Singleton(); 
		return instance; 
	} 
}
```
