### Spring Overview

* Client --> web.xml --> Request (send all requests to the dispatcher servlet)
* Front Controller - Dispatcher Servlet (checks xml configuration file)
```web.xml
<servlet>
   <servlet-name>yourservletname</servlet-name>
   <servlet-class>
      org.springframework.web.servlet.DispatcherServlet
   </servlet-class>
</servlet>
<servlet-mapping>
   <servlet-name>yourservletname</servlet-name>
   <url-pattern>/</url-pattern>
</servlet-mapping>
```
* XML Configuration file
   * component-scan
* Annotation @Controller
