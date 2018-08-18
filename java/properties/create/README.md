```java
import java.io.FileOutputStream;
import java.io.IOException;
import java.io.OutputStream;
import java.util.Properties;
```
```java
Properties prop = new Properties();
OutputStream output = null;
	try {

		output = new FileOutputStream("config.properties");

		// set the properties value
		prop.setProperty("propertyName", "propertyValue");

		// save properties to project root folder
		prop.store(output, null);
	}
	catch(Exception exc) {
		exc.printStackTrace();
	}
	finally {
		if (output != null) {
			try {
				output.close();
			} catch (IOException e) {
				e.printStackTrace();
			}
	}
```
