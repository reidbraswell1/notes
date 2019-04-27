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
### Singleton - Classic Synchronized Thread Safe - may decrease performance
```java
class Singleton 
{ 
	private static Singleton instance; 

	// private constructor
        // object can only be created by calling getInstance()
	private Singleton() {
        } 

	public static synchronized Singleton getInstance() 
	{ 
		if (instance==null) 
                    instance = new Singleton(); 
		return instance; 
	} 
}
```
### Singleton - Classic Eager Initialization - created when class is loaded
```java
class Singleton 
{ 
	private static Singleton instance = new Singleton(); 

	// private constructor
        // object can only be created by calling getInstance()
	private Singleton() {
        } 

	public static Singleton getInstance() 
	{
		return instance; 
	} 
}
```
### Singleton - Double Checked Locking
```java
class Singleton 
{ 
        // write variable to main memory not to CPU cache
	private static volatile Singleton instance; 

	// private constructor
        // object can only be created by calling getInstance()
	private Singleton() {
        } 

	public static Singleton getInstance() 
	{
		if (instance==null)
		{
		    // thread safety
		    synchronized(Singleton.class) 
		    {
		    	// double check
		    	if (instance==null)
                            instance = new Singleton();
                    }
		}
	        return instance;
	} 
}
```
[Back](../../../../tree/java/)
