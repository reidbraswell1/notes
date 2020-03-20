# Creating a Spring Boot Project with vscode.

### Add the following extensions to vscode
1. Spring Boot Extension Pack
1. Spring Initializr Java Support (Similar to Spring Boot Extension Pack)
1. Spring Boot Tools
1. Thymeleaf

### Creating the application
1. Open the command palette (Ctrl + Shift + P) and Type Spring Initializr to start generating a Maven or Gradle project.
1. Choose __Maven__ or Gradle.
1. Choose Project Language (Java)
1. Enter a Group Id  ie. __com.helloworld__
1. Enter artifact ie. __demo__
1. Specify Spring Boot Version
1. Specify Dependencies
1. Choose your project folder
1. In the POM.xml file you should see your dependencies.
1. The main method in the application is the starting point for your application.
1. You will need a controller for your appliaction ie.
```java
package com.helloworld.demo;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RequestMethod;
import org.springframework.web.bind.annotation.ResponseBody;

@Controller
public class HelloWorldController {

    @RequestMapping(value = "/", method = RequestMethod.GET)
    @ResponseBody
    public String helloworld() {
        return "<h1>Hello Spring World</h1>";
    }
}
```
1. Run the application (F5).

### Additional Documentation and Examples:
1. [External Website Documentation](https://medium.com/programming-is-hard/creating-a-hello-world-spring-boot-app-using-vs-code-f59b1e2e95d)
1. [Visual Studio Code](https://code.visualstudio.com/docs/java/java-spring-boot)

[Back](../../tree/spring-boot)
