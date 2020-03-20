# Creating a Spring Boot Project with vscode.

### Add the following extensions to vscode
1. Spring Boot Extension Pack
1. Spring Initializr Java Support (Similar to Spring Boot Extension Pack)
1. Spring Boot Tools
1. Thymeleaf


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
    public String helloworldRoot(Model model) {
        return "<h1>Hello Spring World</h1>";
    }
}
```

[Back](../../tree/spring-boot)
