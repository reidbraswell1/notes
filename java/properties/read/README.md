```java
import java.io.FileInputStream;
import java.io.IOException;
import java.io.InputStream;
import java.util.Properties
```
```java
  	Properties prop = new Properties();
	InputStream input = null;

	try {

		input = new FileInputStream("config.properties");

		// load a properties file
		prop.load(input);

		// get the property value and print it out
		System.out.println(prop.getProperty("property"));
    
	} catch (IOException ex) {
		ex.printStackTrace();
	} finally {
		if (input != null) {
			try {
				input.close();
			} catch (IOException e) {
				e.printStackTrace();
			}
		}
	}
```
Gets properties file from your project classpath root folder.
```java
   	Properties prop = new Properties();
    	InputStream input = null;
    	
    	try {
        
    		String filename = "config.properties";
    		input = YourClass.class.getClassLoader().getResourceAsStream(filename);
    		if(input==null){
    	            System.out.println("Unable to find " + filename);
    		    return;
    		}

    		//load a properties file from class path
    		prop.load(input);
 
                // get the property value
                System.out.println(prop.getProperty("property"));
 
    	} catch (IOException ex) {
    		ex.printStackTrace();
        } finally{
        	if(input!=null){
        		try {
				input.close();
			} catch (IOException e) {
				e.printStackTrace();
			}
        	}
        }
```
